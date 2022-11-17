<div style='text-align: center'>
    <img src='images/logo.svg' width=20%/><br>
    <img src='https://img.shields.io/github/repo-size/Andrew-Flame/mnt?style=for-the-badge'/>
    <img src='https://img.shields.io/github/license/Andrew-Flame/mnt?color=%233FBA12&style=for-the-badge'><br>
</div>

# MNT
### Description
'mnt' is a program that allows you to quickly mount and unmount disk devices in Linux-based operating systems. It will allow you to save a lot of time when mounting disks in systems with or without a graphical environment.

### Installation
There is a ready-made script in the root directory of the repository that will install the program for you. You only need to run it and follow the instructions:
```BASH
git clone https://github.com/Andrew-Flame/mnt.git
chmod +x install
./install
```

### Customization
'mnt' is a configurable program. Location of the configuration file ~/.config/mnt.ini
You can configure:
- The name of the folder where each disk will be mounted. For this purpose, the file has a section '[associations]'. Example:
  ```INI
  [associations]
  Disk C = C
  Disk I = I
  Disk H = H
  ```
- The display of disks in the dialog window. Example
  ```INI
  # Default: ON
  Disk C = OFF
  Disk I = ON
  Disk H = ON
  ```
- Some other values:
  ```INI
  [general]
    # The language in which the program will be output.
    language = 'en'

    # The directory where the disks will be mounted.
    mountpoint = '/mnt'
  ```

### Dependencies
- whiptail