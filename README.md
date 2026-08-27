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


if needed
```
export DISPLAY=:1
```


if needed
```
udroid install jammy:gnome
```
```
udroid login jammy:gnome
```

**Help**
**Main RIPO : https://github.com/RandomCoderOrg/ubuntu-on-andro**
