# Video Settings
This covers all the settings in Content Manager > Settings > Video  

?> Note that in Content Manager > Video most settings have an ![image](https://github.com/user-attachments/assets/9f386396-4427-4b7a-b75b-127258967f94) icon next to them that will show what each setting does and the performance impact.  

# Resolution and FPS
**Rendering Mode** should already be set depending on your headset as shown above.  

**Fullscreen** will simply display the game in Fullscreen instead of a window, recommended to have it `enabled` as it slightly helps with performance but its not a must.  

**Resolution** doesnt really matter for VR use, it will only set the game window size, does not affect VR image quality.  

**Virtual synchronization** is not needed, keep it `disabled`  

**Limit framerate** is not needed in VR as the headset will limit fps as needed by itself, keep it `disabled`.  

# Quality
**MSAA** (Multisample anti-aliasing) is an Anti-Aliasing technique which helps with jagged edges, pixelation or shimmering especially into the distance. Highly recommended to keep it enabled in VR, either `2x` or `4x`. `8x` will have a major impact on performance and is generally not worth using.  

**Anisotropic Filtering** helps with texture clarity into the distance, it has a no performance impact so it's recommended to just keep it at `16x`.  

**World details** will affect object count on tracks (if they support it), set it as needed. Can also be adjust in-game using the "View & Video Settings" app.  

**Shadows resolution** affects how sharp the shadows will look. Higher resolution will make shadows look better but decrease performance. I would recommended using `1024x1024` and increase if performance isnt an issue.  

**Smoke generation** simply controls the smoke quantity, adjust as needed, but I would recommend using CSP smoke instead (Custom Shaders Patch > Particles FX > New smoke and dust)  

# Reflections
**Reflection Resolution** simply adjusts how sharp / clear the reflections will look, `512x512` is a good base value to start with, can increase if needed.  

**Rendering frequency** adjusts how frequently the reflections will update. Set it to `two faces per frame`, any higher is not really needed as they get reprojected anyway. Don't use Static either as it will cause issues with Pure.  

**Rendering distance** Adjusts the reflection rendering distance, does not have a noticeable performance impact so you can set it to `at least 1000m` or higher if needed.  

# Post-Processsing
**Enable post-processing effects** this enables post processing in general, very useful to have to improve the graphics and look of the game, however has a big performance impact. Most PCs should have it `enabled` but low-end PCs should probably `disable` it on more demanding servers.  

**Overall Quality** sets the post processing resolution, `High` is a good middle ground performance wise but can also just set it to `Maximum`.  

**Glare Quality** sets the quality of glare effects, `High` is a good middle ground performance wise but can also just set it to `Maximum`.  

**Depth of field** adjusts the depth of field quality, only works in replays so can keep it `Off` if you don't care about it.  

**Motion blur** not recommended to use with VR, set it to `Off`  

**Saturation** is basically the intensity of the colors, keep it at `100%` and adjusts colors in Pure instead if needed.  

**Heat shimmering** adds a heat shimmering effect, `set as needed`  

**Sunrays** enables sun rays / god rays / sun shafts, `set as needed`  

**FXAA** is an anti aliasing technique, keep it `enabled` as it is required for some CSP functionality but will not affect image quality in VR.

# Mirrors
**Mirror resolution** how sharp / clear the mirrors will look, higher resolutions will reduce performance, `256x1024` is a good base value  

**High quality** enables additional effects in the mirrors and increases the rendering distance (from 400 to 800 meters), will reduce performance, recommended to `enable`.    

# Oculus (only affects Oculus / Meta headsets)
**Pixels per display** is same as resolution multiplier in the oculus app or oculus pixels per display pixel override in oculus debug app, `set as needed`  

**Mirror texture** enables the game window to show your VR view, recommended to have it `enabled`  

# System
I would recommend not messing with these settings as they don't really have any meaningful impact and can cause issues.
