# Additional Notes

?> There is another guide written by CSOCSO which has some more in depth details for Virtual Desktop and Pimax users. You can [find it here](https://docs.google.com/document/d/1q-taJt5q9oKWPuCB63rbAC6ZzlZMxqjworgpc10ETDE/edit?tab=t.0).  

### Performance
When it comes to VR performance, the most important thing is having a consistent framerate. You want to utilize your GPU as much as possible by increasing the headsets resolution or graphical settings, but also leaving enough headroom to avoid any fluctuation in framerate. You can use things like Render Stats app in-game, SteamVR performance graph, OpenXR Toolkit advanced overlay or programs like GPU-Z to monitor GPU and CPU usage and adjust settings as needed.  

On some systems using HAGS (Hardware accelerated GPU Scheduling) can potentially cause performance issues (Especially on windows 10 or if you are using OBS), you can change it in Windows Settings > System > Display > Graphics settings or just search for "GPU" in the start search, requires a system restart to apply.  

### Headset adjustments
If your headset has built in `IPD (inter-pupillary distance)` adjustment it is important to set it correctly to have the best image quality and correct world scale, there are various ways to figure out what your IPD is, read more [here](https://www.vive.com/us/support/vive-xr/category_howto/how-can-i-find-my-ipd.html). Most people should be in the 60mm to 70mm range.  

If you are far or near sighted and wear glasses or contact lenses, the same thing will apply to you in VR so you will also need to wear glasses or contact lenses while you're using VR.  

Field of view is an important aspect in VR as it can greatly impact the immersiveness of your experience. Basically the closer your eyes are to the lenses the higher your Field of View will be (up to the limitations of the actual headset). Users wearing glasses will usually have to sacrifice some Field of View for comfort.  

### Nvidia Control Panel tweaks
<details>
  <summary>Anisotropic Filtering</summary>
  
Setting Anisotropic Filtering in the Nvidia Control Panel can potentially improve texture quality. Set it as shown in the image below.    
<img src="https://github.com/user-attachments/assets/58802765-659f-497d-81f7-e9fd0489795f" width="600">  
</details>

<details>
  <summary>MFAA (Multi-Frame Anti-Aliasing)</summary>


[MFAA](https://www.nvidia.com/en-us/geforce/news/multi-frame-sampled-anti-aliasing-delivers-better-performance-and-superior-image-quality/) is an anti-aliasing technique which by alternating AA sample patterns both temporally and spatially can improve the quality of MSAA.  
4xMFAA (2xMSAA + MFAA) has the performance cost of 2xMSAA, with anti-aliasing properties equivalent to 4xMSAA.  
Requires MSAA to bet set to atleast 2x in <ins>Content Manager > Settings > MSAA</ins>  
<img src="https://github.com/user-attachments/assets/ea28aeec-ca77-4f4c-b614-32174566e79c" width="600"> 
</details>

### Miscellaneous tweaks
Using overlays (like Discord, Steam, Nvidia overlays) can potentially affect VR performance in a negative way, it is recommended to disable them when using VR.

Having hardware acceleration enabled in various programs (like Steam, Discord, Spotify) can potentially affect VR performance in a negative way and also use additional VRAM, it can be worthwhile to disable hardware acceleration for such programs.
