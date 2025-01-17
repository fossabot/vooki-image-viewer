# VookiImageViewer
Lightweight image viewer for a fast image preview. It has been developed to have the same viewer available for all major operating systems - Microsoft Windows 10, MacOS and GNU/Linux.

The main goal is to have a free of charge cross-platform viewer with a simple design and minimum functions which are commonly used.

- Transformations
  - Flip _(horizontal, vertical)._
  - Rotation _(clockwise and counterclockwise in 90° steps)._
  - Zoom _(in, out, original size, fit to window)._
- Fullscreen or Window mode.
- Custom background color.
- Custom image border color.
- Remembers recent files.
- Supports Apple high definition trackpad gestures.

![Application screenshot](src/resource/readme/screenshot_2017-10-19_21-24-02.png?raw=true "")
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fvookimedlo%2Fvooki-image-viewer.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fvookimedlo%2Fvooki-image-viewer?ref=badge_shield)

Supported image formats cover the very common formats as well as the rare ones. Viewer does not intentionally [demosaic][1] the RAW images, but only displays the embedded thumbnail.


| FORMAT             | DESCRIPTION                                      |
|--------------------|--------------------------------------------------|
| GIF                | Graphic Interchange Format                       |
| JPG                | Joint Photographic Experts Group                 |
| PNG                | Portable Network Graphics                        |
| PBM                | Portable Bitmap                                  |
| PGM                | Portable Graymap                                 |
| PPM                | Portable Pixmap                                  |
| XBM                | X11 Bitmap                                       |
| XPM                | X11 Pixmap                                       |
| SVG                | Scalable Vector Graphics                         |
| BMP                | Windows Bitmap                                   |
| XCF                | Gimp                                             |
| PSD                | Photoshop Documents                              |
| RAS                | Sun Raster                                       |
| PCX                | Personal Computer Exchange                       |
| RGB, RGBA, SGI, BW | SGI Images                                       |
| PIC                | Softimage                                        |
| TGA                | Targa                                            |
| TIFF               | Tagged Image File Format
| ARW                | Sony Alpha Raw [Inner thumbnail only]            |
| CR2                | Canon Raw Version 2 [Inner thumbnail only]       |
| DNG                | Digital Negative [Inner thumbnail only]          |
| ERF                | Epson RAW File [Inner thumbnail only]            |
| MOS                | Leaf Raw Image File [Inner thumbnail only]       |
| MRW                | Konica Minolta RAW [Inner thumbnail only]        |
| NEF                | Nikon Raw Image File [Inner thumbnail only]      |
| ORF                | Olympus Raw Image File [Inner thumbnail only]    |
| PEF                | Pentax Raw Image File [Inner thumbnail only]     |
| RAF                | Fuji Raw Image File [Inner thumbnail only]       |
| RW2                | Panasonic RAW Image File [Inner thumbnail only]  |
| SRW                | Samsung RAW Image File [Inner thumbnail only]    |
| X3F                | SIGMA X3F Camera RAW File [Inner thumbnail only] |
| [MacOS/Windows only] HEIC| High Efficiency Image File Format            |


All operations have assigned shortcuts and all of them can be user re-assigned except the one which is used for Preferences on MacOS.


| MacOS            | Windows                     | GNU/Linux                   | OPERATION                                |
|------------------|-----------------------------|-----------------------------|------------------------------------------|
| ﻿<kbd>﻿⌥c</kbd>  | <kbd>ALT</kbd>+<kbd>c</kbd> | <kbd>ALT</kbd>+<kbd>c</kbd> | Clear recent file                        |
| ﻿<kbd>﻿q</kbd>   | <kbd>q</kbd>                | <kbd>q</kbd>                | Quit application                         |
| ﻿<kbd>﻿﻿⌘,</kbd> | <kbd>p</kbd>                | <kbd>p</kbd>                | Preferences                              |
| ﻿<kbd>﻿f</kbd>   | <kbd>f</kbd>                | <kbd>f</kbd>                | Show image in fullscreen mode            |
| ﻿<kbd>﻿,</kbd>   | <kbd>,</kbd>                | <kbd>,</kbd>                | Rotate left                              |
| ﻿<kbd>﻿.</kbd>   | <kbd>.</kbd>                | <kbd>.</kbd>                | Rotate right                             |
| ﻿<kbd>﻿h</kbd>   | <kbd>h</kbd>                | <kbd>h</kbd>                | Flip horizontally                        |
| ﻿<kbd>﻿v</kbd>   | <kbd>v</kbd>                | <kbd>v</kbd>                | Flip vertically                          |
| ﻿<kbd>﻿+</kbd>   | <kbd>+</kbd>                | <kbd>+</kbd>                | Zoom in                                  |
| ﻿<kbd>﻿-</kbd>   | <kbd>-</kbd>                | <kbd>-</kbd>                | Zoom out                                 |
| ﻿<kbd>﻿*</kbd>   | <kbd>*</kbd>                | <kbd>*</kbd>                | Zoom reset                               |
| ﻿<kbd>﻿w</kbd>   | <kbd>w</kbd>                | <kbd>w</kbd>                | Fit to window                            |
| ﻿<kbd>﻿[</kbd>   | <kbd>[</kbd>                | <kbd>[</kbd>                | Previous image                           |
| ﻿<kbd>﻿]</kbd>   | <kbd>]</kbd>                | <kbd>]</kbd>                | Next image                               |
| ﻿<kbd>﻿i</kbd>   | <kbd>i</kbd>                | <kbd>i</kbd>                | Scroll up                                |
| ﻿<kbd>﻿k</kbd>   | <kbd>k</kbd>                | <kbd>k</kbd>                | Scroll down                              |
| ﻿<kbd>﻿j</kbd>   | <kbd>j</kbd>                | <kbd>j</kbd>                | Scroll left                              |
| ﻿<kbd>﻿l</kbd>   | <kbd>l</kbd>                | <kbd>l</kbd>                | Scroll right                             |
| ﻿<kbd>﻿s</kbd>   | <kbd>s</kbd>                | <kbd>s</kbd>                | Toggle statusbar                         |
| ﻿<kbd>﻿n</kbd>   | <kbd>n</kbd>                | <kbd>n</kbd>                | Toggle filesystem navigation             |
| ﻿<kbd>﻿t</kbd>   | <kbd>t</kbd>                | <kbd>t</kbd>                | Toggle toolbar                           |
| ﻿<kbd>﻿F1</kbd>  | <kbd>F1</kbd>               | <kbd>F1</kbd>               | About application                        |
| ﻿none            | none                        | none                        | About components                         |
| ﻿none            | none                        | none                        | About Qt                                 |
| ﻿none            | none                        | none                        | About supported formats                  |

All code developed during this project is [GPLv3][2] licensed. Images as well as the 3rd-party components have their own licenses, see proper LICENSE files in a [GitHub Source Tree][3].

-----------------

## Releases
[Prebuilt binaries][5] for Windows 7, Windows 10 and MacOS as well as sources are available [here.][5]
Unix binaries are not prebuilt and can be easily built from sources.

Mac users can install the VookiImageViewer by Homebrew.
```
brew tap vookimedlo/homebrew-vookiimageviewer
brew cask install vookiimageviewer-macos
```

-----------------

## Builds
All binaries could be built easily. For your convenience, travis-ci is used to continuously check if current source code is buildable on Linux and MacOS.

And the result is: 
 - Linux and MacOS: [![Build Status](https://travis-ci.org/vookimedlo/vooki-image-viewer.svg?branch=master)](https://travis-ci.org/vookimedlo/vooki-image-viewer)
 - Windows: [![Build status](https://ci.appveyor.com/api/projects/status/a0ots8hy6d8lutdv/branch/master?svg=true)](https://ci.appveyor.com/project/vookimedlo/vooki-image-viewer/branch/master)
 
-----------------

Homepage: [https://vookiimageviewer.cz/][4]

[1]: https://en.wikipedia.org/wiki/Demosaicing
[2]: ./LICENSE
[3]: https://github.com/vookimedlo/vooki-image-viewer/
[4]: https://vookiimageviewer.cz/
[5]: https://github.com/vookimedlo/vooki-image-viewer/releases/latest


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fvookimedlo%2Fvooki-image-viewer.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fvookimedlo%2Fvooki-image-viewer?ref=badge_large)