# install-environement

Install the environment for the workshop

# you have a windows 10 build > 1903

## Add WSL from "Turn windows features on off"
With the GUI or simply open powershell as Adminsitrator and run this command

```ps
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all
```

Reboot if needed

## Install Ubuntu 20.04 and Visual Studio code from microsoft store

## Run ubuntu

### First time
create a user and password : to use the same user choose **`bdml`**

### install needed softwares on ubuntu 
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
