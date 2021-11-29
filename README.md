# OSagnosticDESops

This is a repository for instructions on how to do Operating System Agnostic Data Engineering Science Operations, especially for students of Mathematics, Computer Science, Statistics, Data Science and Data Engineering.

## Problem 0, Individual Assignment 3

Please do the following STEPS to document your installation of SageMath on your laptop's and/or desktop's operating system(s):

1. STEP 0: Get a Github Account at https:/github.com if you do not already have one and install git on your laptop by following this [Quickstart](https://docs.github.com/en/get-started/quickstart) with these two minimal steps:
    - [Hello World](https://docs.github.com/en/get-started/quickstart/hello-world)
    - [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
2. STEP 1: fork **this** GitHub repository: [https://github.com/datascience-intro/OSagnosticDESops](https://github.com/datascience-intro/OSagnosticDESops) 
    - the easiest way is to login to your GitHUb account and go to the above URL, 
    - click the 'fork' button from the web browser [as shown here](images/fork00.png),
    - choose your GitHub username where you want the fork of OSagnosticDESops repository to go to [as shown here](images/fork01.png),
    - now you should be able to see your fork of the repository at `https://github.com/yourGitHubUsername/OSagnosticDESops/` [as shown here](images/fork02.png),
    - go to `Code` and chose one of the methods (SSH is recommended; HTTPS or CLI are also ok; see [connect with SSH](https://docs.github.com/en/enterprise-server@3.0/authentication/connecting-to-github-with-ssh) for the setup instructions) [as shown here](images/fork03.png),
    - finally you can go into the appropriate directory in your local machine (laptop/desktop) and clone your fork of the repository [as shown here](images/fork04_cloneYourForkLocally.png),
    - you can stay up to date with the upstream [https://github.com/datascience-intro/OSagnosticDESops](https://github.com/datascience-intro/OSagnosticDESops) [as showh here](images/fork05_fetchAndMetgeUpstream.png) and commit and push your own changes by taking a brief tour of [git](https://en.wikipedia.org/wiki/Git) and completing other steps in [Quickstart](https://docs.github.com/en/get-started/quickstart).
3. STEP 2: You main task is to document the steps you took to install SageMath the easy way from binaries or the harder way from source on your local machine, by following the guidelines in:
    - [https://github.com/datascience-intro/how2_MacOSX_2SageMath-2021](https://github.com/datascience-intro/how2_MacOSX_2SageMath-2021)
    - [https://github.com/datascience-intro/how2_WindowsOS10-\_2SageMath-2021](https://github.com/datascience-intro/how2_WindowsOS10-_2SageMath-2021)
    - You may either document using markdown by editing this `README.md` file in your fork of this repository by simply writing down the steps you took to install SageMath
    - Or give a URL to another repository that documents your installation steps in detail
    - The main expectation is that you should be able to install SageMath on your local machine a lot faster by following the instructions you have given
    - Below are the steps I have taken to install SegeMath on my laptop
    - 1. Install WSL and Ubuntu on [https://docs.microsoft.com/en-us/windows/wsl/install](https://docs.microsoft.com/en-us/windows/wsl/install)
    - 2. Set up my user info (username and password) in WSL
    - 3. Run update and upgrade to the packages by sudo apt update && sudo apt upgrade (error on unable to resolve domains occurred here so I resorted to passing an extra line of code: echo "nameserver 8.8.8.8" | sudo tee /etc/resolv.conf > /dev/null (Reference: [https://github.com/MicrosoftDocs/WSL/issues/937](https://github.com/MicrosoftDocs/WSL/issues/937))
    - 4. Update Ubuntu to 20.10 following the steps here [https://linuxconfig.org/how-to-upgrade-ubuntu-to-20-10](https://linuxconfig.org/how-to-upgrade-ubuntu-to-20-10) (For some reasons, sudo do-release-upgrade -d does not work on my laptop. So instead, I followed the instructions here [https://github.com/microsoft/WSL/issues/6942](https://github.com/microsoft/WSL/issues/6942) to replace focal with groovy manually in /etc/apt/sources.list with nano or sed, and do an apt update; apt upgrade)
    - 5. Download Sage9.1 from this site [https://www.sagemath.org/download-source.html](https://www.sagemath.org/download-source.html]
    - 6. Follow the procedures in [https://doc.sagemath.org/html/en/installation/source.html#sec-installation-from-sources-linux-recommended-installation](https://doc.sagemath.org/html/en/installation/source.html#sec-installation-from-sources-linux-recommended-installation) to build sege
    - 7. Follow the images in [https://github.com/datascience-intro/how2_WindowsOS10-_2SageMath-2021/tree/main/images/settingUpSageMathInWSL2UbuntuOnWindows](https://github.com/datascience-intro/how2_WindowsOS10-_2SageMath-2021/tree/main/images/settingUpSageMathInWSL2UbuntuOnWindows) to install python/Sage packages, change %PATH variable, install Visual Studio, et cetera.
 
Further instructions, if needed, will follow shortly after the computer labs in Angstrom are tested. Please discuss in threads at the course instructure page so you can learn from one another.
