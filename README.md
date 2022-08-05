# The Alcatel Quickflip (4044C)
This phone, man. I bought this flip phone during my senior year of high school - mostly as a joke. But now we're here, and I still have the phone. This phone, in terms of useability, rocks. It does exactly what you need it to do; it can send and receive text messages and phone calls. It can even connect to the internet.
Unfortunately, Alcatel didn't seem to like this phone very much - or maybe it was Kai OS Technologies, the company behind the phone's operating system, KaiOS. Whoever gave the phone the axe beside, the phone runs KaiOS 1.0 which has more or less zero support by Kai OS Technologies. There is sparse documentation on this version of the OS and most searches will only result in help for the later versions of the OS.
KaiOS 1.0 doesn't have an app store, and there's no official way to install 3rd-party applications onto the device. Not only that, but somebody made the decision for this 4044 phone to not be allowed adb access. Through some research I was finally able to find [this github guide](https://github.com/chin123/archlinux-4044C) that explained how to install an arch linux chroot on this specific 4044C flip phone. I didn't really want to do this, but the method showed how to access EDL on the phone which then showed me how to read and write partitions.
## EDL mode and how to use it
Before continuing, there are a few things you will need in order to actually read and write partitions:
1. The phone
2. https://github.com/andybalholm/edl
3. [The firehose file in misc folder](https://github.com/chin123/archlinux-4044C)

I would recommend using a linux environment for this - I couldn't get the phone to be detecting by the edl script in windows but when I switched to linux it worked without issue.

To enter EDL mode on the flip phone, first power off the phone. After that, hold down both volume up and down buttons and while holding them down, plug in the phone to the computer. A screen will pop up saying "Entering downdload mode" once that appears, let go of the volume down button, and once the screen turns black you're in EDL mode.
