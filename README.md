
# Philips Hue Plugin for Elgato Stream Deck 
# UPDATE INFORMATION

## There's a new version of the Philips Hue plugin available on the [Elgato Marketplace](https://marketplace.elgato.com/product/philips-hue-27f49792-2de3-455f-8892-fd382716f548).

You'll find that version [here](https://marketplace.elgato.com/product/philips-hue-27f49792-2de3-455f-8892-fd382716f548)

New discussions/support will move to [Discord](https://discord.gg/elgato)

The new version of the plugin should work with all recent Philips Hue Bridges (sold like 6-7 years ago).

**If you have the original plugin installed, please, first install the update to the old plugin** [Philips-Hue original plugin 1.6.8](https://github.com/user-attachments/files/15746596/com.elgato.philips-hue.streamDeckPlugin.zip), or remove it - otherwise your sidebar gets mixed up...

You can install both versions (old and new) in parallel without problems, but it has no benefits. The new version is far more capable than the legacy version.

<img width="952" alt="CleanShot_2024-06-08_08 35 59" src="https://github.com/elgatosf/streamdeck-philipshue/assets/80752/621322d9-5e19-42fb-aec4-7fce9a11aac6">


----

(The notes below are kept for reference)

## Philips Hue Plugin for Elgato Stream Deck (legacy version)
This sample plugin allows controlling `Philips Hue` lights in your network. It's a demonstration of the [Stream Deck SDK](https://developer.elgato.com/documentation/stream-deck/).
Since version 1.6.0, it also supports the Stream Deck +. The brightness-action contains an example of how to change the display of the dial-control's touch-panel.

## Version 1.6.7 is also available in the Stream Deck Store!

## Features
- Code written in JavaScript
- Cross-platform (macOS, Windows)
- Localized
- Basic support for Stream Deck +

![](screenshot.png)


# Installation
In the [Release](./Release) folder, you can find the file `com.elgato.philips-hue.streamDeckPlugin`. If you double-click this file on your machine, Stream Deck will install the plugin.


# Source code
The [Sources](./Sources) folder contains the source code of the plugin.

# Changes
## 1.6.4
- fixed/improved support for temperature actions
- PI now lets you only select lights for a temperature action if they support color temperature

## 1.6.3
- updated CSS to the latest versions of our SDK-libs
- added an option to the PI to allow larger steps if you rotate dials (1,2,3,4,5,10).

## 1.6.0
- fixed broken localizations
- changed versioning to semver
- added basic support for Stream Deck +

# How it works (since 1.6.0)
![](touchpanel.png)

 You can now drag a brightness-/ or temperature-action to a SD+ dial-control. It supports these actions:
 - Turn the dial to change the brightness/temperature
 - Press the dial to:
 - - set the brightness/temperature to the configured value - if the light is on
 - - turn the light on - if the light is off
 - Long-Press the dial to toggle the light on/off
 - Tap the touch-panel to toggle the light on/off
  
 DialStacks are not properly supported yet.

