# waybackurls
Tool ini digunakan untuk mengumpulkan link aktif dari suatu website yang berada di internet

- Link download dan instalasi: https://github.com/tomnomnom/waybackurls

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/tomnomnom/waybackurls@latest
```


- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/waybackurls /usr/bin
```


- Dokumentasi cara penggunaan tool httprobe bisa dilihat dengan perintah berikut
```sh
waybackurls --help
```

## Contoh Penggunaan
- Sebelumnya menggunakan tool ini, anda disarankan untuk mengumpulkan daftar domain yang aktif menggunakan tool httprobe
- Berikut ini pengecekan link dari live domain aktif dari `google.com`
```sh
cat live-domains.txt | waybackurls > urls
```

- Dari percobaan diatas diperoleh 2.086.496 link yang aktif
