# dalfox
Tool ini digunakan untuk menemukan kerentanan XSS Reflected pada suatu URL di website

- Link download dan instalasi: https://github.com/hahwul/dalfox

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/hahwul/dalfox/v2@latest
```
- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo mv go/bin/dalfox /usr/bin
```
- Dokumentasi cara penggunaan tool httprobe bisa dilihat dengan perintah berikut
```sh
dalfox -h
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dalfox/dalfox%201.JPG)

## Contoh Penggunaan
- Gunakan tool [Paramspider](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/parameter/paramspider.md) terlebih dahulu untuk mengumpulkan daftar URL yang bisa digunakan untuk pengujian XSS Reflected pada web http://testphp.vulnweb.com/
```sh
dalfox file url_file -b hawhul.xss.ht
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dalfox/dalfox%202.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dalfox/dalfox%203.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dalfox/dalfox%204.JPG)

- Akses tiap URL yang mengandung payload di browser untuk mengecek kerentanan XSS Reflected

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dalfox/dalfox%205.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dalfox/dalfox%206.JPG)