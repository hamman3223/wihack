# W! hack Cheetsheat
<br />

## Set Up environment
<br />

|Purpose|Command|
|----|----|
|lsusb|List all usb devices attached to machine|
|ethtool -i {interface} | Get detailed information about interface|
|iwconfig | View all WiFi interfaces on system | 
|iw phy| View information about an interfaces and its capabilities|
|iw reg get|Check the regulatory domain|
|iw reg set {region}|Set reg domain |
|iw dev {interface} set channel {number}|Setting channel |
|iwconfig {interface} essid {ssid} | Connect to specific SSID|

<br />
<br />

<h2>
<b>Configure hostapd service to deploy Honey Pot</b></h2>


```
## To configure hostapd for WiFi Honeypot firstly we need to install it

    sudo apt install hostapd

## Therefore we need to create configuration file

    touch /etc/hostapd/hostapd.conf

## hostapd.conf content is ...

    interface={interface}
    driver=nl80211
    ssid={ssid}
    bssid={mac_addr}
    channel={channel}

## After that just start hostapd service

    systemctl start hostapd.service
```
<br />

<h2><b>Toolkits/Plugins</b></h2>

|Name|Description|
|----------|------------|
|<a href="https://github.com/pentesteracademy/patoolkit"> Patoolkit </a>|Wireshark plugin, which implements the automation WiFi packets analysis|

<br />

## Attacks

|Type of attack|Command|
|---------------|-------------|
|Deathentication Attack|aireplay-ng -0 {count} -a {bssid} {interface} -c {sta_mac}|
|WiFi HoneyPot|hostapd {config_file}|
|Beacon flood|mdk4 {interface} b|


<br />
