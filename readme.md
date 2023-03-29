#### Title: "Node.js and Build Tools Installation Guide with Optional OS Upgrades"

1. Get Debian/Ubuntu:
   1. [Install WSL Debian on Windows](https://github.com/brettjrea/Windows_WSL_Debian)
   2. [Install WSL Ubuntu on Windows](https://github.com/brettjrea/Windows_WSL_Ubuntu)
   3. [Install VSCode with Remote Pack on Windows](https://github.com/brettjrea/Windows_VSC_Remote_Pack)

2. Optional OS upgrades:
   1. [Upgrade Debian Bullseye to Buster](https://github.com/brettjrea/Debian_Bullseye_Upgrade_Script)
   2. [Upgrade Ubuntu Focal to Jammy](https://github.com/brettjrea/Ubuntu_Jammy_Upgrade_Script)

3. Node.js tools:
   1. [Install NVM](https://github.com/brettjrea/Debian_Install_NVM) - Node Version Manager
   2. [Install NVS](https://github.com/brettjrea/Debian_Install_NVS) - Node Version Switcher (added 02/23 it is a cross-platform node based successor/replacement for NVM)
   
4. Build tools:
   1. [Install common build tools.](https://github.com/brettjrea/Debian_Install_Common_Build_Tools)
   
6. Add a Backend:
   1. [Install Strapi.io backend](https://github.com/brettjrea/Debian_Strapi_Backend_API)
  
7. Add a Frontend:
   1. [Install Gatsby frontend](https://github.com/brettjrea/Debian_Gatsby_Frontend_Client)
 
8. Configure Process Manager:
   1. [Configure PM2 Process Manager](https://github.com/brettjrea/Debian_Configure_PM2)

9. Add GitHub CLI:
   1. [Install GitHub CLI](https://github.com/brettjrea/Debian_Install_GitHub_CLI)
---
### Upgrade Debian Buster to Bullseye with upgrade.sh

This markdown provides a quick and easy script to upgrade a Debian Buster operating system to Bullseye. The script has been verified as still working in 2022, although it may require the manual installation of wget.

To upgrade Debian Buster to Bullseye with upgrade.sh run the following commands:

```
sudo apt upgrade -y && sudo apt update -y && sudo apt autoremove -y &&
sudo apt install wget -y &&
sudo apt-get install --reinstall ca-certificates -y &&
wget https://raw.githubusercontent.com/brettjrea/Scripts_Fix/master/fixscripts.sh &&
wget https://raw.githubusercontent.com/brettjrea/Debian_Bullseye_Upgrade_Script/master/debian-bullseye-upgrade-script.sh &&
sudo bash fixscripts.sh &&
sudo bash upgrade.sh && 
sudo apt autoremove -y &&
sudo apt clean -y
```