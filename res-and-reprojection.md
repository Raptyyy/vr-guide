# Resolution and Reprojection

### Resolution
Unlike monitors, VR headsets dont have a "native" resolution because of [barrel distortion](https://github.com/user-attachments/assets/cc384ebe-96b5-4272-a26b-cf7a3eb14afe) which reduces detail in the center part of the image, to counteract that we need to supersample - use a higher resolution.    
It is important to set the resolution as high as possible while also trying to avoid sacrificing performance.  
Start with 100% or 1.0x resolution (can also be called render scale) and adjust as needed based on Quality and Performance.  
On some headsets (like Pimax) 100% can already be very high resolution, you might have to lower it to get good performance.    

- **Oculus / Meta** headsets you can adjust it in the Oculus app (Settings > Graphics Preference > Render Resolution) Or in the [Oculus Debug Tool](https://smartglasseshub.com/oculus-debug-tool/) with the Pixels Per Display Pixel Override setting.  
- **Steam VR** headsets you can adjust it in SteamVR settings (Video > Resolution Per Eye).  
- **Windows Mixed Reality** headsets you can adjust it in OpenXR Tools for Windows Mixed Reality (Custom Render Scale).  
- **Pimax** headsets you can adjust it in the Pimax Play software (Render Quality).  

?> The Resolution in Content Manager <ins>Settings > Assetto Corsa > Video</ins> does NOT affect VR resolution.  

### Reprojection
Reprojection reduces system load by halving the amount of rendered frames and extrapolating the rest to maintain a smooth experience, very similarly to frame generation.    
For example - Using a 90Hz headset, your PC would need to render only 45 fps, the rest being generated by reprojection.    
However, it may cause artifacts, input delay, or stuttering (if it's switching between reprojection on or off). 
- **Oculus / Meta** you can set it in the [Oculus Debug Tool](https://smartglasseshub.com/oculus-debug-tool/) with the PC Asynchronous Spacewarp setting. (Debug tool can sometimes not honor the setting and ignore it).  
Alternative method: Download [this archive](https://github.com/Raptyyy/rapty_ac_vr_guide/raw/refs/heads/main/resources/oculus%20asw%20enable%20disable%20registry.zip)  
Run "oculus disable asw.reg" to disable ASW, or "oculus enable asw.reg" to enable it.
- **Steam VR** you can set it in SteamVR settings (Video > Motion Smoothing).  
- **Windows Mixed Reality** you can set it in OpenXR Tools for Windows Mixed Reality (Motion Reprojection Rate).  
- **Pimax** you can set it in the Pimax Play software (Smart Smoothing).  

Any headset using OpenComposite and the OpenXR Toolkit can also adjust Resolution and Reprojection through the OpenXR Toolkit.  