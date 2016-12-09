
# Get info
> iwconfig

# Configure wifi hotspot
> sudo vim /etc/wpa_supplicant.conf
network={
    ssid="ssid_name"
    psk="password"
}

# Apply
> sudo wpa_supplicant -B -iwlp3s0 -c/etc/wpa_supplicant.conf -Dwext
> sudo dhclient wlp3s0
