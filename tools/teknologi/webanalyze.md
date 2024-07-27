# webanalyze
Tool ini digunakan untuk menemukan teknologi yang digunakan oleh suatu web seperti web server, bahasa pemrograman, dan sebagainya

- Link download dan instalasi: https://github.com/rverton/webanalyze

## Instalasi
- Install menggunakan tool go
```sh
go install -v github.com/rverton/webanalyze/cmd/webanalyze@latest
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/webanalyze/analyze%201.JPG)

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/webanalyze /usr/bin
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/webanalyze/analyze%202.JPG)

- Update
```sh
webanalyze -update
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/webanalyze/analyze%203.JPG)

## Contoh Penggunaan
- Cara pemakaian
```sh
webanalyze -host <URL>
```
- Contoh pengujian pada web `http://testphp.vulnweb.com/`

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/webanalyze/analyze%204.JPG)

- Contoh pengujian pada web DVWA

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/webanalyze/analyze%205.JPG)

- Contoh pengujian pada API VAMPI

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/webanalyze/analyze%206.JPG)

- Pengujian di URL yang berbeda pada API VAMPI hasilnya tetap sama

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/webanalyze/analyze%207.JPG)