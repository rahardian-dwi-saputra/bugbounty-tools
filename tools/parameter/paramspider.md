# ParamSpider
Tool ini digunakan untuk mengumpulkan URL yang mengandung parameter dari suatu domain website. URL ini nantinya bisa digunakan untuk pengujian XSS dan SQL Injection

- Link download dan instalasi: https://github.com/devanshbatham/ParamSpider

## Instalasi
- Jalankan satu per satu perintah dibawah ini
```sh
git clone https://github.com/devanshbatham/paramspider
cd paramspider
pip install .
```

## Contoh Penggunaan
```sh
paramspider -d <domain>
```
- Hasil akan tersimpan otomatis dalam folder **results**
```sh
cat results/nama_file
```