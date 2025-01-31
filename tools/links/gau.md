# getallurls (gau)
Tool ini digunakan untuk mengumpulkan link aktif dari suatu website yang berada di Wayback Machine

- Link download dan instalasi: https://github.com/lc/gau

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/lc/gau/v2/cmd/gau@latest
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%201.JPG)

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo mv go/bin/gau /usr/bin
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%202.JPG)

- Dokumentasi cara penggunaan tool httprobe bisa dilihat dengan perintah berikut
```sh
gau -h
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%203.JPG)

- Download file konfigurasi gau, file ini harus berada di direktori `/home/nama_user/`
```sh
wget https://raw.githubusercontent.com/lc/gau/refs/heads/master/.gau.toml
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%204.JPG)

## Contoh Penggunaan
- Setelah mengumpulkan daftar live subdomain dengan tool [httpx](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/teknologi/httpx.md), sekarang kita bisa mengumpulkan daftar URL dari masing-masing live subdomain yang berada di wayback machine.
```sh
cat live-subdomains-file | gau --fc 400,404 --o output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%205.JPG)

- Dari percobaan diatas diperoleh 9.470.125 link yang aktif

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%206.JPG)

- Contoh pengujian pada web `http://testphp.vulnweb.com/`
```sh
gau --fc 400,404 --o output_file URL
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%207.JPG)

- Pada web `http://testphp.vulnweb.com/` ditemukan 11.117 link

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%208.JPG)

- Memfilter URL javascript
```sh
cat output_file | grep -E "\.js$"
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%209.JPG)

- Memfilter URL dengan format tertentu
```sh
cat output_file | grep -E "\.txt|\.log|\.cache|\.secret|\.db|\.backup|\.bak|\.json|\.yml|\.rar|\.cgi|\.sql|\.config|\.conf|\.tar|\.tar.gz|\.zip|\.xml|\.csv"
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%2010.JPG)

- Memfilter URL yang mengandung parameter
```sh
cat output_file | grep "?*="
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/gau/gau%2011.JPG)