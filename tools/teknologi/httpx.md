# httpx
Tool ini digunakan untuk menemukan teknologi yang digunakan oleh suatu web seperti web server, CMS, library JavaScript dan sebagainya

- Link download dan instalasi: https://github.com/projectdiscovery/httpx

## Instalasi
- Install menggunakan tool go
```sh
go install -v github.com/projectdiscovery/httpx/cmd/httpx@latest
```

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/httpx /usr/bin
```

- Dokumentasi cara penggunaan tool httpx bisa dilihat dengan perintah berikut
```sh
httpx -h
```

## Contoh Penggunaan
- Tool ini bisa dikombinasikan dengan tool pencari sub domain seperti `sublist3r`
```sh
sublist3r -d domain -o output_file
```

- Melakukan pengecekan status di tiap sub domain
```sh
cat output_file | httpx -sc
```

- Melakukan pengecekan teknologi di tiap sub domain
```sh
cat output_file | httpx -td
```
