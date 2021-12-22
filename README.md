# Monitoring_Zergpool
## Bash file monitoring wallet to telegram
![This is a alt text.](https://github.com/bayufrd/Monitoring_Zergpool/blob/main/image_2021-12-22_161618.png "Monitoring Zergpool.")
##### fitur
* auto retry jika gagal mendapatkan api, sampai dapat.

##### Install apk JQ
```
sudo apt install jq
```

#### Cara Install
* Buka terminal linux lalu jalankan
```
wget -L https://raw.githubusercontent.com/bayufrd/Monitoring_Zergpool/main/stat.sh
```

* Edit file stat.sh dengan nano
```
nano stat.sh
```
* Bisa dirubah bagian ini ganti milik kalian

![This is a alt text.](https://github.com/bayufrd/Monitoring_Zergpool/blob/main/image_2021-12-23_031237.png "Silahkan diganti.")

* Bagi yang belum mengerti untuk mendapatkan ID Telegram dan TOKEN BOT nya bisa akses link berikut:

[ID Telegram](https://qastack.id/programming/32423837/telegram-bot-how-to-get-a-group-chat-id).

[TOKEN BOT](https://langsungviral.com/2019/12/04/cara-mendapatkan-api-key-atau-token-bot-telegram-dan-chat-id-telegram/).

* Save dan Keluar >> (Ctrl + X) lalu Y, Enter.
* Tambah kan pengijinan untuk akses file
```
chmod +x stat.sh
```

* Untuk mengetest nya bisa jalankan dengan

```
./stat.sh
```

* Untuk membuatnya auto dijalankan bisa menambahkan sedikit script ke crontab

```
sudo crontab -e
0 * * * * bash /root/stat.sh > /root/stat.log 2>&1
```

* bisa dirubah sesuai keinginan, jika ingin dijalankan per10 menit dapat diganti menjadi:

```
*/10 * * * * bash /root/stat.sh > /root/stat.log 2>&1
```

Selesai =))

## Sumber
[API ZERGPOOL](https://zergpool.com/site/api).

## Bug
```
[Solved] Sometimes error at reading total hashrate, cz im writin' code manual, total hashrate not available at api pool. Will solved as soon as posible =D "kalo ga mager"
```

# Donasi
* DOGE  : D8QyZTdUo6jLpx3RVj6pwbCmgeVh6pC59m
* SKY   : 2gkeczcbPXSWUNKBzNVHoXbmBvqKEmQV5Gz
* VRSC  : -
* BNB   : 0x89d5cfdbc82d6a768d2279ba04b2dffeeb6b50e1
