# Docker Environment

This portion of the guide, will walk through setting up the Docker Environment to be used for development and deployment of the 2018 Hack Oregon Transportation Systems project.

It will also provide some introductory information into Docker to help our volunteers get up and running in this project season.

## Getting Started - What is Docker?

If you are not familiar with Docker, your first step should be understanding the basics of Docker, ie how it works, some terms, and how it is different then running a full virtual machine like Vagrant.

I would suggest watching this video to get a short introduction into Docker:  
[Docker Tutorial - What is Docker & Docker Containers, Images, etc?](https://www.youtube.com/watch?v=pGYAg7TMmp0)


This is also a great guide to review:  
[A Beginner-Friendly Introduction to Containers, VMs and Docker](https://medium.freecodecamp.org/a-beginner-friendly-introduction-to-containers-vms-and-docker-79a9e3e119b)

Next, you will need to install Docker if you have not already...


## Installing Docker

Instead of providing specific instructions here, we will link to the Docker guides on installing.

* We will be working with Docker CE (Community Edition) as an Open Source Project.

### Installing for Macs

*System Requirements*

* Mac hardware must be a 2010 or newer model, with Intel’s hardware support for memory management unit (MMU) virtualization; i.e., Extended Page Tables (EPT) and Unrestricted Mode. You can check to see if your machine has this support by running the following command in a terminal: sysctl kern.hv_support

* macOS El Capitan 10.11 and newer macOS releases are supported. At a minimum, Docker for Mac requires macOS Yosemite 10.10.3 or newer, with the caveat that going forward 10.10.x is a use-at-your-own risk proposition.

* Starting with Docker for Mac Stable release 1.13, and concurrent Edge releases, we will no longer address issues specific to macOS Yosemite 10.10. In future releases, Docker for Mac could stop working on macOS Yosemite 10.10 due to the deprecated status of this macOS version. We recommend upgrading to the latest version of macOS.

* At least 4GB of RAM

* VirtualBox prior to version 4.3.30 must NOT be installed (it is incompatible with Docker for Mac). If you have a newer version of VirtualBox installed, it’s fine.

If your system does not meet these minimum requirements you will not be able to run Docker for Mac. You may attempt to run using [Docker Toolbox](https://docs.docker.com/toolbox/overview/) but this has not been tested and we may have limited assistance to troubleshoot issues.

*Installation*

When you are ready follow Docker's Official Guide to install Docker for Mac:  
[Docker for Mac Installation](https://docs.docker.com/docker-for-mac/install/)

All work should be done using the "Stable" build.

### Installing for Windows 10
Some quick notes:

* These instructions are for the stable release of Docker for Windows (as opposed to the edge release).
* These instructions also assume a 64-bit Pro version of Windows with Hyper-V installed. If your machine does not meet these specs, please try [Docker Toolbox](https://docs.docker.com/toolbox/overview/). You could also run the local Ubuntu instance installed with the Creators Update, and use the [Ubuntu Install Instructions](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/).
* This process will involve at least one restart.
* The following tools are highly recommended for managing Docker for Windows:
    * [Windows Git](https://git-scm.com/download/win)
    * [Visual Studio Code](https://code.visualstudio.com/)
    * Alternatively, you could use PowerShell or cmd

To begin, navigate to [Docker for Windows Installation](https://docs.docker.com/docker-for-windows/install/#download-docker-for-windows) and download the stable install. Once downloaded, run the executable.

After a restart, Docker will probably start automatically, but if not, simply open it through the icon. You should notice the whale in your notifications bar. From Git Bash, CMD, or PowerShell, run the following command:

```docker run hello-world```

Docker should pull down the necessary image from the Docker daemon and display the results, thus verifying the proper installation.

### Installing for Ubuntu/Linux Systems

You will want to consult Docker's Guides to installation on Linux Systems:

* [Ubuntu](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/)
* [Debian](https://docs.docker.com/engine/installation/linux/docker-ce/debian/)
* [CentOS](https://docs.docker.com/engine/installation/linux/docker-ce/centos/)
* [Fedora](https://docs.docker.com/engine/installation/linux/docker-ce/fedora/)
