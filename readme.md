# Easy-Install-Docker-in-Windows-with-Powershell-script

## Introduction
Installing docker in windows is a troublesome task. This repo will help you to install docker on windows. 

## Running the Script
Clone the repository
```sh
git clone https://github.com/chinmay-d/Easy-Install-Docker-in-Windows-with-Powershell-script.git
```
Open windows Powershell with administrator privileges by `Menu > Windows Powershell > Run as Administrator`.

`cd` to the path where you have the cloned repository and then simply run
```sh
.\dockerinstallwsl2.ps1
```

**Note:**  Read the below instruction thoroughly and then run the script.

## To Install Docker <br>

**Note:** Step 1 has to be manually done and other steps will be done automatically by running the provided script

1. Turn on virtualization technology by entering into BIOS. As docker runs natively over Linux and to run Linux on a system we have to turn on the `Virtualization Technology` from the BIOS.
2. The  provided script will check if hyper-V is enabled (requirement to install ubuntu distro). If hyper-V is not enabled the script will enable the hyper-V.
3. Now when you restart the system the hyper-V is enabled and the script will check if WSL certificate is on verion 2. If not then the script will download and set the wsl certificate to version 2 and ask for `restart`. <br>
**Note:** Run the script again after restarting the system.
4. Now the script will download and set the linux kernel and update its packages and ask for a `restart`. <br>
**Note:** Run the script again after restarting the system.
5. Finally, after all requirements for installing docker in windows are satisfied the script will install docker and ask for a `restart`, this is the final `restart`.

Now you will be able to see docker installed into your windows system. 🎊 🎊 🥳 🥳
