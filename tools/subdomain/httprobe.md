# httprobe
Tool ini digunakan untuk mengecek apakah subdomain aktif atau tidak

- Link download dan instalasi: https://github.com/tomnomnom/httprobe

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/tomnomnom/httprobe@latest
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%201.JPG)

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/httprobe /usr/bin
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%202.JPG)

- Dokumentasi cara penggunaan tool httprobe bisa dilihat dengan perintah berikut
```sh
httprobe --help
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%203.JPG)

## Contoh Penggunaan
- Sebelumnya menggunakan tool ini, anda disarankan untuk mengumpulkan sub domain dari suatu domain menggunakan tool untuk mencari sub domain seperti [subfinder](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/subdomain/subfinder.md) dan [sublist3r](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/subdomain/sublist3r.md)
- Berikut ini pengecekan sub domain aktif dari `google.com`
```sh
cat subdomains.txt | httprobe | tee live-domains.txt
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%204.JPG)

- Dari percobaan diatas diperoleh 45 sub domain yang aktif

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%205.JPG)