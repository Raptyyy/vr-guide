# 7.1 OpenComposite
Allows you to play SteamVR games without actually needing SteamVR, it is highly recommended for users wanting more performance.  
On non native SteamVR headsets (Quest, Pimax, WMR) SteamVR simply acts as a middle layer which increases resource usage while bringing no real benefit to your VR experience.  
OpenComposite can also be used with Virtual Desktop when using it with VDXR, [more info here](https://github.com/mbucchia/VirtualDesktop-OpenXR/wiki)  

?> Using OpenComposite with native SteamVR headsets (Vide, Index, Beyond) wont allow you to bypass SteamVR as it is required no matter what. However it would give you access to the OpenXR Toolkit if needed.  


?> Pico standalone headsets dont have their own OpenXR runtime, so to bypass SteamVR you would need to use Virtual Desktop with VDXR and OpenComposite.

### To install OpenComposite:
1. Download the OpenComposite dll from one of the links  
  1.1. From [this repository](https://github.com/Raptyyy/rapty_ac_vr_guide/raw/refs/heads/main/resources/openvr_api.dll)  
  1.2. From the [OpenComposite mirror](https://opencomposite.znix.xyz/builds/) (Select the first result and download the Platform: x64	x64/openvr_api.dll file)  
2. Make sure the file is called "openvr_api.dll" (rename it if needed)
3. Place the file to <ins>"steamapps\common\assettocorsa\system\x64"</ins>, overwrite files if prompted to.
4. In <ins>Content Manager > Settings > Video</ins> set "Rendering Mode" to "OpenVR"
5. You also need to make sure your headset is using its native OpenXR Runtime (or VDXR for Virtual Desktop) and not the SteamVR one  


?> **IMPORTANT** If you encounter any issues using OpenComposite, I have the [original dll file uploaded here](https://github.com/Raptyyy/rapty_ac_vr_guide/raw/refs/heads/main/resources/openvr_api.dll.og), rename it to "openvr_api.dll", put it in the same location as the opencomposite dll and overwrite, this will remove opencomposite.  

# 7.2 OpenXR Toolkit
OpenComposite also lets you use the OpenXR Toolkit which brings [additional functionality and tweaks](https://mbucchia.github.io/OpenXR-Toolkit/features.html).  
The toolkit allows you to use things like Upscaling (NIS,FSR,CAS), Foveated rendering and more.  
The toolkit [can be downloaded here](https://mbucchia.github.io/OpenXR-Toolkit/#downloads)  
If you have OpenComposite set up correctly and the Toolkit installed, it should pop up by itself in game. I would recommend changing the default hotkeys from F keys to arrow keys for convenience in the OpenXR Toolkit Companion app in windows.   
<img src="https://github.com/user-attachments/assets/6b1f4817-cae9-4907-a9fa-5c9aff2a0b05" width="300">  


### Recommended settings for the Toolkit:
Set these settings in game through the toolkit menu (CTRL + F2 by default to open or whatever hotkey you change it to).  
- Upscaling set to `FSR` if you need more performance or set to `CAS` to improve image quality by sharpening the image, strength of `80% to 100%` should work best.
- Foveated rendering set to `Preset - Quality - Balanced`, this will be a good starting point, adjust as needed. `Custom` will allow you to tweak things further.  
- System > FOV allows you to change the size of the FOV (Field of View). This has the benefit of increasing image quality at the expense of reduced FOV, I personally use `94%` on my Revern G2 V1. Might not work well with every headset.  
