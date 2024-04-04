1. Go to [HST Secure Gateway](https://remote-access.ahc.umn.edu/logon/LogonPoint/tmindex.html).
2. Log in.
3. You should now be in the Citrix Workspace.
4. Click on Desktops at the top.
5. Double-click on AHC-IE Shared Desktop.
6. You will now find yourselves in Windows.
7. Run PuTTY.
8. For Host Name (or IP address), enter</br>
   * ahcie-gpuctl.ahc.umn.edu
9. In the Windows Command Prompt that is opened, enter your login ID.  It didn't ask me for a password.
10. Enter `srun --nodes=1 --gpus-per-node=1 --time=1:0:0 --pty bash`
11. You will get this error:
```
srun: Required node not available (down, drained, or reserved)
srun: job 387 queued and waiting for resources
```

* https://github.umn.edu/AHC-OPS/GPUClusterWiki/wiki/
* /scratch/ahcie-gpu2/CQODE_MHFV
* https://portunus.ahc.umn.edu/
* https://confluence.ahc.umn.edu/display/DSV2/Anaconda+Virtual+Environment+Setup+on+Windows
