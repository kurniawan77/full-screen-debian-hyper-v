# full-screen-debian-hyper-v

1. Run `sudo nano /etc/default/grub`
2. Find `GRUB_CMDLINE_LINUX_DEFAULT`
3. Append `video=hyperv_fb:[the resolution you want]`, for example: `GRUB_CMDLINE_LINUX_DEFAULT="quiet splash video=hyperv_fb:1920x1080"`
4. Write the changes, quit nano
5. Run sudo update-grub
6. Run sudo reboot

h/t https://blogs.msdn.microsoft.com/virtual_pc_guy/2014/09/19/changing-ubuntu-screen-resolution-in-a-hyper-v-vm/
