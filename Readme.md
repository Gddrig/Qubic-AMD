
# Repo outdated, please go [here](https://github.com/Gddrig/Qubic_Hiveos) (https://github.com/Gddrig/Qubic_Hiveos)

**!! TUTO RQINER 0.4.1 ( EPOCH 104)  for AMD GPU !!** ( AMD RX série 6000 et 7000 )
**!! For HiveOs 6.1 !!**

**Update your system :**
```sh
apt update && apt install unzip g++ gcc  -y
```
**Install ROCM 5.7 for Hiveos :**
```sh
amd-ocl-install 5.7 5.7
```

**Install lib Zluda :**
```sh
mkdir /usr/lib/zluda && cd /usr/lib/zluda && wget https://github.com/Gddrig/Qubic-AMD/releases/download/3.22/zluda_hiveos-6.1.zip && unzip zluda_hiveos-6.1.zip && chmod +rwx /usr/lib/zluda/* && cd /
```

**Install lib ROCM :**
```sh
cd /opt/rocm/lib && wget https://github.com/Gddrig/Qubic-AMD/releases/download/3.22/libamdhip64.so.zip && unzip libamdhip64.so.zip && chmod +rwx /opt/rocm/lib/* && rm libamdhip64.so.zip && cd / && ldconfig
```

**If error glibc/lib6 :**
```sh
apt update && echo "deb http://cz.archive.ubuntu.com/ubuntu jammy main" >> /etc/apt/sources.list && apt update && apt install tmux -y && apt install libc6 -y
```

**If error glibcxx :**
```sh
apt install g++-11
```

![alt text](https://github.com/Gddrig/Qubic-AMD/blob/main/Capture.PNG)

Based on the work of  **ViporLab** : https://downloads.viporlab.net/#/


To support my work, Qubic : CZBJCMAWKIBLEHVJPAWERRNVKKNAXUSPMJIYZXCKYCGJSWNMUGCJPLCEEGKE
