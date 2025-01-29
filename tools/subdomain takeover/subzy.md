# Subzy
Tool ini digunakan untuk mengecek apakah ada kerentanan subdomain takeover atau tidak

- Link download dan instalasi: https://github.com/PentestPad/subzy

## Instalasi
- Install menggunakan tool go
```sh
go install -v github.com/PentestPad/subzy@latest
```

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/subzy /usr/bin
```

- Dokumentasi cara penggunaan tool subzy bisa dilihat dengan perintah berikut
```sh
subzy --help
```


## Contoh Penggunaan
- Sebelum menggunakan tool ini, kumpulkan daftar subdomain terlebih dahulu menggunakan tool [assetfinder](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/subdomain/assetfinder.md), [subfinder](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/subdomain/subfinder.md), [sublist3r](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/subdomain/sublist3r.md)
```sh
subzy run --targets nama_file
```

