# Custom Shaders Patch settings
I will not cover every setting in CSP (that would be a lot to cover), but only the ones that matter for VR performance.  

# General Patch Settings
**Audio > Decompress Samples** recommended to have it `enabled`. Reduces CPU overhead for higher memory (RAM) usage.  

**New KN5 loader** recommended to have it `enabled`, reduces RAM and VRAM usage.  

CPU optimizations:
- **Flatten nodes** keep it `enabled`  
- **Chunks optimization** helps with CPU load. Set it to `Advanced` unless you have issues (like the screen going black), then keep it at `Basic`.  
- **Limit audio for other cars** set it to `Always` if you have a slower PC.
- **Apply Hyperthreading fix** highly recommended to have it `enabled`, benefits any CPU that uses Hyperthreading or SMT. Might not work well on 4 or 2 core CPUs. (Requires CSP version 0.2.7 / 0.2.8 preview or newer) 

GPU optimizations: 
- **Optimize meshes some more** helps with GPU load, have it `enabled`  
- "**Deduplicate meshes**" helps with VRAM, have it `enabled`  
- "**Upgrade AC textures**" can improve loading times and reduce VRAM usage, recommended to have it `enabled`. Will make the game folder size bigger (shouldnt be more than 5GB for most users).  
- "**Deduplicate textures**" can potentially lower how much VRAM the game uses but can also cause graphical issues or game crashes, use with caution. For most users I recommend keeping this `disabled`

# Extra FX
Extra FX doesnt work in VR so this will have no effect, keep it `disabled` if you don't ever use Extra FX.  

# GUI
**New driver tags** recommended to have it `enabled` so you can see driver names in VR. Its not a performance tweak but a very useful thing to have.  
**Font Scale** Set this to `125%` or higher if you struggle reading the names.  

# Graphics Adjustments
**AMD FidelityFX SuperResolution** also known as "FSR" is an upscaler that can help with performance by rendering the game at a lower resolution and then upscaling the image. Should only be needed for lower end PCs. Can also be used through the OpenXR Toolkit.

LOD settings:
- **Force low-res drivers for other cars in first person view** have it `enabled` for performance
- **Multiplier for car LODs** this sets how far away the car LOD (level of detail) will change, lower multiplier will help with performance but can make cars look worse up close, for performance set it to `75%`.
- **Multiplier for track LODs** same thing as car LODs but for the track, I would recommend not going below `80%` as it can cause issues.
- **Multiplier for trees LODs** same thing as car LODs but for 3D trees, you can set it to `0% for best performance` if you don't care about 3D trees (makes them 2D instead), otherwise keep it around `100%`.  
- **Add extra collider-based LODs for distant cars** will make low quality LODs for cars that don't have them, can help a lot in dense lobbies like VDC, recommended to have it `enabled`. Set the "Limit LODless cars" to a low value between 5 to 10 for best performance.

**Post processing antialiasing** set to `disabled` as post process AA doesnt work in VR (Will update this if it changes)  

**Accessible color buffer > Full resolution for better quality** set to `disabled` for a tiny boost in performance  

**Draw grooves over track, but before dynamic entities** Can help with performance but can also cause issues on some tracks (Like mirror / see through roads), use with caution.  

# Lighting FX
**Cars casting lights** set this to a lower amount like `5` for better performance in dense lobbies, lights are expensive performance wise.

**Disable mirroring in first person view** helps with performance a bit, have it `enabled`  

**Enable lighting in reflections** `disabled` for a performance boost  

# Neck FX
Not related to performance but there are good NeckFX scripts for VR to enhance immersion or comfort, here are two most popular ones: 
- [AC Head Physics](https://www.overtake.gg/downloads/ac-head-physics.68266) fancier script, has more movement  
- [NeckFX LUA script](https://www.overtake.gg/downloads/neckfx-lua-script-vr-stabilize.65087) more basic, static script.

# Smart Mirror
**Custom render distance** `enabled` and set the distance to 400 meters if you use High Quality mirrors in video settings, helps with performance.

**Real mirrors** highly recommended in VR, makes the mirrors change perspective based on your head movement also lets you adjust mirror positioning through the "Car Mirrors" app in-game (Install it from the "App Shelf" app in-game first)  
- **Active** `enabled`
- **Alter FOV** This will change the Field of View of the mirror depending how close you are to it. Set based on your preference, I have it `disabled`
- **Refresh rate per frame** set to `Update single reflection per frame` for best performance, can look a little laggy on lower refresh rate headsets, use higher if needed.

# Weather FX
**Weather style** this should be set to either `Pure Gamma` or `Pure LCS`. `Pure Gamma` is the recommended option as of now and has better performance, `Pure LCS` is able to produce a better looking image but could cause some issues too.  

**Replace YEBIS with lightweight alternative** is a more basic post-processing implementation which uses less CPU and GPU resources, for performance I would recommend to `enable` it. Does not work with some pp filters like C13, can also cause excessive glare.  

**Automatically guess white reference point** This can make the UI very bright when using Pure, `disable` it.  

# Mode Tweaks VR:
Make sure the extension is enabled (Active)  

**Single Pass Stereo** Highly recommended to have it `enabled`, especially on slower CPUs. It renders both eye images at the same time into one packed Render Texture, meaning that the whole Scene is only rendered once, and CPU processing time is significantly reduced. Can make some Pure shaders not work.  

**Single YEBIS pass** Have it `enabled` for best performance if needed. Instead of running post-processing individually for each eye, runs it once for both eyes. Can potentially affect glare effects in an undesirable way.  

## Nvidia VRS
also known as Foveated rendering ([What is Foveated Rendering](/foveated-rendering)), only works for Nvidia GPUs.  
If you want to use Nvidia VRS (Requires Single Pass Stereo to be enabled):  
- **Nvidia VRS** `enabled`
- **VRS preset** `Custom`
- **VRS rate** `High performance`, can set to Highest performance if you need every bit of performance but it will be more visible.
- **VRS detailed area** `Balanced`, set it to `Wide` if you use a Quest 3 or Pico 4 as they will show foveated rendering more clearly.

You can also test using the VRS presets if those work better for you.  

?> You can use the VR Tweaks app that lets you adjust all these settings (and more) in-game which you can find here: [VR Tweaks](https://www.overtake.gg/downloads/vr-tweaks.76283/)

**Corners masking optimization** Recommended to keep this one `enabled`. Also known as Hidden Area Mesh, it allows your GPU to not waste time rendering parts of the image that you wouldnt be able to see because of how the lenses work. Disable this if the black shape in the VR mirror (game window) is undesired.    

**Custom VR HUD rendering** This is not a performance related setting but its recommended to keep this `enabled` as it makes the HUD work better in VR. To adjust the HUD settings I'd recommend to use the VR tweaks app mentioned above.    
