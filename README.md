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


**Help**
**Main RIPO : https://github.com/RandomCoderOrg/ubuntu-on-andro**
** also : https://docs.udroid.org/**
