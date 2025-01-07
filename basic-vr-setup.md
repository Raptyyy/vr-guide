## Basic VR setup

> Click on your brand of headset to expand the instructions, you only need to use one of the provided methods.

<details>
  <summary style="cursor: pointer"><b>Oculus / Meta</b></summary>

### A. Native Oculus implementation (easiest method):  
1. First make sure that you have successfully set up Quest link or Air link and that the headset is connected to your PC - [Tutorial how to do so](https://www.meta.com/help/quest/articles/headsets-and-accessories/oculus-link/connect-with-air-link/)  
  1.1. If youre using an Oculus Rift (S) then you simply need to have the headset connected and showing in the oculus app.  
2. In the Oculus App, <ins>Settings > General</ins> enable "Unknown sources" and next to the "OpenXR Runtime" press "Set Oculus as active" (If its greyed out then you don't need to press it)  
3. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and set "Rendering Mode" to "Oculus Rift", this does not require SteamVR.  

### B. Using Virtual Desktop and OpenComposite (Can give better results however costs money):
1. Purchase Virtual Desktop on the Oculus / Meta store (do not buy it on steam itself)
2. Follow the instructions provided in Virtual Desktop to connect your headset to your PC (Quest / Air Link is not required).   
3. Open the Virtual Desktop Streamer application, and under settings, select VirtualDesktopXR (VDXR) as the OpenXR runtime.
4. Set up OpenComposite, [instructions here](#to-install-opencomposite)
5. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and set "Rendering Mode" to "OpenVR"  

Using this method you can also look into the [OpenXR Toolkit](#openxr-toolkit)

### C. Using SteamVR (Generally not recommended):
1. First make sure that you have successfully set up Quest link or Air link and that the headset is connected to your PC - [Tutorial how to do so](https://www.meta.com/help/quest/articles/headsets-and-accessories/oculus-link/connect-with-air-link/)
  1.1. If youre using an Oculus Rift (S) then you simply need to have the headset connected and showing in the oculus app.  
3. Install and set up SteamVR from Steam  
4. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and set "Rendering Mode" to "OpenVR"

#### Oculus / Meta additional notes and troubleshooting  

- Game lagging when using the headset wirelessly: Your router might not be able to handle the high amount of bandwidth required for a smooth experience, this will generally show as high network latency. Try to lower the bitrate in the [Oculus Debug Tool](https://smartglasseshub.com/oculus-debug-tool/) or set it to 0 for auto bitrate.  
- USB-C, Make sure your headset runs USB 3 and not USB 2, if it keeps connecting via USB 2 even with a new cable and using a USB 3 port, reset your headset to factory defaults which will fix the issue.
- using USB-C set the bitrate to 500mbps or higher in the Oculus Debug Tool. More info about the [Oculus Debug Tool here](https://smartglasseshub.com/oculus-debug-tool/).  

</details>
<br>

<details>
  <summary style="cursor: pointer"><b>SteamVR headsets (Vive, Index, Bigscreen beyond)</b></summary>



### A. Using SteamVR:  
1. Make sure your headset is connected to your PC
2. Install and set up SteamVR from Steam  
3. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"
</details>
<br>

<details>
  <summary style="cursor: pointer"><b>Windows Mixed Reality headsets</b></summary>
  


### A. Using OpenComposite (Highly recommended): 
1. Make sure your headset is connected to your PC  
2. Install and set up Windows Mixed Reality from the Microsoft Store
3. Install and set up OpenXR Tools for Windows Mixed Reality from the Microsoft Store  
  3.1. If you see a button that says "Set as active runtime" - press it.  
5. Set up OpenComposite, [instructions here](#to-install-opencomposite)  
6. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"  

Using this method you can also look into the [OpenXR Toolkit](#openxr-toolkit)

### B. Using SteamVR:
1. Make sure your headset is connected to your PC  
2. Install and set up Windows Mixed Reality from the Microsoft Store  
3. Install and set up SteamVR from Steam  
4. Install Windows Mixed Reality for SteamVR from Steam  
5. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"  
</details>
<br>

<details>
  <summary style="cursor: pointer"><b>Pimax headsets</b></summary>

### A. Using OpenComposite (Highly recommended): 
1. Make sure your headset is connected to your PC  
2. Install and set up Pimax Play, [link here](https://pimax.com/pages/downloads-manuals)  
3. Set the OpenXR Runtime to Pimax OpenXR in Pimax Play, [instructions here](https://pimax.com/blogs/blogs/how-to-use-pimax-openxr)  
5. Set up OpenComposite, [instructions here](#to-install-opencomposite)  
6. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"  

Using this method you can also look into the [OpenXR Toolkit](#openxr-toolkit)

### B. Using SteamVR:
1. Make sure your headset is connected to your PC
2. Install and set up Pimax Play, [Link here](https://pimax.com/pages/downloads-manuals)
3. Install and set up SteamVR from Steam  
4. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"
</details>

> Once you have the correct settings applied for your headset, test it out in singleplayer first before joining a server !
