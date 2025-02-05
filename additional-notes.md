## 9. Additional Notes

When it comes to VR performance, the most important thing is having a consistent framerate. You want to utilize your GPU as much as possible by increasing the headsets resolution or graphical settings, but also leaving enough headroom to avoid any fluctuation in framerate. You can use things like Render Stats app in-game, SteamVR performance graph, OpenXR advanced overlay or programs like GPU-Z to monitor GPU and CPU usage and adjust settings as needed.  

There is another guide written by CSOCSO which has some more in depth details for Virtual Desktop and Pimax users. You can [find it here](https://docs.google.com/document/d/1q-taJt5q9oKWPuCB63rbAC6ZzlZMxqjworgpc10ETDE/edit?tab=t.0).  

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


?> On some systems using HAGS (Hardware accelerated GPU Scheduling) can cause performance issues, you can change it in Windows Settings > System > Display > Graphics settings or just search for "GPU" in the start search.  

Reshade is available for VR too but it can also significantly impact performance so generally would not recommend using it.  
