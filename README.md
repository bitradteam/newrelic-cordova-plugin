# New Relic plugin for Cordova

> The official [New Relic](https://newrelic.com/mobile-monitoring) [Cordova](http://cordova.apache.org/) plugin for iOS and Android.

# When added the New Relic Cordova plugin will
* Detect the platforms added to your Cordova application and apply the most recent release of the appropriate New Relic Mobile agent ([Android ](http://docs.newrelic.com/docs/releases/android), [iOS ](http://docs.newrelic.com/docs/releases/ios))
* Add post-build scripts for uploading iOS symbolication files
* Upload Android Proguard mapping files
* Automatically instrument mobile applications built via Cordova

# Installation

### Prerequisites
1. Cordova 4.x or newer
2. Node 6.0 or newer
3. Cordova CLI tools
4. Android and iOS Cordova platforms
5. New Relic Mobile application tokens

### Adding the plugin
Change to your Cordova project directory and add the plugin to your project using the Cordova command line tool. The `--variable` argument is used to pass application tokens to the plugin.
```
# Install from github repository
cordova plugin add https://github.com/nirmal-mobiquity/newrelic-cordova-plugin.git --variable IOS_APP_TOKEN="{ios-app-token}" --variable ANDROID_APP_TOKEN="{android-app-token}"
```
