# merc1_klipper
Mercury One Klipper profile

# Install KAMP macros

https://github.com/kyleisah/Klipper-Adaptive-Meshing-Purging

cd ~

git clone https://github.com/kyleisah/Klipper-Adaptive-Meshing-Purging.git

ln -s ~/Klipper-Adaptive-Meshing-Purging/Configuration printer_data/config/KAMP

cp ~/Klipper-Adaptive-Meshing-Purging/Configuration/KAMP_Settings.cfg ~/printer_data/config/KAMP_Settings.cfg
 
# Install Beacon

https://docs.beacon3d.com/quickstart/

cd ~

git clone https://github.com/beacon3d/beacon_klipper.git

./beacon_klipper/install.sh

# Orbiter / Filament Sensor / Orbitool
https://www.orbiterprojects.com/orbitools/

# E34M1
https://github.com/jon-harper/E34M1

# Enraged Rabbot Carriage Feeder
https://github.com/Enraged-Rabbit-Community/ERCF_v2

# Happy Hare
https://github.com/moggieuk/Happy-Hare/tree/main

cd ~

git clone https://github.com/moggieuk/Happy-Hare.git


# Calibration
With Beacon, auto calibrate axis twist:
AXIS_TWIST_COMPENSATION_CALIBRATE AUTO=True

# WIFI
## Disable
**rfkill block wifi**

## Enable
**rfkill unblock wifi**

## Status
**rfkill**

## Disabled on boot
added to \boot\firmware\config.txt
dtoverlay=disable-wifi