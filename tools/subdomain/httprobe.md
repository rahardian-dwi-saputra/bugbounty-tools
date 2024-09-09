# httprobe
Tool ini digunakan untuk mengecek apakah subdomain aktif atau tidak

- Link download dan instalasi: https://github.com/tomnomnom/httprobe

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/tomnomnom/httprobe@latest
```


- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/httprobe /usr/bin
```


- Dokumentasi cara penggunaan tool httprobe bisa dilihat dengan perintah berikut
```sh
httprobe --help
```

## Contoh Penggunaan
- Sebelumnya menggunakan tool ini, anda disarankan untuk mengumpulkan sub domain dari suatu domain menggunakan tool untuk mencari sub domain seperti [subfinder](tools/subdomain/subfinder.md) dan [sublist3r](tools/subdomain/sublist3r.md)
- Berikut ini pengecekan sub domain aktif dari `google.com`
```sh
cat subdomains.txt | httprobe | tee live-domains.txt
```

- Dari percobaan diatas diperoleh 45 sub domain yang aktif
