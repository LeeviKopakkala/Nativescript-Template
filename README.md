# NativeScript-Angular with Sidedrawer and TabView

## Installation:

### Quick:

1. Install Node.JS https://nodejs.org/

2. Install Nativescript CLI `npm install -g nativescript`
 
3. Check that Nativescript CLI is working `tns`

4. Install Android Studio (OR iOS equivalent) https://developer.android.com/studio/

+ 4.1 Open Android Studio -> AVD Manager -> Create Emulator

5. (Optional but useful) Install https://www.nativescript.org/nativescript-sidekick

### Run:

1. `git clone https://github.com/LeeviKopakkala/movie-app-Nativescript/`

2. `cd movie-app-Nativescript`

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

