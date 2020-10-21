## Windows Subsystem for Linux

Windows Subsystem for Linux or WSL lets developers run a GNU/Linux environment directly on windows without using VMware. This above statement itself makes you wonder that what is going in the software industry. Microsoft is certainly gearing to adopt Linux into windows.

I wanted to switch to Linux for a very long time but always hit the roadblock with several things e.g. copying files to the Linux environment, running VMware, and hypervisor at the same time, or dual boots. It was messy and unproductive. The only solution was to buy a new laptop for Linux which I did. 

WSL2 is a total game-changer with the following features and many more: 

1. Choose your favorite GNU/Linux distributions from the Microsoft Store.
2. Run common command-line tools such as grep, sed, awk, or other ELF-64 binaries.
3. Install additional software using your own GNU/Linux distribution package manager.
4. Invoke Windows applications using a Unix-like command-line shell.
5. Invoke GNU/Linux applications on Windows.
6. Ease in copying things b/w windows and WSL.
7. VS Code integration 


### Installation

Please follow the direction [here](https://docs.microsoft.com/en-us/windows/wsl/install-win10) .

### How about docker desktop?

You are in luck, docker desktop has upgraded the architecture to use the WSL2. It means docker desktop moby VM which is a Linux has been migrated to WSL2, it will certainly improve the docker development much easier. Please follow the link provided below:

https://docs.docker.com/docker-for-windows/wsl/

### What is the catch here?

There are certain limitations (I knew that) although this should not limit anything related to development.  e.g.

1. No *systemd *support, so you need to configure startup services manually.

2. Using windows directory has speed implication, so avoid mixing windows directory with WSL directory.

3. It is still windows 

### Additional links 

https://adamtheautomator.com/windows-subsystem-for-linux/


 
So no more excuses for me anymore to learn Linux, haha.





