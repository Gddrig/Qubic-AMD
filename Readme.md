**!! TUTO RQINER pour AMD !!** ( AMD RX série 6000 et 7000 )
**!! Pour HiveOs 6.1 !!**

apt install unzip g++ gcc  -y

amd-ocl-install 5.7 5.7

**Installation lib Zluda :**
mkdir /usr/lib/zluda && cd /usr/lib/zluda && wget https://github.com/Gddrig/Qubic-AMD/releases/download/3.22/zluda_hiveos-6.1.zip && unzip zluda_hiveos-6.1.zip && chmod +rwx /usr/lib/zluda/* && cd /

**Installation lib ROCM :**
cd /opt/rocm/lib && wget https://github.com/Gddrig/Qubic-AMD/releases/download/3.22/libamdhip64.so.zip && unzip libamdhip64.so.zip && chmod +rwx /opt/rocm/lib/* && rm libamdhip64.so.zip && cd / && ldconfig

**Si erreur Glib :**
apt update && echo "deb http://cz.archive.ubuntu.com/ubuntu jammy main" >> /etc/apt/sources.list && apt update && apt install tmux -y && apt install libc6 -y

**Si erreur Glibcxx :**
apt install g++-11

![alt text](https://github.com/Gddrig/Qubic-AMD/blob/main/Capture.PNG)

Basé sur le travail de **ViporLab** : [https://downloads.viporlab.net/#/](url)
