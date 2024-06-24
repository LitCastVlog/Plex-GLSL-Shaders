# Plex GLSL Shaders (Video Filters)
GLSL Shader pack for Plex HTPC/Plex Media Player
# Installation:
just copy the `Shaders` folder and `input.conf` to `%LOCALAPPDATA%\Plex HTPC\shaders` or `%LOCALAPPDATA%\Plex\shaders` (Windows)

(for MacOS: `/Library/Application Support/Plex/shaders` or `/Library/Application Support/Plex HTPC/shaders`)

![CRT Filter](http://images2.imgbox.com/6a/eb/rjMKMTAk_o.jpg)
![Animation Filter](https://i.ibb.co/r5QWtLM/ffdsffds.jpg)
![Make My GPU Hurt 2](https://images2.imgbox.com/9d/cf/MGP63ldy_o.png)
 # Usage:

 Shader Hotkeys are:

 CTRL + 0 : Clear all shaders

 ALT + 0 : Animation/Cartoon Upscale (Anime4k+Enhanced FSRCNNX) (Upscale/Sharpen/Denoise)

 CTRL + 1-6 : Anime4k 
 
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
 if you want to enable a shader by default when you open Plex, create an `mpv.conf` in the same directory as `input.conf`
 and edit it like so:
```
#enable shader(s) on startup (SSimSuperRes-mitchell)
glsl-shaders="~~/shaders/SSimSuperRes-mitchell.glsl"
```
replace the shaders with the ones you wish to use 

optionally, use a semicolon `;` to load multiple filters at once:
```
#enable shader(s) on startup (Filmgrain + SSimSuperRes-mitchell)
glsl-shaders="~~/shaders/filmgrain-lighter.glsl;~~/shaders/SSimSuperRes-mitchell.glsl"
```
