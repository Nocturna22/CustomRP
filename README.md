# Custom-RockPi-setup


With this simple setup it is possible to customize a new installation of DietPi on the RockPi4 like I always do. It is possible to do single parts of this installation on other boards. 

### What is possible so far:

- Wireguard installation on a RockPi with DietPi
- Change the Bashpromt
- Change MOTD for DietPi





Example:
![BashPromt example](https://raw.githubusercontent.com/twerpyfie/Custom-RockPi-setup/master/files/Bashpromt.PNG?raw=true "BashPromt")



**Usage:**

```bash
$ git clone https://github.com/twerpyfie/Custom-RockPi-setup.git
$ cd Custom-RockPi-setup
$ sudo chmod +x ./Setup
$ sudo bash ./Setup
```

### To do:

- Include wireguard configurator
- Include wireguard QR-Code generator for Peers
- Include Pihole installation
- Maby make some new Repositorys for the other Projects included
- Maby make for every underproject an single file that will be executed
- Maby make an updater
