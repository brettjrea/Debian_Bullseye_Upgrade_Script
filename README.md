# Debian_Bullseye_Upgrade_Script
Upgrade Debian Buster to Bullseye with upgrade.sh


## Always be updating:

```
sudo apt upgrade -y && sudo apt update -y && sudo apt autoremove -y
```

---

## Install required programs:

```
sudo apt install wget
```

---
## Commands:

```
wget https://raw.githubusercontent.com/brettjrea/Scripts_Fix/master/fixscripts.sh &&
wget https://raw.githubusercontent.com/brettjrea/Debian_Bullseye_Upgrade_Script/master/upgrade.sh &&
sudo bash fixscripts.sh &&
sudo bash upgrade.sh && 
sudo apt autoremove -y &&
sudo apt clean -y
```

---

*The following command adds emac key bindings good for the missing up and down keys on chromeos virtual keyboard.*

```
set -o emacs
```

*Ctrl-p is previous or up.*

*Ctrl-n is next or down.*

---

*You might now want to [Install NVM](https://github.com/brettjrea/Debian_Install_NVM)*
