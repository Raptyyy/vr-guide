# Foveated Rendering

?> Foveated Rendering works ONLY on Nvidia 16xx, 20xx or newer series GPUs, AMD not supported.  

Foveated rendering helps to achieve greater performance by rendering the outer parts of the image at a lower resolution as shown in the example below. On most headsets only the center part of the lense is in focus and can display the image clearly, except for pancake lenses.  
Foveated rendering is a significant performance boost (GPU wise) so it is recommended to take advantage of it.   

<img src="https://github.com/user-attachments/assets/9a4c7415-2240-463d-8455-646f1ae8d1ff" width="400">   

**How to enable Foveated rendering (Use only one of these methods, click to expand):**  
<details>
  <summary style="cursor: pointer; font-size: large"><b>Nvidia VRS in Custom Shaders Patch (Recommended for most users)</b></summary>
    


In **Mode Tweaks: VR** or **Display mode > VR**:

Make sure **Single Pass Stereo** is `enabled`

- **Nvidia VRS** - `enabled`
- **VRS preset** - `Custom`
- **VRS rate** - `High performance`, can set to Highest performance if you need every bit of performance but it will be more visible.
- **VRS detailed area** - set to `Balanced`, set it to `Wide` if you use a Quest 3 or Pico 4 as they will show foveated rendering more clearly.

You can also use the provided presets (VRS preset), however some of them don't help with performance but instead increase image quality.  

?> You can use the VR Tweaks app that lets you adjust all these settings (and more) in-game which you can find here: [VR Tweaks](https://www.overtake.gg/downloads/vr-tweaks.76283/)
</details>  </br>

<details>
  <summary style="cursor: pointer; font-size: large"><b>Foveated Rendering in OpenXR Toolkit</b></summary>



  In the OpenXR Toolkit overlay menu set **Foveated rendering** to Preset - Quality - Balanced, this will be a good starting point, adjust as needed. Custom will allow you to tweak things further.  
  [More info about OpenXR Toolkit](/opencomposite-openxr-toolkit?id=recommended-settings-for-the-toolkit)   
</details>  </br>
  


<summary style="cursor: pointer; font-size: large"><b>For Pimax users you can enable Foveated Rendering in Pimax Play</b></summary>