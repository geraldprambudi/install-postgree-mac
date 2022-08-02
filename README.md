# Cara Install Postgree Mac Os

Ada 2 option untuk instalasinya yang pertama menggunakan brew dan yang kedua menggunakan postgree dari official website

Saya memilih menggunakan postgree melalui website, agak nyesel ternyata lebih mudah pake brew kwkwkw tapi yaudalah ya kwkw

# Download Postgree 
https://www.postgresql.org/download/macosx/

Seperti biasa setelah selesai download, langsung klik install dan next - next. Oh iya jangan lupa masukin passwordnya ya

Kalau sudah selesai kalian bisa buka app yang bernama pgAdmin 4 *punya saya versi 4

# Cara setting terminal postgree untuk Mac Os
Kan kadang males juga pake GUI ya, enakan pake terminal biar sat set sat set, eh pas mau di pake kok ga bisa. Nah ternyata harus di setting dulu.
Nah saya mau share pengalaman saya ya.

1. Kalian Buka terminal, lalu kalian ketikan 
```
$ vim ~/.bashrc atau vim ~/.zshrc 
```
Kalian bisa pake vim atau nano atau text editor yang biasa kalian gunakan ya.
Tiap laptop environment nya berbeda - beda, saat ini saya menggunakan macbook air m1
lalu kalian masukan pathnya dengan mengetikan 
```
export PATH=/Library/PostgreSQL/14/bin:$PATH

```
14 artinya version postgree yang kalian gunakan, kalian bisa sesuaikan postgree yang kalian install.

Oke Setelah itu kita kembali ke terminal, jangan lupa di save ya

Selanjutnya kita cek terlebih dahulu apakah postgree kita sudah terinstall dengan mengetikan
```
$ postgres -V
Jika sudah muncul seperti postgres (PostgreSQL) 14.4 maka postgree nya berhasil
```

Selanjutnya kita coba masuk posgree nya dengan ketikan terminal seperti dibawah ini 
```
$ sudo -u postgres psql

```
Selanjutnya berikan password laptop / pc kita 
```
password laptop kita 
```

Lalu ia akan meminta password untuk masuk ke postgree yang telah kita buat pada saat instalasi postgree.
```
password yang kita buat saat instalasi
```

Setelah bisa masuk ke postgree maka tulisannya akan seperti ini
```
postgres=# 
```

# Membuat Database 
Ketikan 
``` 
postgres=#  Create Database store_baju;
```
Jangan lupa terakhirnya ketikan titik koma ya ;

Akan saya update lagi untuk tutorial postgree yang lainnya di sini ya



