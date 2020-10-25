# install environement before Spark, just python3 and dev environement

Install the environment for the workshop
# Table of Contents
1. WSL
2. Ubuntu 20.04
3. Visual studio code
4. Java in Ubuntu
5. Python3 and importatnt package for python3
    1. pip
    2. venv
    3. jupyterlab

# you have a windows 10 build > 1903

## Add WSL from "Turn windows features on off"
With the GUI or simply open powershell as Adminsitrator

First, open PowerShell as an Administrator and run the following commands:

```ps
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
Reboot if needed

## Install Ubuntu 20.04 and Visual Studio code from microsoft store

### Ububtu 20.04
### Visual studio code

Will be installed in windows usable iin WSL ubuntu

## Run ubuntu

### First time
create a user and password : to use the same user choose **`bdml`**

### install needed softwares on ubuntu 

#### Java version >=8 <=11
```bash
bdml@PF:~$ #WSL ubuntu 20.04 insalled
bdml@PF:~$ #User bdml created
bdml@PF:~$ #install java : sudo apt install default-jre
bdml@PF:~$ #verify by typing java -version
bdml@PF:~$ java -version
openjdk version "11.0.8" 2020-07-14
OpenJDK Runtime Environment (build 11.0.8+10-post-Ubuntu-0ubuntu120.04)
OpenJDK 64-Bit Server VM (build 11.0.8+10-post-Ubuntu-0ubuntu120.04, mixed mode, sharing)
bdml@PF:~$ #must be 8 <= version <=11
```
#### Python3

`sudo apt install python3`

verify

`python3 --version`

```bash
bdml@PF:~$ sudo apt install python3
[sudo] password for bdml:
Reading package lists... Done
Building dependency tree
Reading state information... Done
python3 is already the newest version (3.8.2-0ubuntu2).
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.
bdml@PF:~$ python3 --version
Python 3.8.5
bdml@PF:~$
```

#### inportant package for python

There are a few more packages and development tools to install to ensure that we have a robust setup for our programming environment:

sudo apt install -y python3-pip build-essential libssl-dev libffi-dev python3-dev

#### Setting up JupyterLab
JupyterLab requires Python 3, as well as a Python package manager – we’ll use pip – so let’s install these now. Open a WSL terminal (if you’re not sure how to do this, search for Ubuntu in the start menu and hit return) and type the following command:

sudo apt install python3 python3-pip
You’ll be prompted for your password that you set earlier - note that it won’t show up on the screen at all as you type, but this is normal. After pressing return, you’ll then be prompted to continue, which you can do by pressing return once again.

Now that you’ve installed Python, it’s time to install JupyterLab:

`python3 -m pip install --user jupyterlab pandas matplotlib`

Along with JupyterLab, we’ll also install pandas and Matplotlib, as these are two popular Python libraries used in conjunction with Jupyter itself.

We use the `--user` option to install these packages separately from system packages 
– system ones are managed by apt (the command we used earlier to install Python) and we could cause problems if we install packages with pip globally, rather than with --user.

then try it 

`jupyter lab --no-browser`

We specify the --no-browser option to disable automatically opening a browser window, as this feature doesn’t work in WSL, and instead we’ll open the page manually.
