# sd-webui-stealth-pnginfo

This extension embeds image generation metadata into the (unused) alpha channel of a PNG generated in [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui). 

**Will not work for JPEG images.** Untested on webp, should work in theory but who knows.

***Please note that as this data is embedded in the image pixels, it is not visible in an EXIF data viewer.***

It will show up in the PNG info tab in the webui and via bots like [Prompt Inspector](https://github.com/sALTaccount/PromptInspectorBot), but not via EXIF tools.

Extension auto-activates and runs alongside standard webui PNG info functions, no extra settings are required. It can optionally be disabled in settings if desired.

### Acknowledgements

Forked from [@ashen-sensored/sd_webui_stealth_pnginfo](https://github.com/ashen-sensored/sd_webui_stealth_pnginfo) - this was originally created to get around Discord stripping the text sections from PNGs, but they've reversed that change so Ashen is not maintaining that anymore. I find it convenient though (since it doesn't rely on that data being retained, and many websites/devices will strip it) so here it is.
