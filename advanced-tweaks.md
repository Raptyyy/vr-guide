# Advanced tweaks
!> **WARNING** These tweaks are meant to be used only if you understand what they do and how to revert them if needed, not recommended for most people.

### CPU Affinity
#### Using only one CCD (Chiplet) on a multi CCD AMD CPU (12 or 16 core).
1. Install and open [Process Lasso](https://bitsum.com/) 
2. Run Assetto Corsa (Ideally in windowed mode)
3. in Process Lasso find acs.exe, right click, select CPU Affinity > Always > Select CPU Affinity
4. Select only the first half of the available CPU cores (CCD0)
5. Press Ok
6. Set Process Lasso to run the Governor at startup, click Options > General > Startup options at the top.

This can also be done using [Process Governor](https://github.com/SystemXFiles/process-governor) if you wish not to use Process Lasso.

?> If you wish to ondo this, in step 3 simply select None for the CPU affinity and then disable Process Lasso at startup.

### Nvidia ReBar
[You can read about Nvidia ReBar here](https://www.rockpapershotgun.com/what-is-resizable-bar-and-should-you-use-it)  
Make sure Resizable Bar is enabled and supported on your system, its explained in the link above.  

1. Download Nvidia Profiler Inspector [here](https://github.com/Orbmu2k/nvidiaProfileInspector/releases)
2. Click on the Profiles selection bar and type in Assetto Corsa, then select it
3. Under 5 - Common find rBAR, set Feature to "Enabled" and Size Limit to 0x0000000012C00000 (Paste it in)
4. Press Apply changes in the top right

?> If you wish to ondo this, set  rBAR - Feature to "Disabled" and press Apply changes

Comparison of performance difference when using ReBar  
Baseline is ReBar disabled (default)  
0x0000000012C00000 is 300mb  
<img src="https://github.com/user-attachments/assets/79d0b521-cb77-451e-9861-5703f431c0ba" width="800">  
