# Dark space - The best dynamic theme - Adapted by Yass1G1 (Static)

Switching from Firefox to Brave made me recreate this theme (without its dynamic background image :( )

## How to install it ?
1. Go in the extensions setting (or type `chrome://extensions` or `brave://extensions` in search field)
2. Turn on Developer Mode (*top left*) to allow drag & drop .crx files 
--> If you don't want to pack the extension by yourself, skip to step 4
3. Click on "Pack extension" (*top left*) and select `Dark-Space-Theme/` directory to create a .crx file (chrome extension format)
4. Drag and drop the .crx file into the extension settings window (refresh if it doesn't work directly)
5. A popup should appear warning you that this isn't official brave content (approve or not, i'm not reponsible=)
6. Enjoy !

## Yass, why it isn't dynamic ?
After searching and reviewing Chromium's UI components source code, and with the help of ChatGPT for code understanding (i'm not a C++ folk 🤡), it seems that the decoding of the custom image is made on a "single-frame" basis by this line : 

`476: SkBitmap bitmap = gfx::PNGCodec::Decode(*raw_data);`

[Link to file](https://source.chromium.org/chromium/chromium/src/+/main:chrome/browser/themes/browser_theme_pack.cc)

Which make every animated image decoded based on their first frame (converted to a [bitmap](https://en.wikipedia.org/wiki/Bitmap)) (*correct me if i'm wrong*)

(+ other part of the code that load only one time the bitmap which cannot create this dynamic effect)

__Don't hesitate to correct me if I did something wrong !__


Original repo : [Link to file](https://github.com/nicoth-in/Dark-Space-Theme)]
---
<https://addons.mozilla.org/addon/nicothin-space/> — Most popular and Highest rated Firefox Theme 🎉

![preview](https://addons.mozilla.org/user-media/version-previews/full/3827/3827732.svg)

 
