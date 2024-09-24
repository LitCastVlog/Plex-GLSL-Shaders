# Plex GLSL Shaders (Video Filters)
GLSL Shader pack for Plex HTPC/Plex Media Player/MPV (Realtime Upscaling, CRT, FilmGrain)
# Installation:
just copy the `Shaders` folder and `input.conf` to `%LOCALAPPDATA%\Plex HTPC\shaders` or `%LOCALAPPDATA%\Plex\shaders` (Windows)

(for MacOS: `/Library/Application Support/Plex/shaders` or `/Library/Application Support/Plex HTPC/shaders`)

![CRT Filter](http://images2.imgbox.com/6a/eb/rjMKMTAk_o.jpg)
![Animation Filter](https://i.ibb.co/r5QWtLM/ffdsffds.jpg)
![Animation Filter](https://i.ibb.co/181PScy/gfdgfd.jpg)
![Make My GPU Hurt 2](https://github.com/LitCastVlog/Plex-GLSL-Shaders/blob/main/Screenshot_4k.png)
 # Usage:

 Shader Hotkeys are:

 CTRL + 0 : Clear all shaders

 ALT + 0 : Animation/Cartoon Upscale (Anime4k Restore+Enhanced FSRCNNX) (Upscale/Sharpen/Denoise)

 CTRL + 1-6 : [Anime4K](https://github.com/bloc97/Anime4K) shaders by bloc97 
 
 CTRL + 7 : FilmGrain
 
 CTRL + 8 : Filmgrain (Light) + SSimSuperRes-Mitchell (Upscale/sharpener)
 
 CTRL + 9 : Filmgrain + SSimSuperRes-Mitchell (Upscale/sharpener)
 
 CTRL + - : CRT Simulator (Brighter)
 
 CTRL + = : CRT Simulator (+Filmgrain)
 
 ALT + 1-4 : CRT alternative modes (crt-lottes shadow mask setting)
 
 ALT + 5 : Make My GPU Hurt (FSRCNNX+KrigBilateral)
 
 ALT + 6 : Make My GPU Hurt Ultra (FSRCNNX+SSimSuperRes-mitchell+KrigBilateral)
 
 ALT + 7 : FilmGrain (Lighter) + SSimSuperRes-Mitchell (Upscale/sharpener)
 
 ALT + 8 : Filmgrain (Medium) + SSimSuperRes-Mitchell (Upscale/sharpener)
 
 ALT + 9 : Filmgrain (Heavy) + SSimSuperRes-Mitchell (Upscale/sharpener)
 

 # Load on startup
 to enable a shader by default when you open Plex, create an `mpv.conf` in the same directory as `input.conf`
 and edit it like so:
```
#enable shader(s) on startup (SSimSuperRes-mitchell)
glsl-shaders="~~/shaders/SSimSuperRes-mitchell.glsl"
```
optionally, use a semicolon `;` to load multiple shaders:
```
#enable shader(s) on startup (Filmgrain + SSimSuperRes-mitchell)
glsl-shaders="~~/shaders/filmgrain-lighter.glsl;~~/shaders/SSimSuperRes-mitchell.glsl"
```
