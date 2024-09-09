# waybackurls
Tool ini digunakan untuk mengumpulkan link aktif dari suatu website yang berada di internet

- Link download dan instalasi: https://github.com/tomnomnom/waybackurls

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/tomnomnom/waybackurls@latest
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/waybackurls/waybackurls%201.JPG)

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/waybackurls /usr/bin
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/waybackurls/waybackurls%202.JPG)

- Dokumentasi cara penggunaan tool httprobe bisa dilihat dengan perintah berikut
```sh
waybackurls --help
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/waybackurls/waybackurls%203.JPG)

## Contoh Penggunaan
- Sebelumnya menggunakan tool ini, anda disarankan untuk mengumpulkan daftar domain yang aktif menggunakan tool httprobe
- Berikut ini pengecekan link dari live domain aktif dari `google.com`
```sh
cat live-domains.txt | waybackurls > urls
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/waybackurls/waybackurls%204.JPG)

- Dari percobaan diatas diperoleh 2.086.496 link yang aktif

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/waybackurls/waybackurls%205.JPG)