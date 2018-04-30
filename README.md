ANNOUNCING RECALBOX FOR THE ROCK64 - ALPHA RELEASE

After many efforts with much teamwork, collaboration, and testing, we are very excited to provide the ALPHA release of RECALBOX for the ROCK64 board! 

-- The download is located under this repository's releases --
https://github.com/mrfixit2001/recalbox_rock64/releases

Details on the ROCK64 SoC can be found here:
https://www.pine64.org/?page_id=7147

For those of you unfamiliar with Recalbox:
https://www.recalbox.com/
"Recalbox offers a wide selection of consoles and game systems. From the very first arcade systems to the NES, the MEGADRIVE, 32-bit platforms (such as the Playstation) and even Nintendo64. With Kodi already includeed, Recalbox also serves as a Media Center. By connecting it to your home network, you will be able to stream videos from any compatible devices (NAS, PC, External HDD, etc.)."

Please do keep in mind that this is an ALPHA release, which means you should EXPECT some things not to work. We have done a fair amount of testing on our own to try and resolve as many issues as we can before this release, but now you get to help! (Lucky you!) So if/when you do find things that don't work right, please use the link in github to report the issue. 

When reporting issues:
 - Provide logs or screenshots of the issue so that we can see the error(s) you are seeing
 - Provide detailed steps for us to follow in order to reproduce the issue

A few things you can expect not to work or be included (yet):
 - Amstrad (Caprice) Emulator
 - Dreamcast (Reicast) Emulator
 - SPI booting from USB

Some things we have added:
 - Upgraded Kodi (and addons) from Krypton to Leia
 - InputStream.Adaptive Kodi Addon
 - Multiple N64 cores so that you can select which core works best for you on each ROM!
 - Overclocked the CPU and the GPU by default

Some things we have tested:
 - Bluetooth and Wifi adapters from the Pine store have been tested and work for sure
 - N64 core named "n64" is "GLES2N64" and runs Mario Kart pretty smoothly

Some important notes:
 - Sometimes when the image first boots there can be a delay. Please be patient and let this complete. It should not happen on every boot.
 - We highly recommend that you install a heatsink on the board. The temp without a heatsink sit at 76*C when in EmulationStation - which is just 4*C under thermal throttling. With a heatsink - even a poor one - the temps are at approx. 66*C and around 73*C when playing mariokart (24*C ambient temp). 

The alpha release is just the compiled image at this time while the source is cleaned up and organized in preparation to be made available for the recalbox team to maintain. The source code will be added to this same repository as soon as possible. 

Lastly, please remember this is a community build, and just something I've worked on in my free time. There's no pressure at all, but if you appreciate the work then feel free to send me a buck on paypal: mrfixit2001 at gmail.

Special thanks go out to Substring at Recalbox and LukasZ at Pine64 for all their efforts in testing and feedback!
