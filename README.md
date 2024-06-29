# Sonaric AI Node Kurulum
![image](https://pbs.twimg.com/media/GO0Ojjga4AAqFnm?format=jpg&name=4096x4096)

Minimum Sistem Gereksinimleri :
✅ 4 GB RAM
✅ 2 CPU cores
✅ 20 GB free disk space
✅ 64-bit operating system

### Linkler
[Explorer](https://tracker.sonaric.xyz/)
[Twitter](https://x.com/Sonaricnetwork)
[Twitter](discord.gg/MZ247hw47z)

## 🟢 Sistemi güncelleyelim
```shell
sudo apt update && \
sudo apt install curl git jq build-essential gcc unzip wget lz4 -y
```

## 🟢 Gerekli dosyayı yüklüyoruz ve izinleri verelim
```shell
wget https://raw.githubusercontent.com/aksamlan/Sonaric/main/sonaric.sh && chmod +x sonaric.sh && ./sonaric.sh
```

## 🟢 Yükleme bittikten sonra portları açalım
```shell
ufw allow 22
ufw allow ssh
sudo ufw allow 44004
```

## 🟢 Düğümünüzün Başarıyla Kurulup Kurulmadığını Kontrol Edin
```shell
sonaric node-info
```

## 🟢 GUI'yi çalıştırın
➖ Yerel terminalinizi açın
➖ "user@your-vps-ip" kendi IP'nizle değiştirin (örneğin: root@123.456.789)
```shell
ssh -L 127.0.0.1:44003:127.0.0.1:44003 -L 127.0.0.1:44004:127.0.0.1:44004 -L 127.0.0.1:44005:127.0.0.1:44005 -L 127.0.0.1:44006:127.0.0.1:44006 user@your-vps-ip
```
Girdikten sonra sunucu şifrenizi girip çalışıyor.

## 🟢 Sunucudaki bilgilerinizi yedekleyin
```shell
sonaric identity-export -o mysonaric.identity
```
## 🟢 Sunucuda puanlarınızı görmek için bu kodu girin
```shell
sonaric points
```

mysonaric.identity dosyasını güvenli bir yere kaydedin. Root klasörü içerisinde oluşmaktadır.

İŞLEMLERİMİZ BU KADARDI. TEŞEKKÜRLER...
