# Bye Bye Windows

If nothing, this is a checklist for me to use when I reinstall Linux.

## Get Pop!_OS

It's the best!

I'm using 20.10. It comes with gnome 3.38, which is not yet supported by many extensions, but it's working out well for me.

https://pop.system76.com/

Also, did I tell you it uses systemd-boot instead of Grub? I might change this later to use btrfs instead of ext4.
Update before you go ahead.

## Get VScode

And Chrome, if you're into it. They're available in the Pop_Shop!

## Touchpad gestures

Install this: https://github.com/bulletmark/libinput-gestures
Here is my conf file. Gives MacOS/Windows 10 like gestures.
```conf
gesture swipe up	xdotool key super
gesture swipe down	xdotool key super
gesture swipe left	_internal ws_up
gesture swipe right	_internal ws_down
gesture pinch in	xdotool key super+a
gesture pinch out	xdotool key super
```

## Get Workspaces to Dock

https://github.com/RensAlthuis/workspaces-to-dock

The biggest problem with workspaces to dock is it's default configuration. Let's change it:
- General
  * Set dock position to Top
  * Set use horizontal switching
  * Set extend dock to fill screen
  * Set Center the dock
  * Top and Bottom margin: 0
  * Padding 10
- Behavior
  * Unset toggle overview with right click
  * Turn on intelligent hiding
  * Turn on Autohide
  * Turn off Intellihide
  * Set partial/full dock as you like. I like full dock.
- Thumbnails
  * I disabled customisation of thumbnails and captions
- Favorites
  * I disabled favorites

## Get Gnome Tweaks
- Workspaces: Dynamic
- Touchpad: Natural scrolling
- Fonts: Change font sizes here

## Make netflix quality better

Netflix sets video quality to 720p on Linux. Search for "test patterns" it shows video quality on top right.

Try this firefox extension: https://addons.mozilla.org/en-US/firefox/addon/netflix-1080p-firefox/

## Improve bluetooth audio quality

The default audio codec for bluetooth audio on linux is SBC. If your headphones support better codecs (and the should!), install this: https://github.com/EHfive/pulseaudio-modules-bt

Google and find out what codecs your headphones support. Change to a better codec in settings > sound.

https://kn100.me/improving-bluetooth-audio-linux/
