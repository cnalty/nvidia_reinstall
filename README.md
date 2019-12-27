# A guide to reinstalling NVIDIA Drivers, CUDA and cudnn on Ubuntu

1. Download The runfile (local) for the CUDA version you wish to use at https://developer.nvidia.com/cuda-downloads
2. Reboot your machine in recovery mode. Instructions [here](https://wiki.ubuntu.com/RecoveryMode)
3. Once recovery mode boots, select networking so you're changes will be saved to your machine
![recovery_image](https://github.com/cnalty/nvidia_reinstall/edit/master/recoveryimage.png)
4. Then choose the root option.
5. Remove your previous nvidia drivers and cuda. This process depends on how you previously installed CUDA, instructions found [here](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html#handle-uninstallation)
6. Install the new drivers with "sudo sh /path/to/cuda/runfile" and follow the prompts. (note you can skip scrolling through the EULA by pressing q if it is displayed with more)
7. Once installiation is completed enter the "exit" command and select the resume option from the boot menu.
