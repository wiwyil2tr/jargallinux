# Jargal Linux
Based on Arch Linux with customized XFCE desktop, i3wm and calamares installer

## Extracting

The isos bigger than certain threshold are provided in multipart zip files because of the filesize restriction of github. To extract the iso, download all the zipped parts, and open the zip file with ``file-roller``, ``engrampa`` or ``7z``.

or run

```
cat jargal-2024.11.01-X86-64.iso.z** > jargal.zip
unzip jargal.zip

```

This should automatically extract the iso from all the files.

## Building 
### Extracting
run
```
cat archiso.tar.gz.part-* > archiso.tar.gz
tar -xvf archiso.tar.gz
git clone https://github.com/wiwyil2tr/jargal-build
mv archiso jargal-build
```
### building iso image
* See [alci](https://github.com/arch-linux-calamares-installer/alci-iso-zen)
  or [jargal-build](https://github.com/wiwyil2tr/jargal-build)

## Introduction

I integrated the configurations of XFCE, i3, zsh, vim, and ranger together, added xfce desktop and some commonly used software, and packaged them into an image based on Arch Linux. Originally, I planned to call it "optimized Arch", but later I felt that it did not comply with the KISS principle of Arch, so I renamed it Jargal Linux. This system can be installed using Calamares. I want to make a system that is easy to install and use right out of the box. 
![Screenshot_2024-11-01_13-02-46](https://github.com/user-attachments/assets/858a9b37-9ce0-4f1f-a17a-af2fd4799143)
![jargal1](https://github.com/user-attachments/assets/4f47ca29-4256-41a7-9934-70d7a0db1e1b)
* You can switch between xfwm4 and i3wm in xfce with shortcuts without logging out
`Super+Shift+i` switch to i3wm
`Super+Shift+x` switch to xfwm4
![jargal2](https://github.com/user-attachments/assets/0fec93d9-3eb1-4be5-9160-e2a102e1274f)
It also have configured zsh and vim, etc.
* It can be easily installed with Calamares Installer
![image](https://github.com/user-attachments/assets/6f605c24-c0b8-4b82-9655-1a1c64f191ce)
![Screenshot_20240113_210628](https://github.com/wiwyil2tr/jargallinux/assets/108447154/c9a21e0a-0f89-418f-870a-0418b346f145)

## Notice

There's no GUI when booting from livecd, you should manually run `systemctl start lightdm` to start it

## Download
To download it , see [Github Releases](https://github.com/wiwyil2tr/jargallinux/releases)


