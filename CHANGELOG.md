<a href="https://www.patreon.com/vladimirkharlampidi"><img src="https://cdn.framework7.io/i/support-badge.png" height="20"></a>

# Change Log

# [v3.0.2](https://github.com/framework7io/framework7-cli/compare/v2.3.3...v3.0.0) - October 7, 2019
  * Fixed typo in prop (`breanpoint` -> `breakpoint`) name in generated Vue split-view template

# [v3.0.1](https://github.com/framework7io/framework7-cli/compare/v2.3.3...v3.0.0) - October 7, 2019
  * Fixed issue with unable to create app without bundler

# [v3.0.0](https://github.com/framework7io/framework7-cli/compare/v2.3.3...v3.0.0) - October 7, 2019
  * Generated app templates updated to Framework7 v5
  * Generated app templates updated to use Framework7 Icons v3
  * Update cordova `backbutton` handler. Now it will close opened modals (if available) or go back in navigation
  * Updated cordova-related scripts names, e.g. `build-cordova-dev` -> `build-dev-cordova`
  * Added alias `f7` for CLI command. Now we can run it like `f7 create --ui`
  * UI
    * Added new Text Editor to custom build settings
    * Added options to include/exclude Dark and Light themes in custom build
    * Added ability to import project setting from JSON file
    * Added ability to export project setting to JSON file

# [v2.3.3](https://github.com/framework7io/framework7-cli/compare/v2.3.2...v2.3.3) - July 5, 2019
  * Added `--skipUpdate` parameter to `create` and `generate-assets` commands to skip update check
  * Fixed CLI usage text

# [v2.3.2](https://github.com/framework7io/framework7-cli/compare/v2.3.1...v2.3.2) - May 25, 2019
  * UglifyJS webpack plugin replaced with Terser

# [v2.3.1](https://github.com/framework7io/framework7-cli/compare/v2.3.0...v2.3.1) - May 22, 2019
  * Now created project will contain default `.gitignore` file
  * Added Treeview component to the custom build components list
  * `cordova-plugin-wkwebview-file-xhr` plugin will be always used instead of `cordova-plugin-wkwebview-engine`

# [v2.3.0](https://github.com/framework7io/framework7-cli/compare/v2.2.0...v2.3.0) - May 1, 2019
  * All new UI 🎉
    * Now it is possible to change `cwd` (project destination)
    * Advanced webpack configuration
    * Advanced pre-installed Cordova plugins configuration
    * More theming options with instant theming preview - dark mode, fill-style navigation bars
    * New custom build section (for webpack + Less only)
  * Fixed electron settings file reference
  * Minor fixes

# [v2.2.0](https://github.com/framework7io/framework7-cli/compare/v2.1.3...v2.2.0) - April 22, 2019
  * Electron build 🖥🎉
  * Now it uses `cordova-plugin-wkwebview-file-xhr` (where local XHR works) iOS plugin when no-bundler used
  * Lots of minor improvements

# [v2.1.3](https://github.com/framework7io/framework7-cli/compare/v2.1.2...v2.1.3) - April 8, 2019
  * Fixed issue when webpack build could remove `type="text"` attributes from inputs

# [v2.1.2](https://github.com/framework7io/framework7-cli/compare/v2.1.1...v2.1.2) - April 8, 2019
  * Fixed issue when `build-cordova-android-prod` script generated iOS app instead of Android

# [v2.1.1](https://github.com/framework7io/framework7-cli/compare/v2.1.0...v2.1.1) - March 25, 2019
  * Update Sharp lib to latest

# [v2.1.0](https://github.com/framework7io/framework7-cli/compare/v2.0.4...v2.1.0) - March 25, 2019
  * Templates updated to be compatible with new Aurora theme
  * There is a new option on app creation that allows to exclude Framework7 Icons and Material Icons fonts
  * Webpack config:
    * `watchOptions.poll` changed to `1000` (1s) to decrease CPU overload
  * New Webpack NPM scripts:
    * `build-dev` - build web app using development mode (faster build without minification and optimization)
    * `build-cordova-dev` - build cordova's `www` folder from and build cordova app using development mode (faster build without minification and optimization)
    * `build-cordova-ios-prod` - to build only iOS app
    * `build-cordova-ios-dev` - to build only iOS app in dev mode
    * `build-cordova-android-prod` - to build only Android app
    * `build-cordova-android-dev` - to build only Android app in dev mode
  * New NPM scripts when Webpack is not used:
    * `build-cordova-ios` - to build only iOS app
    * `build-cordova-android` - to build only Android app
