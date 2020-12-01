## My Raspberry Pi fresh install instructions
How to format your readme.md on GitHub: [GitHub Readme Markdown](https://guides.github.com/features/mastering-markdown/)

### Install from scratch instructions

#### Create bootable OS

1. Download [Raspberry Pi Imager](https://www.raspberrypi.org/software/)
2. Insert Micro SD card and install desired OS
3. Unplug card from PC and insert into Raspberry Pi

#### Instalation process

1. Connect the Display and keyboard
2. Power on the device (Plug in the power source)
3. Wait for system auto installation
4. Log in Raspberry Pi OS default user (username: **pi**, password: **raspberry**)
4. Configure CLI (Optional)
```bash
sudo dpkg-reconfigure console-setup
```
5. Configure Your Raspberry Pi Device
```bash
sudo raspi-config
```
6. Alternative network configuration
```bash
sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
```

7. Install additional software
Install software by starting [script](https://github.com/crazieNephilim/crazie_scripts/blob/master/raspberry_scripts/raspberry_resources/rspberry_pi_4_small_home_server.sh)
Installed software:
- [Git](https://git-scm.com/)
- [Java default-jdk](https://packages.debian.org/stretch/default-jdk)
- [Ranger](https://github.com/ranger/ranger)
- [Apache Tomcat 9 Full](https://tomcat.apache.org/index.html)
- [PostgreSQL](https://www.postgresql.org/)

8. Configure installed software

    1. [Tomcat](https://github.com/crazieNephilim/crazie_scripts/tree/master/raspberry_scripts/raspberry_resources/README_TOMCAT9.md)
    2. [PostgreSQL](https://github.com/crazieNephilim/crazie_scripts/tree/master/raspberry_scripts/raspberry_resources/README_POSTGRESQL.md)