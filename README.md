# Building Home Lab Environment
<h2>Description</h2>
This project consists of two main parts.
In the <a href="#part1">first part</a>, I set up the foundation by downloading and Oracle VirtualBox along with two virtual machines: Windows 10 Pro (using a custom ISO image created via the Media Creation Tool) and Kali Linux (using a pre-built 64-bit virtual machine from kali.org).
In the second part, I configured the network settings for both machines to create a secure sandbox environment.
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


<h3>Part 2:</h3>
<h2>Conclusion</h2>
