# XSpear
Tool ini digunakan untuk menemukan kerentanan XSS Reflected pada suatu URL di website

- Link download dan instalasi: https://github.com/hahwul/XSpear

## Instalasi
- Jalankan satu per satu perintah dibawah ini untuk menginstall dependensi
```sh
gem install colorize
gem install selenium-webdriver
gem install terminal-table
gem install progress_bar
```
- Install tool XSpear
```sh
gem install XSpear
```
- Dokumentasi cara penggunaan tool XSpear bisa dilihat dengan perintah berikut
```sh
gem install XSpear
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/xspear/xspear%201.JPG)

## Contoh Penggunaan
- Gunakan tool [Paramspider](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/parameter/paramspider.md) terlebih dahulu untuk mengumpulkan daftar URL yang bisa digunakan untuk pengujian XSS Reflected pada web http://testphp.vulnweb.com/
- Pilih salah satu URL yang akan diuji
```sh
XSpear -u "URL" -v 0
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/xspear/xspear%202.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/xspear/xspear%203.JPG)

- Akses tiap URL yang mengandung payload di browser untuk mengecek kerentanan XSS Reflected

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/xspear/xspear%204.JPG)