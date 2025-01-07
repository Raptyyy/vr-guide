## 4. What is Foveated Rendering

?> Note that since Assetto Corsa is a DirectX 11 game, Foveated Rendering works ONLY on Nvidia 16xx, 20xx, 30xx and 40xx series GPUs or newer. 

Foveated rendering is a method in VR to achieve greater performance by rendering the outer parts of the image at lower resolution as shown in the example below. This makes sense on most headsets as only the center part of the lense is in focus and can display the image clearly.  
Foveated rendering is the biggest performance increase (GPU load wise) that you can get in VR so it is highly recommended to take advantage of it.  
Some headsets with eye tracking can support Dynamic Foveated Rendering (more info about this in the future)  

<img src="https://github.com/user-attachments/assets/9a4c7415-2240-463d-8455-646f1ae8d1ff" width="600">   


Ways to enable / use Foveated rendering (Use only one of these methods):  
- Enable "Nvidia VRS" in Custom Shaders Patch, [explained further here](#csp-settings/nvidia-vrs) (Easiest way to enable it)  
- Enable Foveated Rendering in the OpenXR Toolkit if you're using OpenComposite, [explained further here](#opencomposite-openxr-toolkit/recommended-settings-for-the-toolkit) (Gives more adjustability compares to Nvidia VRS)  
- For Pimax users you can enable Foveated Rendering in Pimax Play (More convenient but less options compared to the OpenXR Toolkit)  

?> Foveated rendering might be easily noticeable on headsets that use pancake lenses with large sweetspots such as the Quest 3 or Pico 4, on such headsets it is recommended to use a very large center ring.  
