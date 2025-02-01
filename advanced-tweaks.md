## Advanced tweaks
### These tweaks are meant to be used only if you understand what they do and how to revert them if needed, not recommended for most people.

### CPU Affinity
Using [Process Lasso](https://bitsum.com/) you can set the CPU affinity to gain some extra performance, especially in the 0.1% / 1% low fps.  
#### A. Disabling SMT / Hyperthreading for Assetto Corsa only. 
1. Install and open Process Lasso (Its free to use)
2. Run Assetto Corsa (Ideally in windowed mode)
3. in Process Lasso find acs.exe, right click, select CPU Affinity > Always > Disable SMT / Hyper-threading
4. Set Process Lasso to run the Governor at startup, click Options > General > Startup options at the top.

#### B. Using only one CCD (Chiplet) on a multi CCD AMD CPU (12 or 16 core).
1. Install and open Process Lasso
2. Run Assetto Corsa (Ideally in windowed mode)
3. in Process Lasso find acs.exe, right click, select CPU Affinity > Always > Select CPU Affinity
4. Select only the first half of the available CPU cores
5. If you wish to also disable SMT, then select only every other core (CPU 0, CPU 2, CPU 4, CPU 6, CPU 8, CPU 10 for my 5900X 12 Core)
6. Press Ok
7. Set Process Lasso to run the Governor at startup, click Options > General > Startup options at the top.

?> If you wish to ondo this, in step 3 simply select None instead and then disable Process Lasso at startup.

### Nvidia ReBar

#### Nvidia ReBar
[You can read about Nvidia ReBar here](https://www.rockpapershotgun.com/what-is-resizable-bar-and-should-you-use-it)  
Make sure Resizable Bar is enabled and supported on your system, its explained in the link above.  

1. Download Nvidia Profiler Inspector [here](https://github.com/Orbmu2k/nvidiaProfileInspector/releases)
2. Click on the Profiles selection bar and type in Assetto Corsa, then select it
3. Under 5 - Common find rBAR, set Feature to "Enabled" and Size Limit to 0x0000000012C00000 (Paste it in)
4. Press Apply changes in the top right

?> If you wish to ondo this, set  rBAR - Feature to "Disabled" and press Apply changes