# tweak-audiospeaker-android
What is this?
>This is a tweak for audio speaker quality on Android Device that enable both speakers functional, while the one is usually used for calling only or something else. 
But, when enable and switch one else directly, it'll turn out distort. So, we need to set the value for good.

## Installation and Usage
1. Clone This Repository
2. Download ADB
3. On Console, type this command:<br>
`adb pull /system/etc/mixer_paths.xml system/etc/`
4. Patch the file with .patch file provided in this repository with this command:<br>
`patch mixer_paths.xml < tweak_speaker.patch` or `patch < tweak_speaker.patch`
or you can use TortoiseSVN to apply patch. See more about it at [here](https://tortoisesvn.net/docs/nightly/TortoiseMerge_en/tmerge-basics-patch.html)
5. Zip META-INF and system folder
6. Flash via custom recovery
