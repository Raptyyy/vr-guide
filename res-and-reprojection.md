# Resolution and Reprojection

### Resolution
Unlike monitors, VR headsets dont have a "native" resolution because of [barrel distortion](https://github.com/user-attachments/assets/cc384ebe-96b5-4272-a26b-cf7a3eb14afe) which reduces detail in the image.  
It is important to set the resolution high enough to have a clear image, but also not too high to avoid performance issues.  
Start with 100% or 1.0x resolution and adjust as needed based on Quality and Performance.  

- **Oculus / Meta** headsets you can adjust it in the Oculus app (Settings > Graphics Preference > Render Resolution) Or in the [Oculus Debug Tool](https://smartglasseshub.com/oculus-debug-tool/) with the Pixels Per Display Pixel Override setting.  
- **Steam VR** headsets you can adjust it in SteamVR settings (Video > Resolution Per Eye).  
- **Windows Mixed Reality** headsets you can adjust it in OpenXR Tools for Windows Mixed Reality (Custom Render Scale).  
- **Pimax** headsets you can adjust it in the Pimax Play software (Render Quality).  

?> The Resolution in Content Manager <ins>Settings > Assetto Corsa > Video</ins> does NOT affect VR image quality.  

### Reprojection
Reprojection reduces system load by halving the amount of rendered frames and [extrapolating](https://cdn.mos.cms.futurecdn.net/wwXXdLEWrPADG7yLtC48cP-970-80.png) the rest to maintain a smooth experience, very similarly to frame generation.    
For example - a 90Hz headset would need only 45fps with reprojection instead of 90fps.  
However, it may cause artifacts, input delay, or stuttering (if its switching between reprojection on or off). 

- **Oculus / Meta** headsets you can set it in the [Oculus Debug Tool](https://smartglasseshub.com/oculus-debug-tool/) with the PC Asynchronous Spacewarp setting.  
- **Steam VR** headsets you can set it in SteamVR settings (Video > Motion Smoothing).  
- **Windows Mixed Reality** headsets you can set it in OpenXR Tools for Windows Mixed Reality (Motion Reprojection Rate).  
- **Pimax** headsets you can set it in the Pimax Play software (Smart Smoothing).  

Any headset using OpenComposite and the OpenXR Toolkit can also adjust Resolution and Reprojection through the OpenXR Toolkit.  