# Subfinder
Tool ini digunakan untuk mencari sub domain dari suatu domain

- Link download dan instalasi: https://github.com/projectdiscovery/subfinder

- Instalasi
```sh
sudo apt install subfinder
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/subfinder/subfinder%201.JPG)

- Panduan penggunaan tool
```sh
subfinder --help
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/subfinder/subfinder%202.JPG)

- Pemakaian
```sh
subfinder -d domain -all -recursive -o subdomains2.txt
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/subfinder/subfinder%203.JPG)

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/subfinder/subfinder%204.JPG)

- Menghitung jumlah subdomain yang ditemukan
```sh
cat file_name | wc -l
```

![alt text](https://github.com/rahardian-dwi-saputra/bugbounty-tools/blob/main/assets/subfinder/subfinder%205.JPG)