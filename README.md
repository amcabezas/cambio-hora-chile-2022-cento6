# Cambio de hora Centos 6 - Chile septiembre 2022
```
mkdir tzdata && cd tzdata 
wget https://data.iana.org/time-zones/releases/tzdata2022c.tar.gz
tar xvzf tzdata2022c.tar.gz
zic southamerica
ln -sf /usr/share/zoneinfo/America/Santiago /etc/localtime
zdump -v /etc/localtime | grep 2022
```
