# katana
Tool ini digunakan untuk menemukan berbagai direktori web dari suatu website

- Link download dan instalasi: https://github.com/projectdiscovery/katana

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/projectdiscovery/katana/cmd/katana@latest
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%201.JPG)

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/katana /usr/bin
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%202.JPG)

- Dokumentasi cara penggunaan tool httpx bisa dilihat dengan perintah berikut
```sh
katana -h
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%203.JPG)

## Contoh Penggunaan
- Contoh pengujian pada web `http://testphp.vulnweb.com/`
```sh
katana -u url
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%204.JPG)

- Contoh pengujian pada web DVWA tanpa header

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%205.JPG)

- Contoh pengujian pada web DVWA dengan penambahan header cookie
```sh
katana -u url -H "Cookie: cookie_here"
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%206.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%207.JPG)

- Contoh pengujian pada API VAMPI

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%208.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%209.JPG)