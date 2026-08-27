# ubuntu-on-android
modified ubuntu on android installation 

**Here we USE 2 Android Application:**
```
1. Termux
```
```
2. Termux-x11
```

**URL:**
```
1. https://f-droid.org/en/packages/com.termux/
```
```
2. https://github.com/termux/termux-x11/releases/tag/nightly
```

**Video Help URL:**
```
https://youtu.be/ONlPYrN4UHQ
```

**Setup Steps**

```
pkg update && pkg upgrade -y
```
Then
```
. <(curl -Ls https://raw.githubusercontent.com/sharifbinmostafa/ubuntu-on-android/refs/heads/main/install.sh)
```
Then
```
udroid install jammy:xfce4
```
clear
```
pkg install x11-repo -y
```
```
pkg install termux-x11-nightly -y
```

clear
```
if not open display on termux-x11
```
then
```
termux-x11 :1 -ac &
```

then 
```
udroid login jammy:xfce4
```
```
startxfce4 &
```
**NOW RUNNING OUR DISPLAY**


**If you want to remove Distro**
```
udroid remove jammy:xfce4
udroid --clear-cache
```



**Setting up VNC**
```
tigervncserver \
    -geometry 2560x1080 \
    -xstartup /usr/bin/xfce4-session \
    -listen tcp :1 
```

**Display over other devices**
```
tigervncserver \
    -geometry 2560x1080 \
    -localhost no \
    -xstartup /usr/bin/xfce4-session \
    -listen tcp :1 
```


if needed
```
export DISPLAY=:1
```

**OS SUITE Type**

```
udroid install jammy:gnome
```
```
udroid login jammy:gnome
```
```
udroid install jammy:xfce4
```
```
udroid login jammy:xfce4
```

For the complete documentation index, see llms.txt. This page is also available as Markdown.

Copy

🛸udroid-landing
🐧
udroid
udroid Documentation & details

Ubuntu on android

Ubuntu-on-android aims to run ubuntu with pre-installed Desktop Environment, development tools, and software on top of android without root with the help of proot in termux application. This project is just like any other Linux on android projects but with aim of making it easy for end-user on setting up Linux.

codename = udroid

img2 Support Server 

Quick Install
Install all dependencies and developer-selected Distro


Copy
. <(curl -Ls https://bit.ly/udroid-installer)
Android app
An experimental uDroid Android app is in early development. It provides a graphical way to install and manage Linux systems, use the terminal and X11 display, and launch installed Linux applications.

**SUITE Screenshots**
jammy:gnome
<img width="2257" height="1080" alt="image" src="https://github.com/user-attachments/assets/39898817-cb49-429d-b1e2-170ac9a0350a" />

jammy:xfce4
<img width="2292" height="1080" alt="image" src="https://github.com/user-attachments/assets/6918f510-b8d7-4562-b207-11508d7597bb" />

jammy:mate
<img width="2289" height="1077" alt="image" src="https://github.com/user-attachments/assets/f2a5a866-9bc4-4cae-ae67-e44446480eb1" />



**Help**
**Main RIPO : https://github.com/RandomCoderOrg/ubuntu-on-andro**
** also : https://docs.udroid.org/**
