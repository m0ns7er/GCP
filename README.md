# Kali linux on GCP

1. Add repo ```/etc/apt/source.list``` (https://www.kali.org/docs/general-use/kali-linux-sources-list-repositories/)
2. ```apt update```
3. ```gpg --keyserver pgpkeys.mit.edu --recv-key  ED444FF07D8D0BF6```
4. ```gpg -a --export ED444FF07D8D0BF6 | sudo apt-key add -```
   (If fails try```wget https://http.kali.org/kali/pool/main/k/kali-archive-keyring/kali-archive-keyring_2024.1_all.deb``` and
   sudo ```dpkg -i kali-archive-keyring_2024.1_all.deb```)
7. ```apt upgrade```
8. intsall metapackage (https://www.kali.org/docs/general-use/metapackages/)



# Chrome Remote Desktop:


```
sudo apt update
```
 
```
wget https://dl.google.com/linux/direct/chrome-remote-desktop_current_amd64.deb
```

```
sudo apt install ./chrome-remote-desktop_current_amd64.deb
```

Google Chrome:

```
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```

```
sudo apt install ./google-chrome-stable_current_amd64.deb
```
 
XFCE Desktop Environment:
 
```
sudo DEBIAN_FRONTEND=noninteractive \
apt install --assume-yes xfce4 desktop-base dbus-x11 xscreensaver

```

```
sudo bash -c 'echo "exec /etc/X11/Xsession /usr/bin/xfce4-session" > /etc/chrome-remote-desktop-session'

```
 
 
```
sudo systemctl disable lightdm.service
```

go to => https://remotedesktop.google.com/headless
