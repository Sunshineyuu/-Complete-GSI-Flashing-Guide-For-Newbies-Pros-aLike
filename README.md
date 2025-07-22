# 🌿Complete-GSI-Flashing-Guide-For-Newbies-Pros-aLike

Flash Generic System Image [GSI] on any Treble-compatible Android device!

⟩ Treble check app🌿:
https://t.me/Customromsupporthub/51

🪴Requirement;
> Bootloader unlock

____

🌴Downloads You’ll Need:

🌿 GSI ROM (example: system.img)
🌿 VNDK-compatible VBMeta.img (optional but recommended)
🌿 Platform Tools (ADB & Fastboot)
🌿 Custom Recovery (.img like TWRP or Lineage Recovery)
🌿 Correct Firmware/Stock ROM (just in case something breaks)
🌿 Google USB Drivers
🌿 A working brain & charged battery 🔋😄


🌴Preparation Time:

🪴 Extract everything into a folder:

Desktop > GSI_FlashKit 

🪴 Rename the GSI to  system.img

🪴Optional: Rename vbmeta to  vbmeta.img

___

🌴Enable USB Debugging: 

> Go to Settings > About Phone > Tap Build Number 7x

> Enable Developer Options

> Turn on USB Debugging and OEM Unlocking


🌿Connect & Authorize ADB:

CMD: adb devices

> Accept the pop-up on the phone ✅

Then reboot to fastboot:

CMD: adb reboot bootloader

____

⚡ Flashing Steps: [Fastboot Method]

[ Most common method for GSIs ]


⚠️Erase Existing System:

fastboot erase system
fastboot erase product
fastboot erase vendor
fastboot erase userdata

[ Some devices require only system & userdata, but this clears leftover junk ]


🌿Flashing the GSI:

CMD: fastboot flash system system.img

CMD: fast flash vbmeta vbmeta.img [Optional]

🪴 Disable Android Verified Boot [ Optional, but Important ] :

fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img

⚠️ If you don’t flash vbmeta, some devices will bootloop or hang on boot logo.

___

🌴 Factory Reset / Wipe Data:

CMD: fastboot -w

> Avoid skipping this step unless you enjoy bootloops 😜


🌴 Reboot & Pray:

CMD : fastboot reboot


🌴 First Boot Can Take 5–10 Minutes . . .

> Boot time varies depending on the GSI and device specs.

___

🌿Post-Boot Checklist:

☑️ Set up your device
☑️ Check for no signal or no audio bugs
☑️ If broken, try another GSI variant [ A-only vs AB, vndklite, etc...]

____

🌴Tips for Troubleshooting ⚠️ 

🪴 No boot?
Try with --disable-verification vbmeta and full wipe.

🪴 Boot loops?
Use GSI that's compatible with your device's vendor version.

🪴 No signal or Wi-Fi?
Try "vndklite" or "lite" GSI builds. Some require custom vendor patching.
____

💾 Optional Extras:

🪴Magisk Root
Flash  Magisk.zip in recovery after boot
OR patch  boot.img and flash via fastboot:

CMD: fastboot flash boot magisk_patched.img

_____

⚠️Backup before playing with system!
Use custom recovery or TWRP’s Backup feature.

_____

🌿Terms to Know:

GSI               » Generic System Image
VNDK           » Vendor Native Development Kit
AVB               » Android Verified Boot
AB / A-only   » Partition layout types

____________

You're All Set! & Completed ✅
____________
___

🌴Welcome to the World of Android 🌿... 
Clean » Lean » Pure Android...
_ _ _ _

Updates~[Sunshineyou_enigma](https://t.me/Sunshineyou_enigma) 🌿
Join [customromsupportofficial](https://t.me/customromsupportofficial) 🌿
Follow [customromsupportHUB](https://t.me/Customromsupporthub)🌿
