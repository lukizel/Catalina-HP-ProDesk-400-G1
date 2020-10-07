# macOS Catalina on the HP ProDesk 400 G1

[⬅️ Previous: Mojave](https://github.com/lukizel/Mojave-HP-ProDesk-400-G1) | [Next: Big Sur ➡️](https://github.com/puuska/Hackintosh-HP-ProDesk-400-G1)

| Hardware    | Details                |
| ----------- | ---------------------- |
| Processor   | Intel Core i3-4130     |
| Graphics    | integrated (HD4400)    |
| Sound       | Realtek ALC221 (11/15) |
| Networking  | Realtek RTL8168G       |
| Motherboard | HP 18E9                |

![Desktop screenshot](https://i.imgur.com/kzNZ5Re.png)

# Improvements over Mojave guide

- Newer .kext versions (Lilu, WhateverGreen etc.) - I still recommend upgrading them whenever possible, though.
- New, "improved" USBMap.kext - **this might cause issues on your build** - make your own version and replace it after installation.
- Sleep, sound, USB work natively. Absolutely no issues with apps that require lower-level access such as checkra1n.

# Installation

As simple as always, just make a Catalina install thumb drive (or, if you're on Windows/Linux use Olarila builds and replace the EFI partition), install Clover onto it, replace the fresh EFI partition's Clover folder with the one supplied in this repo and install the system. 

Do not configure iCloud in the first setup, make sure you fix USBMap and change all the device identificators in SMBIOS first (S/N etc.). 

After fixing USBMap and replacing SMBIOS identificators (I recommend Clover Configurator for that), you can log in to iCloud without any issue. You're done!

# Issues

- VGA output isn't working (who would have guessed?)
- TV app is unstable, Sidecar isn't working (or at least I assume it isn't working, I can't test it)

# Credits

Thanks to:

- [the Clover team for Clover](https://github.com/CloverHackyColor/CloverBootloader/releases)
- [Acidanthera](https://github.com/acidanthera) for VirtualSMC, Lilu and WhateverGreen
- [puuska](https://github.com/puuska) for the Mojave guide
- [bieleckipawel](https://github.com/bieleckipawel) for the Big Sur guide (both were really helpful while creating this one)
