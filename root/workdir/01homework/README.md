Kernel compile process by Melnikov Alexey

1. Install Vagrant && packets as it guided by TecMint manual
2. Install git
3. Download latest stable kernel - wget
4. unpacking - tar
5. cp current config to .config
6. make oldconfig
7. Install additional packets
8. make oldconfig
9. 1/8 part of questions I answered thoughtfully, but remainig part - just pressed Enter
10. make
11. Installing additional packets
12. make
13. wait about 5 hours
14. make modules
15. make install
16. Oh no! My Mokee swear that directory doesn't exist!
17. mkdir
18. make install success, but with warning on another directories
19. make modules_install
20. make install   Now it worked clear
21. New kernel on /boot/vmlinuz-5.2.8!
22. Unpack to the new dir
23. copy .config from previos
24. make oldconfig - very fast! No changes!
25. In the new dir - make -j4 (4 - cout of my CPU kernel)
26. Great! Compiling take just about 1 hour! But LA was 5.5 versus 2 in the previous time.
27. grub2-mkconfig -o /boot/grub2/grub.cfg
28. reboot
29. uname -r => 5.2.8
30  Amazing! I've just do it!