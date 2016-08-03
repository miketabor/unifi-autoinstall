# unifi-autoinstall
Script that automates upgrading and securing of a Ubuntu host then deploys the Ubiquiti UniFi Controller.

To learn more, visit [https://miketabor.com](https://miketabor.com/install-ubiquiti-unifi-controller-cloud/ "How to install Ubiquiti UniFi controller on the cloud - MikeTabor.com") and follow [@tabor_mike](https://twitter.com/tabor_mike) on Twitter.

## What it does

* Updates all packages on the system.
* Configures UncomplicatedFirewall (UFW) to allow only SSH and Ubiquiti UniFi ports, then enables UFW.
* Adds the UBT repo then installs latest version 5 of UniFi Controller.
* Installs Fail2ban then adds definition and fail regex to monitor for failed UniFi logins.

### How to use
Simply run the following command from terminal:
```
wget https://raw.githubusercontent.com/miketabor/unifi-autoinstall/master/install.sh
less install.sh
sudo bash install.sh
```
Log into UniFi by going to: **https://SERVER_IP:8443**
