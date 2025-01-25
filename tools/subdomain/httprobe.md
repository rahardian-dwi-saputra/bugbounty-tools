# httprobe
Tool ini digunakan untuk mengecek apakah subdomain aktif atau tidak

- Link download dan instalasi: https://github.com/tomnomnom/httprobe

## Instalasi
- Install menggunakan tool go
```sh
go install github.com/tomnomnom/httprobe@latest
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%201.JPG)

- Copy ke folder `/usr/bin` supaya bisa digunakan dimana saja
```sh
sudo cp go/bin/httprobe /usr/bin
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%202.JPG)

- Dokumentasi cara penggunaan tool httprobe bisa dilihat dengan perintah berikut
```sh
httprobe --help
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%203.JPG)

## Contoh Penggunaan
- Sebelumnya menggunakan tool ini, anda disarankan untuk mengumpulkan sub domain dari suatu domain menggunakan beberapa tool dibawah ini:
	- [subfinder](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/subdomain/subfinder.md) 
	- [sublist3r](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/tools/subdomain/sublist3r.md)
- Setelah menggunakan 3 tools diatas, kita akan memperoleh 3 file yang berisi daftar sud-domain dengan jumlah yang berbeda

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%204.JPG)

- Gabungkan 3 file diatas dengan perintah berikut
```sh
sort -u file1 file2 file3 > output_filename
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%205.JPG)

- Hasil penggabungan menjadi 677 baris

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%206.JPG)

- Selanjutnya lakukan pengecekan live sub-domain menggunakan tool `httprobe`
```sh
cat subdomain_file | httprobe | tee output_filename
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%207.JPG)

- Dari percobaan diatas diperoleh 1116 sub domain yang aktif

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/httprobe/httprobe%208.JPG)