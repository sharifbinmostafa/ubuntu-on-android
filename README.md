# ubuntu-on-android
modified ubuntu on android installation 



Steps

'''
pkg update && pkg upgrade -y
'''
Then
'''
. <(curl -Ls https://github.com/sharifbinmostafa/ubuntu-on-android/blob/main/install.sh)
'''
Then
'''
udroid install jammy:xfce4
'''
clear
'''
pkg install x11-repo -y
'''
'''
pkg install termux-x11-nightly -y
'''

clear
'''
if not open display on termux-x11
'''
then
'''
termux-x11 :1 -ac &
'''

then 
'''
udroid login jammy:xfce4
'''
'''
startxfce4 &
'''
// NOW RUNNING OUR DISPLAY


if needed
'''
export DISPLAY=:1
'''


if needed
'''
udroid install jammy:gnome
'''
'''
udroid login jammy:gnome
'''


