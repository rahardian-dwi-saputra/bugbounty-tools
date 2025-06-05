# hakrawler
Tool ini digunakan untuk menemukan berbagai direktori web dari suatu website

- Link download dan instalasi: https://github.com/hakluke/hakrawler

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/hakluke/hakrawler@latest
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%201.JPG)

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo mv go/bin/hakrawler /usr/bin
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%202.JPG)

- Dokumentasi cara penggunaan tool httpx bisa dilihat dengan perintah berikut
```sh
hakrawler -h
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%203.JPG)

## Contoh Penggunaan
- Setelah mengumpulkan daftar live subdomain dengan tool [httpx](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/teknologi/httpx.md), sekarang kita bisa mengumpulkan daftar URL dari masing-masing live subdomain
```sh
katana -u nama_file -d 5 -ef woff,css,png,svg,jpg,jpeg,gif,woff2 -o output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%204.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%205.JPG)

- Dari proses diatas, berhasil dikumpulkan 1778 URL

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%206.JPG)

- Contoh pengujian pada web `http://testphp.vulnweb.com/`
```sh
katana -u URL -d 5 -ef woff,css,png,svg,jpg,woff2,jpeg,gif -ps -pss waybackarchive,commoncrawl,alienvault -jc -fx -o output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%207.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%208.JPG)

- Dari proses diatas, berhasil dikumpulkan 15386 URL

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%209.JPG)

- Memfilter URL javascript
```sh
cat url_file | grep -E "\.js$" >> output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%2010.JPG)

- Memfilter URL yang mengandung parameter
```sh
cat url_file | grep "="
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%2011.JPG)

- Memfilter URL dengan format tertentu
```sh
cat url_file | grep -E "\.txt|\.log|\.cache|\.secret|\.db|\.backup|\.bak|\.json|\.yml|\.rar|\.cgi|\.sql|\.config|\.conf|\.tar|\.tar.gz|\.zip|\.xml|\.csv"
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%2012.JPG)

- Contoh pengujian pada web DVWA tanpa header

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%2013.JPG)

- Contoh pengujian pada web DVWA dengan penambahan header cookie
```sh
katana -u url -H "Cookie: cookie_here"
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%2014.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%2015.JPG)

- Contoh pengujian pada API VAMPI

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%2016.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/katana/katana%2017.JPG)