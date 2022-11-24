<div align=center style='text-align: center'>
    <img src='/images/logo.svg' width=20%/><br>
    <img src='https://img.shields.io/github/repo-size/Andrew-Flame/mnt?style=for-the-badge'/>
    <img src='https://img.shields.io/github/v/release/Andrew-Flame/mnt?style=for-the-badge'/>
    <img src='https://img.shields.io/github/license/Andrew-Flame/mnt?color=%230CD94E&style=for-the-badge'/><br>
    [English]
    [<a href='/docs/README-RU.MD'>Русский</a>]
</div>

# MNT
### Description
'mnt' is a program that allows you to quickly mount and unmount disk devices in Linux-based operating systems. It will allow you to save a lot of time when mounting disks in systems with or without a graphical environment.

### Usage
Everything you need to do to use 'mnt':
1) Call the program from the terminal
2) Mark the disks that should be mounted and uncheck those that you want to unmount
3) Press the 'OK' button in the whiptail window or the 'Enter' key on the keyboard

It's incredibly simple and quick, and will also help you save a lot of time!

![mnt](https://user-images.githubusercontent.com/82677442/203862003-0da65345-417c-4193-9d4a-e344ad100ab4.gif)

### Installation
There is a ready-made script in the root directory of the repository that will install the program for you. You only need to run it and follow the instructions:
```BASH
git clone https://github.com/Andrew-Flame/mnt.git
cd mnt
chmod +x install
./install
```

### Dependencies
- whiptail
- sudo

### Customization
'mnt' is a configurable program. Location of the configuration file ~/.config/mnt.ini
You can configure:
- The name of the folder where each disk will be mounted. Section '[associations]':
  ```INI
  [associations]
  Disk C = C
  Disk I = I
  Disk H = H
  ```
- The display of disks in the dialog window. Section '[display]':
  ```INI
  [display]
  # Default: ON
  Disk C = OFF
  Disk I = ON
  Disk H = ON
  ```
- Some other values. Section '[general]':
  ```INI
  [general]
  # The language in which the program will be output.
  language = 'en'

  # The directory where the disks will be mounted.
  mountpoint = '/mnt'
  ```