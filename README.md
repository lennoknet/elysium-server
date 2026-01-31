# Elysium Server for Debian

This is a guided bash script for easy setup of a Echoes of Elysium dedicated server for command line interface (CLI) users only.
This solution consists of a bash script that automates the process.

## Prerequisites

Refer to https://developer.valvesoftware.com/wiki/SteamCMD#Debian
You need to have software-properties-common installed as well as non-free repository and i386 architecture.

## Documentation

If you have not much clue of Linux, you may also use my step-by-step manual to set up the machine to be able to run the script:
https://github.com/lennoknet/elysium-server/blob/main/preparation.md
NAT and Port rules for your router is then your only thing you need to work on yourself.

## Installation

Ensure you have Debian 12 or 13 installed properly, given your machine a static IP or fixed it at your DHCP. The machine should have internet access and ensure the game port you want to use is accessible through NAT.

To install the Echoes of Elysium Server, please clone the repo, make the install script executable, and then run it:

```bash
git clone https://github.com/lennoknet/elysium-server.git
cd elysium-server
chmod +x setup-elysium-server.sh
./setup-elysium-server.sh
```

## Usage/Examples

Start server:     `systemctl start elysium-server.service`  
Stop server:      `systemctl stop elysium-server.service`  
Restart server:   `systemctl restart elysium-server.service`  
View logs:       `journalctl -u elysium-server.service -f`  
