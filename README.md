## <p align="center">MSI Z370 Gaming M5</p>

<img align="right" width="287" height="419" src="https://github.com/JackGannonUK/HackintoshEFI/blob/main/assets/about-this-mac.png">

## About
This setup contains what is needed. Nothing more, it is not touched by bloat / any clover patches - it is based upon the principles of minimalism and efficiency. This EFI is contemporized consequently to the current prerequisites of the latest macOS versions. All kexts, drivers and tools have been handpicked for my system - allowing for higher optimizations to my workflow and more.

## Word of Caution
Currently, this EFI is built for [macOS Ventura (Beta 1)](https://www.apple.com/uk/macos/macos-ventura-preview/) as of writing. Therefore, this means quirks, drivers and kexts may be inappropriate for earlier macOS versions. These may damage NVRAM, SSDs and Power Management setups - as they have not been tested. I'd advise caution for utilising this EFI for versions less than macOS Ventura, and would vehemently urge constructing your own via the [Dortania Guide](https://dortania.github.io/OpenCore-Install-Guide/)

## Additions for a working EFI (to run on Ventura)
To successfully boot macOS Ventura on a 300-series chipset, I had to update to the latest Opencore Developer Build to enable the quirk `AvoidRuntimeDefrag` - without this quirk, macOS Recovery would hurl an error describing how I needed to [update my firmware](https://forums.macrumors.com/threads/monterey-install-error.2319354/).

Notable changes made to the EFI to successfully boot macOS Ventura:
- AvoidRuntimeDefrag = True
- AdviseFeatures = True
- ReleaseUsbOwnership = True

*In addition of updated opencore, kexts and drivers.

## Screenshots

!(Screenshot #1)[assets/lightvsdark.png]
![assets/centerstage.png]
![assets/system.png]
![assets/weather.png]
![assets/clock.png]
![assets/light.png]
![assets/dark.png]
