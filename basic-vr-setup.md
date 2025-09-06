# Basic VR setup

?> Click on your brand of headset to expand the instructions, you only need to use one of the provided methods.

?> Once you have the correct settings applied for your headset, test it out in singleplayer first before joining a server !


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

Using this method you can also look into the [OpenXR Toolkit](/opencomposite-openxr-toolkit?id=_72-openxr-toolkit)


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

- If you're using the USB cable and quest link (wired) set the encode bitrate to 500mbps or higher in the Oculus Debug Tool. More info about the [Oculus Debug Tool here](https://smartglasseshub.com/oculus-debug-tool/).  
- Game lagging when using the headset wirelessly: Your router might not be able to handle the high amount of bandwidth required for a smooth experience, this will generally show as high network latency. Try to lower the bitrate in the [Oculus Debug Tool](https://smartglasseshub.com/oculus-debug-tool/) or set it to 0 for auto bitrate.  
- When using USB-C make sure your headset runs at USB 3 and not USB 2 speeds (Should be around 1.5Gbps or higher), if it keeps connecting via USB 2 even with a new cable and using a USB 3 port, reset your headset to factory defaults which will fix the issue.

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

#### **Using OpenComposite**
Use this ONLY if the Oasis SteamVR driver doesn't work for you  
1. Make sure your headset is connected to your PC  
2. Install and set up Windows Mixed Reality from the Microsoft Store
3. Install and set up OpenXR Tools for Windows Mixed Reality from the Microsoft Store  
   3.1. If you see a button that says "Set as active runtime" - press it.  
5. Set up OpenComposite, [instructions here](/opencomposite-openxr-toolkit?id=to-install-opencomposite)  
6. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"  

Using this method you can also look into the [OpenXR Toolkit](/opencomposite-openxr-toolkit?id=_72-openxr-toolkit)

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

Using this method you can also look into the [OpenXR Toolkit](/opencomposite-openxr-toolkit?id=_72-openxr-toolkit)

#### **Using SteamVR**
1. Make sure your headset is connected to your PC
2. Install and set up Pimax Play, [Link here](https://pimax.com/pages/downloads-manuals)
3. Install and set up SteamVR from Steam  
4. In Content Manager go to <ins>Settings > Assetto Corsa > Video</ins> and change "Rendering Mode" to "OpenVR"

<!-- tabs:end -->

</details>
