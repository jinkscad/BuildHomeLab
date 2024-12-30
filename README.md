# Building Home Lab Environment
<h2>Description</h2>
This project consists of two main parts.
In the <a href="#part1">first part</a>, I set up the foundation by downloading and Oracle VirtualBox along with two virtual machines: Windows 10 Pro (using a custom ISO image created via the Media Creation Tool) and Kali Linux (using a pre-built 64-bit virtual machine from kali.org).
In the <a href="#part2">second part</a>, I configured the network settings for both machines to create a secure sandbox environment.
The goal of this project is to build a controlled space for practicing malware analysis and gaining a deeper understanding of networking principles.
<br />
<h2>Languages and Utilities Used</h2>
- Oracle VirtualBox<br />
- Windows Media Creation Tool<br />
- Kali Linux Pre-built Virtual Machine <br />
- Windows 10 Pro ISO Image<br />
<h2>Environments Used </h2>
- Host Machine: Windows 11 Pro<br />
- Guest Virtual Machines: Windows 10 Pro, Kali Linux (64-bit)<br />

<h2>Project walk-through</h2>
<h3 id="part1">Part 1:</h3>
First, I downloaded VirtualBox 7.1.4 for windows host from <a href="https://www.virtualbox.org/wiki/Downloads">virtualbox.org</a>. I did not customize VirtualBox in this project.<br />    I built two virtual machines. The first one is Windows 10 Pro, for which I created an ISO image using a<a href="https://www.microsoft.com/en-ca/software-download/windows10iso"> media creation tool.</a> I named this virtual machine "demo" and configured it with a base memory of 4 GB, one CPU, and a virtual hard disk of 50 GB.<br />
The second machine is Kali Linux, which I downloaded and imported as a 64-bit pre-built virtual machine from <a href="https://www.kali.org/get-kali/#kali-virtual-machines" target="_blank">kali.org</a>. I did not perform any additional configuration for this machine. With this, the basic setup of downloading and importing the necessary tools was completed, resulting in the state shown in the picture below.
<img src="https://i.imgur.com/73Ajar1.png" alt="Setup State" style="max-width: 100%; height: auto;">
<h3 id="part2">Part 2:</h3>
Here, I configured the network settings of the two virtual machines to enable malware analysis. In this lab, I set up an Internal Network where the two virtual machines can communicate with each other but are isolated from the host machine.

First, I configured the Windows 10 virtual machine. I set its network adapter to "Attached to Internal Network" and named the network "mytest." 
<img src="https://i.imgur.com/nBy0AgS.png" style="max-width: 100%; height: auto;"><br />
I applied the same configuration to the Kali Linux virtual machine, ensuring that both machines are on the same internal network.
<img src="https://i.imgur.com/Ycp3d0m.png" style="max-width: 100%; height: auto;">

Next, I assigned static IP addresses to both machines so they could communicate seamlessly. For the Windows machine, I set the IP address to 192.168.20.10.
<img src="https://i.imgur.com/MeXIoi3.jpeg" style="max-width: 100%; height: auto;">
<img src="https://i.imgur.com/syXQXlo.jpeg" style="max-width: 100%; height: auto;">
I configured the Kali Linux machine the same.
<img src="https://i.imgur.com/U8ekVQM.jpeg" style="max-width: 100%; height: auto;">
<img src="https://i.imgur.com/p7PdPP0.jpeg" style="max-width: 100%; height: auto;">

Finally, I verified the connectivity between the two machines by using the ping command from the Windows machine. As shown in the image below, the two machines successfully connected and communicated with each other.
<img src="https://i.imgur.com/kZSpWuw.jpeg" style="max-width: 100%; height: auto;">
<h2>Conclusion</h2>
