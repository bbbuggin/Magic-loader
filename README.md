# Magic Loader

A small iPad-friendly web app for organizing Minecraft Bedrock resource-pack files and handing them to Minecraft using the iOS share sheet.

## Run it
- Open `index.html` in a browser for a basic local preview.
- For installable PWA behavior, host this folder on an HTTPS static host.
- On iPad Safari, open the hosted site, use Share > Add to Home Screen.

## Import workflow
1. Tap Import a pack.
2. Choose a `.mcpack` or `.mcaddon` from Files.
3. Tap Share to Minecraft if Minecraft appears in the iOS share sheet.
4. In Minecraft, wait for import to finish.
5. Activate the pack in the world's Resource Packs settings.

## Limitations
- This is a pack manager, not an injected in-game overlay.
- iPadOS app sandboxing prevents this website from injecting a GUI into Minecraft or directly changing Minecraft's private files.
- The app saves pack metadata in browser local storage. The actual selected file is handed to iPadOS sharing and is not uploaded.
- A `.mcpack` import does not guarantee shader effects. Use packs built for your exact Bedrock version and supported rendering pipeline. Traditional third-party shader support is limited; Vibrant Visuals and compatible PBR/deferred packs are a separate path.
- Java Edition shader packs are not compatible with Bedrock.

## Privacy
No analytics, accounts, external requests, or file uploads are included.


## Preloaded shader catalog
The Shaders tab includes links to creator-hosted pages for:
- Enhanced Vibrant Visuals (CurseForge)
- ARCE Visuals (CurseForge)
- Ultra Vibrant Visuals (MCPEDL)
- Realistic Debo Shader (MCPEDL)
- Nexora Shader (MCPEDL)

The project intentionally does not redistribute those creators' `.mcpack` files. Use the creator pages for the latest versions and license terms.
