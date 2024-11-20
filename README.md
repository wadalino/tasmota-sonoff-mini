# Tasmota on Sonoff mini 
[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/wadalino)

## Link to GitLab code

**IMPORTANT** >>> [Please refer to this location](https://gitlab.wadalino.org/wdln-public/tasmota-sonoff-mini)

---
### Compatibility

This software works on devices:  
- Sonoff Mini
- Sonoff Mini R2

### Requeriments

To execute this software you must run it on a Linux system with **Python3** installed with modules:  
- colorama
- docker
- dotenv
- requests
- rich
  
You can install with:  
```code 
pip install python-dotenv rich docker colorama requests
```

However, next modules are built-in:  

- asyncio
- hashlib
- ipaddress
- json
- multiprocessing
- os
- re
- threading
- time
- socket
- warnings

You need to have installed on system 'docker', 'nmap', 'network manager' and 'wireless tools'  

* ### Network Manager
 
NetworkManager, a utility for managing network connections on Linux-based systems. nmcli allows users to interact with the NetworkManager service from the command line, enabling tasks such as managing Wi-Fi connections, checking network status, and configuring interfaces.  

You can install it on most Linux distributions via package managers like apt on Debian-based systems (e.g., Ubuntu) or dnf on Red Hat-based systems (e.g., Fedora).  

On Ubuntu/Debian, you can install it with:  
```code
sudo apt install network-manager
```
On Fedora, you can install it with:  
```code
sudo dnf install NetworkManager
```

* ### Nmap
Nmap (Network Mapper) is an open-source tool used for network discovery and security auditing. It can be used to discover hosts and services on a computer network, thus creating a "map" of the network.  
On Linux (Debian-based, e.g., Ubuntu):  
```code
sudo apt install nmap
```
On Linux (Red Hat-based, e.g., Fedora):  
```code
sudo dnf install nmap
``` 

* ### Wireless tools
The wireless-tools package provides a set of utilities for managing wireless networking in Linux, which includes tools for configuring wireless interfaces, getting wireless statistics, and querying the status of wireless networks.  
On Debian-based systems (e.g., Ubuntu):  
```code
sudo apt-get install wireless-tools
``` 
On Red Hat-based systems (e.g., Fedora):  
```code
sudo dnf install wireless-tools
``` 

* ### Docker
Docker is an open-source platform used for developing, shipping, and running applications inside lightweight, portable containers. A container is a standard unit of software that packages up code and all its dependencies so that the application runs quickly and reliably across different computing environments. With Docker, developers can ensure their application behaves the same way on any machine, whether in development, testing, or production environments.  

Please refer to the Docker installation guide at: https://docs.docker.com/engine/install/   

----

## Execution

### Pre-Configure

First is necessary to configure .env file to fill variables according your necessities, this is fill MQTT user and password, set the ip address for Home Assitant, set the ssid and the password for Wi-Fi Network  

### Executing

The user that execute the program need to be allowed to execute docker containers.  

```code 
python3 main.py
```

----

## To-Do:

- Integrate Nmap with Python instead using subprocess
- Translate comments in various files to English

--- 
# Thanks

### If this software is useful to you, please consider to ...  

---

  
<div style="text-align: center;">
<img src="img.png" alt="Buy Me A Coffee" width="200">
     
[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/wadalino)
</div>
