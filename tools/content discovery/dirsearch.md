# dirsearch
Tool ini digunakan untuk menemukan berbagai direktori web dari suatu website

- Link download dan instalasi: https://github.com/maurosoria/dirsearch

## Instalasi
- Jalankan perintah dibawah ini
```sh
pip3 install dirsearch
```

- Copy folder hasil instalasi ke `/usr/bin` supaya bisa diakses dimanapun
```sh
sudo cp .local/bin/dirsearch /usr/bin
```

- Dokumentasi cara penggunaan tool subzy bisa dilihat dengan perintah berikut
```sh
dirsearch -h
```

## Contoh Penggunaan
- Setelah mengumpulkan daftar live subdomain dengan tool [httpx](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/teknologi/httpx.md), sekarang kita bisa mengumpulkan daftar URL dari masing-masing live subdomain
```sh
dirsearch -l subdomain_file -x 300,301,400,404,403 -r -R 6 -o output_file
```

Contoh pengujian pada web `http://testphp.vulnweb.com/`
```sh
dirsearch -u url -e conf,config,bak,backup,txt,php,cache,cgi,sql,sql.gz,sql.zip,js,json,log,csv,html,rar,tar,tar.gz,zip,xml -x 300,301,400,404,403 -r -R 6 -o testvulnurls2.txt
```
