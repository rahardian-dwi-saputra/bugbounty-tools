# XSpear
Tool ini digunakan untuk menemukan kerentanan XSS Reflected pada suatu URL di website

- Link download dan instalasi: https://github.com/hahwul/XSpear

## Pengujian pada website http://testphp.vulnweb.com/
- Gunakan tool Paramspider terlebih dahulu untuk mengumpulkan daftar URL yang bisa digunakan untuk pengujian XSS Reflected
```sh
XSpear -u "URL" -v 0
```
- Akses tiap URL yang mengandung payload di browser untuk mengecek kerentanan XSS Reflected