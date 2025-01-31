# dirsearch
Tool ini digunakan untuk menemukan berbagai direktori web dari suatu website

- Link download dan instalasi: https://github.com/maurosoria/dirsearch

## Instalasi
- Jalankan perintah dibawah ini
```sh
pip3 install dirsearch
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dirsearch/dirsearch%201.JPG)

- Copy folder hasil instalasi ke `/usr/bin` supaya bisa diakses dimanapun
```sh
sudo cp .local/bin/dirsearch /usr/bin
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dirsearch/dirsearch%202.JPG)

- Dokumentasi cara penggunaan tool subzy bisa dilihat dengan perintah berikut
```sh
dirsearch -h
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dirsearch/dirsearch%203.JPG)

## Contoh Penggunaan
- Setelah mengumpulkan daftar live subdomain dengan tool [httpx](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/teknologi/httpx.md), sekarang kita bisa mengumpulkan daftar URL dari masing-masing live subdomain
```sh
dirsearch -l subdomain_file -x 300,301,400,404,403 -r -R 6 -o output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dirsearch/dirsearch%204.JPG)

Contoh pengujian pada web `http://testphp.vulnweb.com/`
```sh
dirsearch -u url -e conf,config,bak,backup,txt,php,cache,cgi,sql,sql.gz,sql.zip,js,json,log,csv,html,rar,tar,tar.gz,zip,xml -x 300,301,400,404,403 -r -R 6 -o testvulnurls2.txt
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dirsearch/dirsearch%205.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/dirsearch/dirsearch%206.JPG)
