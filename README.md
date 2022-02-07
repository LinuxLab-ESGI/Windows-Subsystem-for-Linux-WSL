# Windows Subsystem for Linux (known as WSL)

*This article has been written to complete the presentation and to deal in depth with the subject in detail.*
__________

## What is the WSL and how it works ?

The WSL for **W**indows **S**ubsystem for **L**inux is a compatibility layer developed by Microsoft for running Linux binaries natively (ELF format) in a console environment on Windows 10 and Windows 11. This ingenious technology provides a Linux-compatible kernel interface and can interact directly with the windows operating system with performances very close to a native Linux distribution. Moreover, it allows a user to chose a Linux distribution to install from the Microsoft Store (more info in below).

### WSL is not a virtual machine !

Oh my god, I have heard so many times *"WSL ? Yeah it's like a virtual machine on your Windows"* and it makes me want to vomit...
Although WSl uses virtualization technologies in some cases (more information in the next section), it does not work in a partitioned environment on your Windows system like a virtual machine on VMWare or Virtualbox.

Indeed, if you try to delete your Document folder for example, you will notice that it will be permanently removed from your computer. You can also create a new file with a text editor like vim or nano, and you will be able to edit it with a Windows text editor (like notepad. The WSL can access and interact with your file system directly.

> For the curious ones, we tried to do a `rm -fr /mnt/c` command with the WSL and the root privileges, to delete all the files in the **C:\\** directory. It seems that the WSL can only delete the files in the user folder in **C:\Users\<name_of-the_user>**. However, the windows system becomes quite unstable and slow.

### WSL 1 vs WSL 2

### The limits of WSL

## Install WSL on Windows

### Requirements

First, you must be running Windows 10 version 2004 or higher (Build 19041 or higher) or Windows 11.

>To check your Windows version and build number, select Windows logo key + R, type winver and select OK.

### Download WSL

### WSL distributions available at this time

## Example of WSL use cases

### Mount an ext file system on Windows with WSL

### Add a desktop environment to your WSL

### Use Docker on Windows (with WSL2 only)

## Pengwin Linux

## Appendix - Sources and References

You can find here all the references that we used to write this article and the presentation :

https://docs.microsoft.com/en-us/windows/wsl/about

https://docs.microsoft.com/en-us/windows/wsl/install

https://docs.microsoft.com/en-us/windows/wsl/compare-versions

https://www.whitewaterfoundry.com/what-is-wsl
__________
<i>Updated : 01/02/2022, Authors : Xen0rInspire, AnthonyF</i>
