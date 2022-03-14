# Kali linux on GCP

1. Add repo /etc/apt/source.list (https://www.kali.org/docs/general-use/kali-linux-sources-list-repositories/)
2. apt update
3. gpg --keyserver pgpkeys.mit.edu --recv-key  ED444FF07D8D0BF6
4. gpg -a --export ED444FF07D8D0BF6 | sudo apt-key add -
5. apt upgrade
6. intsall metapackage (https://www.kali.org/docs/general-use/metapackages/)



