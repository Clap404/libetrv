# libetrv

Monitor and control your eTRV from Python. Recently Danfoss has released new TRVs that can be controlled
over Bluetooth Low Energy. This library will allow connect this devices and control them.

## About this fork
I made this fork in an effort to get more out of my thermostats using [etrv2mqtt](https://github.com/keton/etrv2mqtt). I merged together these repos.
- https://github.com/AdamStrojek/libetrv
- https://github.com/spin83/libetrv
- https://github.com/bartek56/libetrv

## Supported Devices

All supported and tested devices:

- Danfoss Eco Bluetooth LE - WIP

## Bluetooth Permissions
It is recommended to not start this app as `root` user. To avoid this you can allow python3 to access to Bluetooth interface

```bash
$ sudo apt-get install libcap2-bin
$ sudo setcap 'cap_net_raw,cap_net_admin+eip' `readlink -f \`which python3\``
$ sudo setcap 'cap_net_raw+ep' `readlink -f \`which hcitool\``
```
