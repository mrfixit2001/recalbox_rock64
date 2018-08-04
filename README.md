ANNOUNCING RECALBOX FOR THE ROCK64 - BETA RELEASE

After many efforts with much teamwork, collaboration, and testing, we are very excited to provide the BETA release of RECALBOX for the ROCK64 board! 

-- The download is located under this repository's releases --
https://github.com/mrfixit2001/recalbox_rock64/releases

Details on the ROCK64 SoC can be found here:
https://www.pine64.org/?page_id=7147

For those of you unfamiliar with Recalbox:
https://www.recalbox.com/
"Recalbox offers a wide selection of consoles and game systems. From the very first arcade systems to the NES, the MEGADRIVE, 32-bit platforms (such as the Playstation) and even Nintendo64. With Kodi already included, Recalbox also serves as a Media Center. By connecting it to your home network, you will be able to stream videos from any compatible devices (NAS, PC, External HDD, etc.)."

Please do keep in mind that this is a BETA release, which means it’s hugely improved from the ALPHA release but you should still EXPECT some things not to work quite right. We have done a LOT of testing on our own to try and resolve as many issues as we can before this release, but now you get to help! (Lucky you!) So if/when you do find things that don't work right, please use the link in github to report the issue.

When reporting issues:
 - Provide logs or screenshots of the issue so that we can see the error(s) you are seeing
 - Provide detailed steps for us to follow in order to reproduce the issue

A few things you can expect not to work or be included (yet):
 -  Remapping the buttons on some controllers, such as 8BitDo, cause the controller to not work in the emulators – use the default keymaps for these
 -  Resolution for Emulators and EmulationStation is 1080p, manual config edit will be needed to change: 
    o Mount the BOOT partition and edit /boot/extlinux/extlinux.conf -- look for the following value: video=HDMI-A-1:1920x1080@60. Edit to your desired resolution. 
    o NOTE: Resolution in KODI can be adjusted without any config changes (up to 4k!)
 -  Netflix Kodi app is included – you can login but it does not currently play anything (yet)

Some things we have added to Recalbox that are Rock64 Exclusive:
 -  Upgraded Kodi (and addons) from version 17 (Krypton) to a July 2018 commit of version 18 (Leia)
 -  InputStream.Adaptive Kodi Addon
 -  Multiple cores for different emulators so that you can select which core works best for you on each ROM!
 -  Slight default overclock

Improvements since Alpha:
 -  Most Bluetooth and Wifi adapters will now work, including these which are 2-in-1 so that you only need to use one USB port to add both Wifi AND BT:
    - https://www.amazon.com/Wireless-Bluetooth-Adapter-Supports-OS10-9-10-13/dp/B01JYE5BT2/ref=sr_1_2_sspa?ie=UTF8&qid=1532357324&sr=8-2-spons&keywords=wifi+bluetooth+adapter&psc=1
    - https://www.amazon.com/Edimax-EW-7611ULB-Wi-Fi-Bluetooth-Adapter/dp/B01KVZB3A4/ref=sr_1_4?ie=UTF8&qid=1532357324&sr=8-4&keywords=wifi+bluetooth+adapter
 -  Boot from all storage mediums (SD, eMMC and USB) is now supported
 -  Overclocking options from the ES menu (NOTE: we highly suggest active cooling if you don’t use default)
 -  Updated versions of retroarch and most emulators + cores
 -  All emulators working - including PSP, Dreamcast, and Amstrad
 -  Additional Emulators Included:
    - virtualjaguar
    - uae
    - theodore
    - pocketsnes
    - melonds
    - desmume
    - beetle-psx
    - 4do
    - hypseus
    - vice
 -  Included Wolfenstein 3D (shareware version) in DosBox
 -  LED blinking with disk activity
 -  KODI 4K 60FPS with kwiboo’s HDR enhancement
 -  HD Audio with Selectable Output from ES Menu (HDMI, headphone jack, SPIDF)
 -  CEC working in KODI
 -  IR working in KODI – supports multiple remotes out of the box, including the Pine64 / Rockbox remote
 -  Newest Recalbox Version - with Built-In Netplay Features!
 -  Clean boot without messages
 -  Many additional controllers / gamepads are now supported 
 -  Custom kernel (previously borrowed from LE)
 -  Full range HDMI
 -  Added some default shader presets and default cores
 -  Updated Library Versions with Buildroot 2018.2-3
 -  Custom patches to ES and Emulators to improve overall stability

Some important notes:
 -  When the image first boots, you can expect a delay as the partition is expanded to the full size of your disk. Please be patient and let this complete. It will not happen on every boot.
 -  N64 has multiple cores, different ROMS work better with different cores! For example, Mario Kart and Perfect Dark both perform very well using the N64 core (which is “GLES2N64”).
 -  PSP and NDS will run slowly overall, this is not a bug, they are just very demanding of the hardware. Some games will be playable however, and PSP mini ROMs run quite well.
 -  Some emulators / cores are highly dependent on a valid BIOS files being installed (Dreamcast, for example). Be sure to read the documents in the system’s ROM folder for details on what BIOS files are needed. Further documentation is available on the Recalbox wiki.
 -  A single ROM not working is not considered a “bug”, it’s often an incompatibility with the ROM and the emulator or core. We have provided multiple cores for some emulators to try and help maximize the number of ROMS that work.
 -  If you are suddenly and unexpectedly thrown into KODI, then that means EmulationStation may have crashed. Please provide your /recalbox/es.log file so we can review.
 -  We highly recommend that you install a heatsink on the board when you select a non-default overclock! 

"Where's the source code?"
The source is in the final stages of being cleaned up and organized in preparation to be made available for the recalbox team to maintain, instead of having it hosted in this repository. Merging it with the recalbox repo allows them to maintain and update it, which ensures that you will receive their updates as they are made available. 

Lastly, please remember this is a community build, and just something I've worked on in my free time. There's no pressure at all, but if you appreciate the work then feel free to send me a buck on Paypal: mrfixit2001 at gmail.

Special thanks go out to Kwiboo from LibreELEC, Substring at Recalbox, and LukasZ at Pine64 for their efforts in testing and feedback!

- Mr Fix-IT
