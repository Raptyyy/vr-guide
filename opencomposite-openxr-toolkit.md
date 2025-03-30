## 8. OpenComposite and OpenXR Toolkit

# 8.1 OpenComposite
Translates OpenVR games to OpenXR which means SteamVR isnt needed to run the game (Except for SteamVR headsets), it is highly recommended for users wanting more performance.  
On some headsets like Rift, Quest, Pimax or WMR - SteamVR simply acts as a middle layer which increases resource usage while bringing no real benefit to your VR experience.  
OpenComposite can also be used with Virtual Desktop when using it with VDXR, [more info here](https://github.com/mbucchia/VirtualDesktop-OpenXR/wiki)  

?> Using OpenComposite with native SteamVR headsets (Vive, Index, Beyond) wont allow you to bypass SteamVR as it is required for the headset to function. However it would give you access to the OpenXR Toolkit if needed.  


?> Pico standalone headsets dont have their own OpenXR runtime, so to bypass SteamVR you would need to use Virtual Desktop with VDXR and OpenComposite.

### To install OpenComposite:
1. Download the OpenComposite dll from one of the links    
   A. From [this repository](https://github.com/Raptyyy/rapty_ac_vr_guide/raw/refs/heads/main/resources/openvr_api.dll)  
   B. From the [OpenComposite mirror](https://znix.xyz/OpenComposite/download.php?arch=x64&branch=openxr)  
2. Make sure the file is called "openvr_api.dll" (rename it if needed)
3. Place the file to <ins>"steamapps\common\assettocorsa\system\x64"</ins>, overwrite files if prompted to.
4. In <ins>Content Manager > Settings > Video</ins> set "Rendering Mode" to "OpenVR"
5. You also need to make sure your headset is using its native OpenXR Runtime (or VDXR for Virtual Desktop) and not the SteamVR one  


?> **IMPORTANT** If you encounter any issues using OpenComposite, I have the [original dll file uploaded here](https://github.com/Raptyyy/rapty_ac_vr_guide/raw/refs/heads/main/resources/openvr_api.dll.og), rename it to "openvr_api.dll", put it in the same location as the opencomposite dll and overwrite, this will remove opencomposite.  

# 8.2 OpenXR Toolkit
OpenComposite also lets you use the OpenXR Toolkit which brings additional features like upscaling, foveated rendering, world scale or field of view adjustability and more. [Read more about it here](https://mbucchia.github.io/OpenXR-Toolkit/features.html)  
Download the OpenXR Toolkit here [download link](https://mbucchia.github.io/OpenXR-Toolkit/#downloads)  
By default you use Ctrl + F1 to F4 to navigate the on screen menu, can be changed in the OpenXR Toolkit Companion App. [Explained further here](https://mbucchia.github.io/OpenXR-Toolkit/#basic-usage)


### Recommended settings for the Toolkit: 
- Upscaling set to `FSR` if you need more performance or set to `CAS` to improve image quality by sharpening the image. For FSR the lower the scale the more performance you will gain. For CAS use 70% to 100% strength.
- Foveated rendering set to `Preset - Quality - Balanced`, this will be a good starting point, adjust as needed. `Custom` will allow you to tweak things further.  
- Tweaking the `World Scale` in the Appearance tab could fix any issues regarding objects looking too big or too small.  
- For users wearing glasses you might be able to lower the `Field of View (FOV)` which can increase the image quality without any performance loss.  
