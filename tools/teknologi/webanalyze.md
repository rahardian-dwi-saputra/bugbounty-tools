# webanalyze
Tool ini digunakan untuk menemukan teknologi yang digunakan oleh suatu web seperti web server, bahasa pemrograman, dan sebagainya

- Link download dan instalasi: https://github.com/rverton/webanalyze

## Instalasi
- Install menggunakan tool go
```sh
go install -v github.com/rverton/webanalyze/cmd/webanalyze@latest
```

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/webanalyze /usr/bin
```

- Update
```sh
webanalyze -update
```

## Contoh Penggunaan
- Cara pemakaian
```sh
webanalyze -host <URL>
```
- Contoh pengujian pada web `http://testphp.vulnweb.com/`

- Contoh pengujian pada web DVWA

- Contoh pengujian pada API VAMPI

- Pengujian di URL yang berbeda pada API VAMPI hasilnya tetap sama