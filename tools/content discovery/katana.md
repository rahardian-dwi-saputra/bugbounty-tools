# katana
Tool ini digunakan untuk menemukan berbagai direktori web dari suatu website

- Link download dan instalasi: https://github.com/projectdiscovery/katana

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/projectdiscovery/katana/cmd/katana@latest
```


- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/katana /usr/bin
```

- Dokumentasi cara penggunaan tool httpx bisa dilihat dengan perintah berikut
```sh
katana -h
```


## Contoh Penggunaan
- Contoh pengujian pada web `http://testphp.vulnweb.com/`
```sh
katana -u url
```

- Contoh pengujian pada web DVWA tanpa header


- Contoh pengujian pada web DVWA dengan penambahan header cookie
```sh
katana -u url -H "Cookie: cookie_here"
```

- Contoh pengujian pada API VAMPI