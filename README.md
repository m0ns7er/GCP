# Kali linux on GCP

1. Add repo ```/etc/apt/source.list``` (https://www.kali.org/docs/general-use/kali-linux-sources-list-repositories/)
2. ```apt update```
3. ```gpg --keyserver pgpkeys.mit.edu --recv-key  ED444FF07D8D0BF6```
4. ```gpg -a --export ED444FF07D8D0BF6 | sudo apt-key add -```
   (If fails try```wget http://http.kali.org/kali/pool/main/k/kali-archive-keyring/kali-archive-keyring_2022.1_all.deb``` and
   sudo ```dpkg -i kali-archive-keyring_2022.1_all.deb```)
7. ```apt upgrade```
8. intsall metapackage (https://www.kali.org/docs/general-use/metapackages/)



