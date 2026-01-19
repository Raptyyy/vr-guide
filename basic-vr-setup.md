# Headset setup

?> Click on your brand of headset to expand the instructions, use whichever method works best if there's multiple.

<details>
  <summary style="cursor: pointer"><b>Oculus / Meta</b></summary>

<!-- tabs:start -->

#### **Oculus (Easy setup)**
This is the easiest and for most users the best method

1. First make sure that you have successfully set up Quest link or Air link and that the headset is connected to your PC - [Tutorial how to do so](https://www.meta.com/help/quest/articles/headsets-and-accessories/oculus-link/connect-with-air-link/)  
   1.1. If youre using an Oculus Rift (S) then you simply need to have the headset connected and showing in the oculus app.  
2. In the Oculus App, <ins>Settings > General</ins> enable "Unknown sources" and next to the "OpenXR Runtime" press "Set Oculus as active" (If its greyed out then you don't need to press it)  
3. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and set "Rendering Mode" to "Oculus Rift".

**You do not need SteamVR for this**

#### **OpenComposite (Best performance)**
Should deliver a similar experience to native Oculus but will let you use the OpenXR Toolkit  
Can deliver better performance  
Intended more for advanced users

1. First make sure that you have successfully set up Quest link or Air link and that the headset is connected to your PC - [Tutorial how to do so](https://www.meta.com/help/quest/articles/headsets-and-accessories/oculus-link/connect-with-air-link/)  
   1.1. If youre using an Oculus Rift (S) then you simply need to have the headset connected and showing in the oculus app.  
2. In the Oculus App, <ins>Settings > General</ins> enable "Unknown sources" and next to the "OpenXR Runtime" press "Set Oculus as active" (If its greyed out then you don't need to press it)  
3. Set up OpenComposite, [instructions here](/opencomposite-openxr-toolkit?id=to-install-opencomposite)
4. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and set "Rendering Mode" to "OpenVR"  

Using this method you can also look into the [OpenXR Toolkit](/opencomposite-openxr-toolkit?id=openxr-toolkit)


#### **Virtual Desktop**
Virtual Desktop can potentially deliver a better experience but it is also paid.

1. Purchase Virtual Desktop on the Oculus / Meta store (do not buy it on steam itself)
2. Follow the instructions provided in Virtual Desktop to connect your headset to your PC (Quest / Air Link is not required).   
3. Open the Virtual Desktop Streamer application, and under settings, select VirtualDesktopXR (VDXR) as the OpenXR runtime.
4. Set up OpenComposite, [instructions here](/opencomposite-openxr-toolkit?id=to-install-opencomposite)
5. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and set "Rendering Mode" to "OpenVR"  


#### **SteamVR**
Generally not recommended to use

1. First make sure that you have successfully set up Quest link or Air link and that the headset is connected to your PC - [Tutorial how to do so](https://www.meta.com/help/quest/articles/headsets-and-accessories/oculus-link/connect-with-air-link/)  
   1.1. If youre using an Oculus Rift (S) then you simply need to have the headset connected and showing in the oculus app.  
3. Install and set up SteamVR from Steam  
4. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and set "Rendering Mode" to "OpenVR"

<!-- tabs:end -->

### Oculus / Meta additional notes and troubleshooting  

- Run the USB test to make sure you are using a compatible cable and a USB 3 port, you can follow [this video here](https://youtu.be/vvwCVfqBxHw?si=XHUOMkvEDwcnUTrJ&t=244) for instructions. If the USB test shows that you are not using a USB 3 connection then you will likely run into issues when using quest link.
- There are additional settings to tweak in the `Oculus Debug Tool` like bitrate, FOV tangents, ASW etc., you can learn more about it in [this video about the debug tool](https://youtu.be/ZO9A39eypbQ?si=7HLkPuwM5P-XJw8G)
- If you're using the USB cable and quest link (wired) set the encode bitrate to 500mbps or higher in the Oculus Debug Tool.  
- Game lagging when using the headset wirelessly: Your router might not be able to handle the high amount of bandwidth required for a smooth experience, this will generally show as high network latency. Try to lower the bitrate in the Oculus Debug Tool or set it to 0 for auto bitrate.  

</details>
<br>

<details>
  <summary style="cursor: pointer"><b>SteamVR headsets (Vive, Index, Bigscreen beyond)</b></summary>
 
<!-- tabs:start -->

#### **Native SteamVR**
1. Make sure your headset is connected to your PC
2. Install and set up SteamVR from Steam  
3. Some headsets might require an additional driver or utility to function correctly, follow the provided instructions for your headset.  
4. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"
<!-- tabs:end -->
</details>
<br>

<details>
  <summary style="cursor: pointer"><b>Windows Mixed Reality headsets</b></summary>

<!-- tabs:start -->

#### **Using Oasis SteamVR driver (Recommended)**
1. Make sure your headset is connected to your PC  
2. Install [Oasis Driver for Windows Mixed Reality](https://store.steampowered.com/app/3824490/Oasis_Driver_for_Windows_Mixed_Reality/)   
3. Follow [Oasis instructions](https://github.com/mbucchia/Oasis-Driver-for-Windows-Mixed-Reality/wiki#hello-and-welcome-to-the-oasis-driver-for-windows-mixed-reality-documentation)   
4. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"  

### Additional notes

- While Oasis is not officially supported on Windows 10, it does work and shouldn't have any issues. I would recommend using it instead of WMR regardless.
- If you want access to the OpenXR Toolkit then you can still use OpenComposite with Oasis, although it's not neccessary.
- When using Oasis, in SteamVR video settings 150% resolution scale will be the same as 100% on WMR, that is the sweetspot in terms of quality and performance.
- If the image is not as sharp on Oasis as it was on WMR then try lowering the FOV in SteamVR Video settings per game to around 92 - 95%. You can also use vrperfkit to add some CAS sharpening, around 70% gives good results.

#### **Using OpenComposite**

1. Make sure your headset is connected to your PC  
2. Install and set up Windows Mixed Reality from the Microsoft Store
3. Install and set up OpenXR Tools for Windows Mixed Reality from the Microsoft Store  
   3.1. If you see a button that says "Set as active runtime" - press it.  
5. Set up OpenComposite, [instructions here](/opencomposite-openxr-toolkit?id=to-install-opencomposite)  
6. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"  

### Additional notes
- Using this method you can also look into the [OpenXR Toolkit](/opencomposite-openxr-toolkit?id=openxr-toolkit)

<!-- tabs:end -->

</details>
<br>

<details>
  <summary style="cursor: pointer"><b>Pimax headsets</b></summary>

<!-- tabs:start -->

#### **Using OpenComposite (Recommended)**
1. Make sure your headset is connected to your PC  
2. Install and set up Pimax Play, [link here](https://pimax.com/pages/downloads-manuals)  
3. Set the OpenXR Runtime to Pimax OpenXR in Pimax Play, [instructions here](https://pimax.com/blogs/blogs/how-to-use-pimax-openxr)  
5. Set up OpenComposite, [instructions here](/opencomposite-openxr-toolkit?id=to-install-opencomposite)
6. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"  

Using this method you can also look into the [OpenXR Toolkit](/opencomposite-openxr-toolkit?id=openxr-toolkit)

#### **Using SteamVR**
1. Make sure your headset is connected to your PC
2. Install and set up Pimax Play, [Link here](https://pimax.com/pages/downloads-manuals)
3. Install and set up SteamVR from Steam  
4. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"

<!-- tabs:end -->

<!-- ### Pimax additional notes

- Some Pimax headsets that have eye tracking support DFR (dynamic foveated rendering) on AC. This is similar to [Foveated Rendering](foveated-rendering) but the rings will follow your eye gaze which can help with performance.
<br/>Also make sure `Nvidia VRS` in CSP - Display mode - VR is disabled -->


</details>
<br/>

<details>
  <summary style="cursor: pointer"><b>PS VR2</b></summary>

<!-- tabs:start -->

#### **Using SteamVR (Recommended)**
1. Follow the instructions for setting up PSVR2 for PC here - [instructions here](https://www.playstation.com/en-us/support/hardware/pc-ps-vr2-set-up/) 
2. PSVR2 functions as a SteamVR headset, so make sure SteamVR is running and the headset is detected.
3. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"  

### Additional notes

- PSVR2 supports eye tracking and it's possible to use DFR (dynamic foveated rendering) on AC using PimaxMagic4All. This is similar to [Foveated Rendering](foveated-rendering) but the rings will follow your eye gaze which is preferable quality wise.<br/>
For that to work you need to set up the [PSVR2 Toolkit](https://github.com/BnuuySolutions/PSVR2Toolkit) and then download [PimaxMagic4All](https://github.com/mbucchia/PimaxMagic4All). PimaxMagic4All must be opened in the background for DFR to work.
<br/>Also make sure `Nvidia VRS` in CSP - Display mode - VR is disabled
<br/>This does not work with OpenComposite.

#### **Using OpenComposite**

1. Follow the instructions for setting up PSVR2 for PC here - [instructions here](https://www.playstation.com/en-us/support/hardware/pc-ps-vr2-set-up/) 
2. PSVR2 functions as a SteamVR headset, so make sure SteamVR is running and the headset is detected.
5. Set up OpenComposite, [instructions here](/opencomposite-openxr-toolkit?id=to-install-opencomposite)  
6. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"  

### Additional notes

- Using this method you can also look into the [OpenXR Toolkit](/opencomposite-openxr-toolkit?id=openxr-toolkit)


<!-- tabs:end -->

</details>
<br/>

