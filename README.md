# p1_manutencao

:nut_and_bolt: Troubleshooting regarding the maintenance of machines with Linux and Windows OS. :hammer_and_wrench:

## My Linux has a problem, it does not open the browser and I need to download the ISO

No problem use snap to install ubuntu-iso-download :

```
sudo snap install ubuntu-iso-download --edge
```

Once downloaded:

```
sudo apt update && sudo apt updrade -y
cd ~ && ubuntu-iso-download desktop
```

Later if you need to update the program use:

```
sudo snap refresh ubuntu-iso-download
```

If you need to uninstall:

```
sudo snap remove ubuntu-iso-download
```

## Problem creating bootable pendrive, I can't create it with Windows OS

Undoubtedly, throughout the life of an IT student, at least once the situation happened in which a friend or even a family member came to you with the intention of solving some software maintenance and installation problem and you with your Linux from a can of beer searched the web for a solution to create a Bootable Pendrive for another OS such as Windows, which is quite annoying to create an image. Well, 1 solution that I always use, and it never let me down was [WoeUSB-ng](https://github.com/WoeUSB/WoeUSB-ng) , the reason why it is very useful is that it already that it is created using python, every system easily and without much effort runs it.

### Installing WoeUSB-ng on your Linux machine

Taking into account that any Linux machine already comes with python 3 installed, if it didn't come with pip:

```
sudo apt install python3-pip && pip3 --version
```

Downloading the required dependencies and installing:

```
sudo apt install git p7zip-full python3-pip python3-wxgtk4.0 grub2-common grub-pc-bin && sudo pip3 install WoeUSB-ng
```

Now if everything works correctly, just send a bullet, open the program, and make the pendrive bootable.

**Note**: It is worth remembering that from base to Fedora what changes:

```
sudo dnf install git p7zip p7zip-plugins python3-pip python3-wxpython4 && sudo pip3 install WoeUSB-ng
```
