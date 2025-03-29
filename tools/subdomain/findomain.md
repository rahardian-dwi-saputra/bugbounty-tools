# Findomain
Tool ini digunakan untuk mencari sub domain dari suatu domain

- Link download dan instalasi: https://github.com/Findomain/Findomain/tree/master

## Instalasi
- Unduh file zip findomain
```sh
curl -LO https://github.com/findomain/findomain/releases/latest/download/findomain-linux-i386.zip
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/findomain/findomain%201.JPG)

- Unzip
```sh
unzip findomain-linux-i386.zip
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/findomain/findomain%202.JPG)

- Tambahkan permission execute pada file `findomain`
```sh
chmod +x findomain
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/findomain/findomain%203.JPG)

- Pindahkan file `findomain` ke direktori `/usr/bin` supaya findomain bisa diakses di direktori manapun
```sh
sudo mv findomain /usr/bin/findomain
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/findomain/findomain%204.JPG)

- Dokumentasi cara penggunaan tool `findomain` bisa dilihat dengan perintah berikut
```sh
findomain --help
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/findomain/findomain%205.JPG)

- Jika instalasi sudah berhasil, hapus file zip findomain
```sh
rm findomain-linux-i386.zip
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/findomain/findomain%206.JPG)

## Contoh Penggunaan
- Mencari subdomain dari 1 domain
```sh
findomain -t domain -r -u output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/findomain/findomain%207.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/findomain/findomain%208.JPG)

- Menghitung jumlah subdomain yang ditemukan
```sh
cat file_name | wc -l
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/findomain/findomain%209.JPG)