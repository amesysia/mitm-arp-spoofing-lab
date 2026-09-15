# My Lab Environment and First MITM Attack
Welcome to my first cybersecurity write-up. In this write-up, I will be sharing how I configured an isolated lab environment using VirtualBox and executed my first ever Man in the Middle (MITM) attack, also known as ARP spoofing attack.

As for my lab environment, I downloaded and installed both Kali and Windows 7 machines. Then I set up a NAT Network for them, an isolated network for these machines to communicate.

I ran commands to see their IP addresses, `ifconfig` on Kali and `ipconfig` on Windows. The IP address of the Windows machine was 10.0.2.4, whilst Kali’s was 10.0.2.3.

I needed them to be able to see each other, so I ran `arp -a` on Windows. There, I stumbled upon an issue.

![description](screenshots/screenshot-1.png)
