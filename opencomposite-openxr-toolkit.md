## OpenComposite
Recommended for Rift, Quest or Pimax headsets</br>
Not needed for native SteamVR headsets (Vive, Index, PSVR2, Bigscreen, Oasis)</br>
Translates OpenVR games to OpenXR which means SteamVR isn't needed to run the game and reduces resource usage</br>
OpenComposite can also be used with Virtual Desktop when using it with VDXR, [more info here](https://github.com/mbucchia/VirtualDesktop-OpenXR/wiki)  

?> Using OpenComposite with native SteamVR headsets (Vive, Index, Beyond) wont allow you to bypass SteamVR as it is required for the headset to function. However it would give you access to the OpenXR Toolkit if needed.  


?> Pico standalone headsets dont have their own OpenXR runtime, so to bypass SteamVR you would need to use Virtual Desktop with VDXR and OpenComposite.

### To install OpenComposite:
1. Download the OpenComposite dll from one of the links    
   A. From [this repository](https://github.com/Raptyyy/rapty_ac_vr_guide/raw/refs/heads/main/resources/openvr_api.dll)  
   B. From the [OpenComposite mirror](https://znix.xyz/OpenComposite/download.php?arch=x64&branch=openxr)  
2. Navigate to <ins>"steamapps\common\assettocorsa\system\x64"</ins>
3. Rename the `openvr_api.dll` file to `openvr_api_original.dll`
4. Move or copy and paste the downloaded `openvr_api.dll` file to the directory
5. In <ins>Content Manager > Settings > Video</ins> set "Rendering Mode" to "OpenVR"
6. You also need to make sure your headset is using its native OpenXR Runtime (or VDXR for Virtual Desktop) and not the SteamVR one  


?> **IMPORTANT** If you encounter any issues using OpenComposite - simply delete the `openvr_api.dll` and rename the `openvr_api_original.dll` file back to `openvr_api.dll`

## OpenXR Toolkit
Adds additional features like upscaling, foveated rendering, world scale or field of view adjustability and [more](https://mbucchia.github.io/OpenXR-Toolkit/features.html)</br>
**Requires OpenComposite**</br>
[Download the OpenXR Toolkit here](https://mbucchia.github.io/OpenXR-Toolkit/#downloads)</br>
By default you use Ctrl + F1 to F4 to navigate the on screen menu, [can be changed in the OpenXR Toolkit Companion App](https://mbucchia.github.io/OpenXR-Toolkit/#3-launch-the-openxr-toolkit-companion-app-to-confirm-that-the-software-is-active)


### Recommended settings for the Toolkit: 
- Upscaling set to `CAS` to improve image quality by sharpening the image, use 70% to 100% strength.</br>
Set to `FSR` if you need more performance, the lower the scale the more performance you will gain while sacrificing image quality.
- Foveated rendering set to `Preset - Quality - Balanced`, this will be a good starting point, adjust as needed. `Custom` will allow you to tweak things further.
- Tweaking the `World Scale` in the Appearance tab could fix any issues regarding objects looking too big or too small.  
- For users wearing glasses you might be able to lower the `Field of View (FOV)` which can increase the image quality without any performance loss.
