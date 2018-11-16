 <img height="100px" src="https://www.azoft.com/wp-content/uploads/2017/10/nativescript@3x.png"/>

<p align="center">
  <img height="125px" src="https://angular.io/assets/images/logos/angular/angular.png">
 <img height="400px" src="https://d2odgkulk9w7if.cloudfront.net/images/default-source/home/header-graphic-hp-min.png?sfvrsn=31b70efe_6">
 <img height="125px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4f/NativeScript_logo.png/220px-NativeScript_logo.png">
</p>

<a align="center" href="https://leevikopakkala.github.io/Nativescript-Template/">https://leevikopakkala.github.io/Nativescript-Template/</a>
# NativeScript-Angular with Sidedrawer and TabView

This is the ultimate template with improved structure to help you launch your first app or customer project in no-time.

## Overview

We all know the slow process of setting up the project and creating functioning base before being able to add features.
With this template you get fully functioning application out of the box with Sidedrawer and Tabview.

> Perfect for beginners and professionals alike.

Using the best practices, develop your first real mobile application in no-time.

Nativescript Template composed of Nativescript Sidedrawer and Tabview components:

References to individual plugins used in this template:
* https://market.nativescript.org/plugins/tns-template-drawer-navigation-ng
* https://market.nativescript.org/plugins/tns-template-blank-ng
* https://market.nativescript.org/plugins/tns-template-tab-navigation-ng

<p align="center">
 <img height="400px" src="https://raw.githubusercontent.com/NativeScript/template-drawer-navigation-ng/HEAD/tools/assets/phone-drawer-ios.png">
 </p>


## Installation:

<p align="center">
  <img height="500" src="https://media.discordapp.net/attachments/499833921513586688/512377387296489497/unknown.png?width=1130&height=677">
</p>

### Quick:

1. Install Node.JS https://nodejs.org/

2. Install Nativescript CLI `npm install -g nativescript`
 
3. Check that Nativescript CLI is working `tns`

4. Install Android Studio (OR iOS equivalent) https://developer.android.com/studio/

+ 4.1 Open Android Studio -> AVD Manager -> Create Emulator

5. (Optional but useful) Install https://www.nativescript.org/nativescript-sidekick

### Run:

1. `git clone https://github.com/LeeviKopakkala/Nativescript-Template`

2. `cd Nativescript-Template`

3. `tns device android --available-devices` OR `tns device ios --available-devices`

4. `tns run android` / `tns run android --device {device name}` OR `tns run ios` / `tns run ios --device {device name}

**IF USING SIDEKICK**

4. Open Sidekick

+ 4.1 Add Project

+ 4.2 Select Emulator

+ 4.3 Run



### Architecture

The RadSideDrawer component is set up as an application starting point in:

- `/app-component.ts` - sets up the side drawer content and defines a page router outlet for the pages.

RadSideDrawer has the following component structure:

- `RadSideDrawer` - The component to display a drawer on the page.
- `tkDrawerContent` directive - Marks the component that will hold the drawer content.
- `tkMainContent` directive - Marks the component that will hold the app main content.

There are five blank components located in these folders:

- `/browse`
- `/featured`
- `/home`
- `/search`
- `/settings`

### Styling

This template is set up to use SASS for styling. All classes used are based on the {N} core theme – consult the [documentation](https://docs.nativescript.org/angular/ui/theme.html#theme) to understand how to customize it. Check it out to see what classes you can use on which component.

It has 4 global style files that are located at the root of the app folder:

- `_app-variables.scss` - holds the global SASS variables that are imported on each component's styles.
- `_app-common.scss` - the global common style sheet. These style rules are applied to both Android and iOS.
- `app.android.scss` - the global Android style sheet. These style rules are applied to Android only.
- `app.ios.scss` - the global iOS style sheet. These style rules are applied to iOS only.

