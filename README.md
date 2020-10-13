# Server_stuff

## MISC

- `landscape-sysinfo`

Show general system information

## DISKs

- `lsscsi -g`

Information about Disks

- `blkid`
Detailed information about all Disks, including Label type etc.

- `ls -lastr /dev/disk/by-id`
- `ls -l /dev/disk/by-id`

Show symlinks of Disks

- `smartctl -l selftest /dev/{XX}`
Selftest of a specific Disk

## LXC
- `lxc-ls -f`

List all lxc

- `lxc-attach -n {XX}`

Attach to lxc ("login")

- `lxc-stop -n {XX}`

Stop a running LXC (takes a bit to stop)

- `lxc-start -n {XX} -d`

Start a lxc in **detached (-d)** mode

## LXD
- `lxc list`

List all lxd

## IPMItool
- `ipmitool sel list`

Show **S**ystem **E**vent **L**og

- `ipmitool sel elist`

Show **E**xtended **S**ystem **E**vent **L**og

- `ipmitool sel clear`

Clear SEL

- `ipmitool sdr list`
- `ipmi-sensors`

Show Sensor list


## SCREEN
- `screen -l`

List all open Screens

- ´screen -S {XX}`

Create a new Screen

- `screen -r {XX}` 

Reattach to an existing Screen. {XX} only when multiple Screens are open

- `str+alt+d`

Detach from a Screen
