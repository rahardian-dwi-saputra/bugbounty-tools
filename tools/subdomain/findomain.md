# Findomain
Tool ini digunakan untuk mencari sub domain dari suatu domain

- Link download dan instalasi: https://github.com/Findomain/Findomain/tree/master

## Instalasi
- Unduh file zip findomain
```sh
curl -LO https://github.com/findomain/findomain/releases/latest/download/findomain-linux-i386.zip
```

- Unzip
```sh
unzip findomain-linux-i386.zip
```

- Tambahkan permission execute pada file `findomain`
```sh
chmod +x findomain
```

- Pindahkan file `findomain` ke direktori `/usr/bin` supaya findomain bisa diakses di direktori manapun
```sh
sudo mv findomain /usr/bin/findomain
```


- Dokumentasi cara penggunaan tool `findomain` bisa dilihat dengan perintah berikut
```sh
findomain --help
```

- Jika instalasi sudah berhasil, hapus file zip findomain
```sh
rm findomain-linux-i386.zip
```

## Contoh Penggunaan
- Mencari subdomain dari 1 domain
```sh
findomain -t domain -r -u output_file
```


- Menghitung jumlah subdomain yang ditemukan
```sh
cat file_name | wc -l
```


