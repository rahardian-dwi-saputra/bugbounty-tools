# httpx
Tool ini digunakan untuk menemukan teknologi yang digunakan oleh suatu web seperti web server, CMS, library JavaScript dan sebagainya

- Link download dan instalasi: https://github.com/projectdiscovery/httpx
- Dokumentasi: https://docs.projectdiscovery.io/tools/httpx/running

## Instalasi
- Install menggunakan tool go
```sh
go install -v github.com/projectdiscovery/httpx/cmd/httpx@latest
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%201.JPG)

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/httpx /usr/bin
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%202.JPG)

- Dokumentasi cara penggunaan tool httpx bisa dilihat dengan perintah berikut
```sh
httpx -h
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%203.JPG)

## Contoh Penggunaan
- Selain tool [httprobe](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/subdomain/httprobe.md) tool ini juga bisa digunakan untuk pengecekan sub-domain aktif
```sh
cat file_subdomain | httpx > output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%204.JPG)

- Dari hasil diatas, diperoleh 120 sub-domain aktif

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%205.JPG)

- Selain untuk pengecekan sub-domain aktif, tool ini bisa dipergunakan untuk pengecekan HTTP status code di tiap daftar sub-domain kemudian memfilter berdasarkan HTTP status code yang diberikan
```sh
cat file_subdomain | httpx -sc -mc 200,301,302 | tee output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%206.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%207.JPG)

- Melakukan pengecekan teknologi di tiap sub-domain yang aktif
```sh
cat output_file | httpx -td
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%208.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%209.JPG)

- Contoh pengujian pada web `http://testphp.vulnweb.com/` untuk mengetahui server dan teknologi yang digunakan di web tersebut
```sh
echo <URL> | httpx -server -td
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%2010.JPG)

- Contoh pengujian pada web DVWA

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%2011.JPG)

- Contoh pengujian pada API VAMPI

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%2012.JPG)