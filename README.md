This is an extension for Drive Badger. It provides `exclude.list` file, containing a list of exclusions compatible with popular `rsync` program.

The purpose of these exclusions is to decrease the amount of data to be exfiltrated by Drive Badger, and thus to speed up the attack,
by eliminating files and directories, that are not valuable in any way to the attacker:

- VMDK files (images of VMware virtual drives)
- ISO images

### Installing

Clone this repository as `/opt/drivebadger/config/exclude-virtual` directory on your Drive Badger persistent partition.

When you install this extension, you should also install [`hook-virtual`](https://github.com/drivebadger/hook-virtual)
hook - otherwise you will exclude all VMware virtual drives without exfiltrating them from inside.


### More information

- [Drive Badger main repository](https://github.com/drivebadger/drivebadger)
- [Drive Badger wiki](https://github.com/drivebadger/drivebadger/wiki)
- [description, how configuration repositories work](https://github.com/drivebadger/drivebadger/wiki/Configuration-repositories)
