# httpx
Tool ini digunakan untuk menemukan teknologi yang digunakan oleh suatu web seperti web server, CMS, library JavaScript dan sebagainya

- Link download dan instalasi: https://github.com/projectdiscovery/httpx

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
- Tool ini bisa dikombinasikan dengan tool pencari sub domain seperti `sublist3r`
```sh
sublist3r -d domain -o output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%204.JPG)

- Melakukan pengecekan status di tiap sub domain
```sh
cat output_file | httpx -sc
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%205.JPG)

- Melakukan pengecekan teknologi di tiap sub domain
```sh
cat output_file | httpx -td
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httpx/httpx%206.JPG)