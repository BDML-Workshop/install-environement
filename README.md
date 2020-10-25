# install-environement

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
With the GUI or simply open powershell as Adminsitrator and run this command

```ps
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all
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

