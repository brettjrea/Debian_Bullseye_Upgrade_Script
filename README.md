# Debian_Bullseye_Upgrade_Script
Upgrade Debian Buster to Bullseye with upgrade.sh

---
## Commands:

```
sudo apt update -y &&
sudo apt upgrade -y &&
sudo apt autoremove -y &&
sudo apt install wget -y &&
wget https://raw.githubusercontent.com/brettjrea/Scripts_Fix/master/fixscripts.sh &&
wget https://raw.githubusercontent.com/brettjrea/Debian_Bullseye_Upgrade_Script/master/upgrade.sh &&
sudo bash fixscripts.sh &&
sudo bash upgrade.sh && 
sudo apt autoremove -y &&
sudo apt clean -y
```

---

*You might now want to [Install NVM](https://github.com/brettjrea/Debian_Install_NVM)*
