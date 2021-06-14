# wpa_supplicant_cd_gentoo
Como configurar wpa_supplicant desde el CD de instalación de gentoo

`ip link`

`nano /etc/wpa_supplicant/wpa_supplicant-<Nombre_interfaz>.conf`

```
-* archivo wpa_supplicant *-
ctrl_interface=/run/wpa_supplicant
update_config=1
```

`wpa_passphrase <SSID> <passwd> >> /etc/wpa_supplicant/wpa_supplicant-<Nombre_interfaz>.conf`

`wpa_supplicant -B -i <Nombre_interfaz> -c /etc/wpa_supplicant/wpa_supplicant.conf`
