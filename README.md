# Nedir bu bot?
Ac3 veya eac3 ses format�yla kodlanm�� yani telegram�n destek vermedi�i hi� sesi olmayan Telegram videolar�n�n sesini ffmpeg arac�l���yla acc format�na d�n��t�r�p sesin gelmesini sa�lar ve bunu herhangi bir kalite olmadan yapar.

�al��an bir �rnek: [Video Sesini D�n��t�r](https://t.me/SesVideoBot)

### Ortam De�i�kenleri
Ortam de�i�kenlerine de�erler ekleyin veya bunlar� [config.env](./config.env) i�ine ekleyin.
- `API_ID` - [https://my.telegram.org](https://my.telegram.org)'da bir uygulama olu�turarak edinin.
- `API_HASH` - [https://my.telegram.org](https://my.telegram.org)'da bir uygulama olu�turarak edinin.
- `BOT_TOKEN` - [https://t.me/BotFather](https://t.me/BotFather) adresinden bir bot olu�turarak edinin.
- `SUDO_USERS` - Yetkili kullan�c�n�n ID numaras�n� ekleyin. Birden fazla kullan�c� i�in ay�r�c� olarak bo�uk kullan�n.
- `DOWNLOAD_DIR` - (�ste�e ba�l�) �ndirilen dosyalar� saklamak i�in ge�ici indirme dizini. Varsay�lan 'indirilenler/'

### Kodlama Bi�imini Yap�land�rma
ffmpeg profilini de�i�tirmek istiyorsan�z bunlar� �urada d�zenleyin: [ffmpeg_utils.py](/bot/helper/ffmpeg_utils.py)

## Kolay Kurulum:
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)


### Kurulum Gereksinimleri
Makinenize gerekli Python Mod�llerini kurun.
```sh
apt-get -qq install ffmpeg
pip3 install -r requirements.txt
```
### Da��tma
Python3.7 veya �st� ile.
```sh
python3 -m bot
```