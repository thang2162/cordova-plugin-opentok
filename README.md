This plugin has been updated to work with Cordova 9.0.0!

* iOS: If the download for OpenTok.framework fails:
1. remove the plugin 'cordova plugin rm cordova-plugin-opentok'
2. remove the ios platform from your project 'cordova platform rm ios'
3. re-add the plugin 'cordova plugin add https://github.com/thang2162/cordova-plugin-opentok.git'
4. manually download the file (https://s3.amazonaws.com/artifact.tokbox.com/rel/ios-sdk/OpenTok-iOS-2.15.3.tar.bz2)
2. unpack and place OpenTok.framework in 'plugins/cordova-plugin-opentok/src/ios'
6. re-add the ios platform  'cordova platform add ios'

# Cordova Plugin for OpenTok iOS and Android
![OpenTok Labs](https://d26dzxoao6i3hh.cloudfront.net/items/0U1R0a0e2g1E361H0x3c/Image%202017-11-22%20at%2012.16.38%20PM.png?v=2507a2df)

##### Disclaimer: This plugin is based on the [Cordova OpenTok Plugin](https://github.com/songz/cordova-plugin-opentok/). Please keep in mind that this is an OpenTok Labs project which means that it's not officially supported by TokBox.

## Sample code 
To see the plugin in action, please check out [opentok-cordova-samples.](https://github.com/opentok/opentok-cordova-samples)

## Using Cordova CLI
Make sure You have Cordova 3.5.0 or greater installed. If you haven't, take a look at the [Cordova instructions](http://cordova.apache.org/docs/en/3.5.0/guide_cli_index.md.html) Page.

1. Clone this repo to get the source code for the OpenTok Cordova plugin

2. To install the OpenTok Cordova plugin, run the following command in the root of your project:
```
cordova plugin add https://github.com/thang2162/cordova-plugin-opentok.git
```  
3. To remove OpenTok Cordova plugin 3.2.0 and above, use the following command:
``` 
cordova plugin remove cordova-plugin-opentok
```
4. To remove the old OpenTok Cordova plugin, use the following command:  
``` 
cordova plugin remove com.tokbox.cordova.opentok
```

## Getting Started on your Project:
All your editing will be done in your www folder.

To use the opentok library, make sure you include `opentok.js` file in your HTML document.  
` <script type="text/javascript" charset="utf-8" src="opentok.js"></script>`

All JavaScript code should be written in `onDeviceReady` function in `/js/index.js` because it is executed after all dependencies has loaded.
```
    onDeviceReady: function() {
        // Do Your Stuff Here!
    }
```

# Development and Contributing

Interested in contributing? We love pull requests! See the
[Contribution](CONTRIBUTING.md) guidelines.
