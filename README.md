# sd-webui-stealth-pnginfo

This extension embeds image generation metadata into the (unused) alpha channel of a PNG generated in [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui). 
Works in [Forge Neo](https://github.com/Haoming02/sd-webui-forge-classic)!

**Will not work for JPEG images.** Ignores webp too.

***Please note that as the "stealth" copy of the data is embedded in the image pixels, it is not visible in an EXIF data viewer.***

It will show up in the PNG info tab in the webui and via bots like [Prompt Inspector](https://github.com/sALTaccount/PromptInspectorBot), but not via EXIF tools.

Extension auto-activates and runs alongside standard webui PNG info functions, embedding and reading both the typical EXIF info and the resilient signature, no extra settings are required. It can optionally be disabled in settings if desired.

### Acknowledgements

Forked from [@neggles's fork](https://github.com/neggles/sd-webui-stealth-pnginfo) of [@ashen-sensored/sd_webui_stealth_pnginfo](https://github.com/ashen-sensored/sd_webui_stealth_pnginfo) - this was originally created to get around Discord stripping the text sections from PNGs, but they've reversed that change so Ashen is not maintaining that anymore. I find it convenient though (since it doesn't rely on that data being retained, and many websites/devices will strip it) so here it is. Forge Neo changed the infotext hook to infotext_utils.py, warranting an update.
