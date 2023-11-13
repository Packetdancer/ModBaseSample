# User Interaction Sample for ASA Mods

## Summary

This little mod does absolutely nothing other than opening a sample widget. However, it provides two ways to do so; via a hotkey (F10 by default, but it uses a variable so could be set to anything) or a multi-use wheel option. It does so by adding a world singleton (`ModBaseSample_Singleton_BP`) which adds two buffs to every player who spawns:

* `Buff_ModBaseSample_Hotkeys` is an invisible buff which enables input and will listen for a recognized hotkey; upon receiving that key, it will show whatever widget it is set to show.
* `Buff_ModBaseSample_MultiUse` is an invisible buff which adds an option to the Multi-Use menu; when that option is selected, it will show whatever widget it is set to show.

The widget shown is a simple little dialog box that does nothing, but which will appropriately set up user input upon being added to the viewport, and clean up after itself afterwards.

## Use

Just check this project out, and make sure the `ModBaseSample` directory is placed into your `ARKDevkit\Projects\ShooterGame\Mods` directory; you may need to enable the mod in the UGC menu before it will appear. Feel free to use this as the base for a mod, import the files to make use of them in your own mod, whatever. Go nuts!

## Notes

In a real mod, you would almost certainly want to combine the Hotkey and Multi-Use buffs so that you're only adding one persistent invisible buff; they're separated here not for technical reasons but just so that the examples are nicely self-contained in their own buffs.

## Images

![](https://github.com/Packetdancer/ModBaseSample/blob/main/image01.png)

![](https://github.com/Packetdancer/ModBaseSample/blob/main/image02.png)

