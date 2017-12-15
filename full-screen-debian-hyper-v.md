# full-screen-debian-hyper-v

Run sudo nano /etc/default/grub
Find GRUB_CMDLINE_LINUX_DEFAULT
Append video=hyperv_fb:[the resolution you want], for example: GRUB_CMDLINE_LINUX_DEFAULT="quiet splash video=hyperv_fb:1920x1080"
Write the changes, quit nano
Run sudo update-grub
Run sudo reboot
h/t https://blogs.msdn.microsoft.com/virtual_pc_guy/2014/09/19/changing-ubuntu-screen-resolution-in-a-hyper-v-vm/
