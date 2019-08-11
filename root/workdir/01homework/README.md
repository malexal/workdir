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
20. make install Now it worked clear
21. New kernel on /boot/vmlinuz-5.2.8!