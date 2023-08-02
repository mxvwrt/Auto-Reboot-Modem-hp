
# Auto Reboot Modem hp

Keperluan : Optimasi Modem Hp OpenWRT Yang Belum Di root


# Instalasi
## Step 1

Copy Kode Dibawah Ini

```bash
wget -O /bin/ngreboot_hp "https://raw.githubusercontent.com/mxvwrt/Auto-Reboot-Modem-hp/main/ngreboot_hp" && chmod +x /bin/ngreboot_hp  
```
 ## Step 2

Pergi Ke Luci -> System -> Scheduled Tasks, Lalu Sesuai Keinginan Jadwal Untuk Reboot, Contoh :
```bash
0 3 * * * /bin/ngreboot_hp >/dev/null 2>&1
```   
untuk lebih jelas tentang crontab bisa ke Link Berikut 
[Link Berikut](https://crontab.guru/)

