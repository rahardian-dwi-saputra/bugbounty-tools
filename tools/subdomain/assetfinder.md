# assetfinder
Tool ini digunakan untuk mencari sub domain dari suatu domain

- Link download dan instalasi: https://github.com/tomnomnom/assetfinder

- Instalasi
```sh
sudo apt install assetfinder
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/assetfinder/af%201.JPG)

- Panduan penggunaan tool
```sh
assetfinder --help
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/assetfinder/af%202.JPG)

- Pemakaian
```sh
assetfinder -subs-only domain > output_file
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/assetfinder/af%203.JPG)

- Menghitung jumlah subdomain yang ditemukan
```sh
cat file_name | wc -l
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/assetfinder/af%204.JPG)