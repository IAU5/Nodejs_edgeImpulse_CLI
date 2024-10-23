# Nodejs_edgeImpulse_CLI

## Installation procedure:  
 Install Chocolatey Individually - you might be able to skip this if it’s already installed correctly

1. Open Windows PowerShell and give the following command:   Get-ExecutionPolicy 
2. If it returns “restricted” copy the following command and paste it:  Set-ExecutionPolicy Bypass -Scope Process
3. Run this command next:
 “ Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1')) “
4. If you don't see any errors, you are ready to use Chocolatey!


## Install Node.js
1. Go to https://nodejs.org/en and download the latest version LTS
2. Install it , make sure to click the add path option and *Check mark the additional tools needed while installing node.js*
3. It will take some time but should install without and issues.


## Install edge impulse cli
1. Open Powershell again and paste and run this command :  

“ Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iwr -Uri "https://raw.githubusercontent.com/edgeimpulse/ei-install-scripts/main/install-windows.ps1" -Outfile install.ps1; iex .\install.ps1; del .\install.ps1 “


If everything works good then you should be able to install the firmware and do the lab without any issues, use the following link to continue with the rest of the procedure: 

https://docs.edgeimpulse.com/docs/edge-ai-hardware/mcu/arduino-nano-33-ble-sense
