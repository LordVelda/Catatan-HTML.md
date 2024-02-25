# instalasi mySQL
## menggunakan termux
1. Buka termux
2. Ketik ``termux-setup-storage``
3. Klik izinkan/allow access
4. Lakukan update dan upgrade paket.ketik ``pkg update && upgrade``
5. Jika ada konfirmasi untuk melanjutkan instalasi ketik aja ``Y``
6. Install applikasi mariadb dengan mengetik``pkg install mariadb``
7. Ketika proses nya berhenti dan ada pilihan ketik saja ``Y`` untuk melanjutkan proses penginstalannya. 
8. Ketik ``mysqld_safe`` untuk memberi keamanan
9. Untuk menghentikan proses ``ctrl+z``
10. Masuk ke akun admin ``mysql -u root`` 
## referensi youtube
![](https://youtu.be/JojQd-l7fEE?si=OPIB01q45A2FmY1x)

# penggunaan awal MySQL
## Query
``<mysql -u root -p>``
## hasil
![250](asett/mysql1.jpg)

## Analisis kesimpulan
- `<mySQL>` Salah satu aplikasi database server dengan bahasa pemrograman structured query languange `(SQL)` yang berfungsi untuk mengelola data secara terstruktur dan sistematis.
- `<-u root>` Bagian ini mengeset pengguna (user) yang akan digunakan saat terhubung ke server  MYSQL. Dalam contoh ini, pengguna yang digunakan adalah `"root"`. Pengguna `"root"` biasanya memiliki hak akses penuh ke server MYSQL dan dapat melakukan tindakan administratif.
- `<-p>` Opsi ini digunakan untuk meminta kata sandi (password) setelah perintah dijalankan ini adalah langkah keamanan yang umum digunakan untuk memastikan hanya pengguna yang sah yang dapat mengakses server MYSQL. Setelah kita menekan Enter setelah perintah ini, kita akan diminta memasukkan kata sandi untuk pengguna `"root"`.
# Data Base
Database (basis data) adalah kumpulan terstruktur dari informasi yang disimpan secara elektronik dalam sistem komputer. Database dirancang untuk menyimpan, mengatur, dan mengelola data dengan cara yang efisien dan dapat diakses.
## buat data base
- `CREATE DATABASE` adalah perintah untuk membuat database baru.
- ``[XI_RPL_1]`` adalah nama yang Anda pilih untuk database baru Anda. Tanda kurung siku `<("[]")>` digunakan di sini untuk menghindari kesalahan jika nama database mengandung karakter spesial atau spasi. Namun, perlu dicatat bahwa tidak semua DBMS mengizinkan penggunaan tanda kurung siku dalam nama database, jadi pastikan untuk menyesuaikan sintaksdengan DBMS yang Anda gunakan.
### Query
``create database xi_rpl_1;``

### Hasil:
![300](asett/mysql2.jpg)

## Tampilkan data base
`SHOW DATABASE` digunakan untuk menampilkan daftar database yang ada dalam sistem manejemen basis data (DBMS). Perintah ini dapat digunakan di beberapa DBMS seperti MYSQL, PostgreSQL, dan beberapa DBMS lainnya. Namun, perintahnya dapat sedikit berbeda tergantung
### Query 
``show databases;``

### Hasil:
![250](asett/mysql4.jpg)
## hapus database
``<DROP DATABASE [nama_database]>`` digunakan dalam sistem manajemen basis data (DBMS) untuk menghapus sebuah database beserta semua objek yang terkait dengan database tersebut, seperti tabel, indeks, tampilan, prosedur tersimpan, dan lain-lain.
### Query
``drop database xi_rpl_1``
### Hasil:
![300](asett/mysql3.png)

## gunakan data base
``USE [nama_database]`` digunakan dalam sistem manajemen basis data (DBMS) untuk beralih atau memilih database yang akan digunakan. Ketika Anda menggunakan perintah ``<USE>`` diikuti dengan nama database, DBMS akan mengarahkan semua perintah dan operasi selanjutnya pada database yang ditentukan.
### Query
`` use xi_rpl_1; ``
### Hasil:
![300](asett/mysql5.jpg)

# Tipe Data
## Angka
**INT**: Untuk menyimpan nilai bilangan bulat (integer). Misalnya, INT dapat digunakan untuk menyimpan angka seperti 1, 100, -10, dan sebagainya.

**DECIMAL**: Digunakan untuk menyimpan nilai desimal presisi tinggi, cocok untuk perhitungan finansial atau keuangan.

**FLOAT dan DOUBLE**: Digunakan untuk menyimpan nilai desimal dengan presisi floating-point. DOUBLE memiliki presisi lebih tinggi dibandingkan FLOAT.

**TINYINT , SMALLINT , MEDIUMINT , dan BIGINT**: Tipe data ini menyimpan bilangan bulat dengan ukuran yang berbeda-beda.
## Teks
**CHAR(N)**: Menyimpan string karakter tetap dengan panjang N. Contoh: CHAR(10) akan menyimpan stringdengan panjang tepat 10 karakter.

**VARCHAR(N)**: Menyimpan string karakter dengan panjang variabel maksimal N. Misalnya,
VARCHAR(255) dapat menyimpan string hingga
255 karakter, tetapi sebenarnya hanya menyimpan panjang yang diperlukan plus
beberapa overhead.

**TEXT**: Digunakan untuk menyimpan teks dengan panjang variabel, tanpa batasan panjang tertentu. Cocok untukdata teks yang panjangnya tidak terduga.

**ENUM**: Memungkinkan Anda mendefinisikan set nilai yang mungkin dan membatasi kolom hanya dapat mengambil salah satu dari nilai tersebut.

**SET**: Mirip dengan ENUM, namun dapat menyimpan satu atau lebih nilai dari himpunan yang telah ditentukan.
## Tanggal
**Date**: digunakan untuk menyimpan informasi tentang tanggal, biasanya terdiri dari hari, bulan, dan tahun seperti 30 Januari 2024

**Time**: digunakan untuk menyimpan informasi tentang waktu dalam sehari, biasanya terdiri dari jam, menit, detik, dan milidetik seperti 14:30:45.500

**DateTime**: menggabungkan informasi tanggal dan waktu dalam satu objek, biasanya terdiri dari hari, bulan, tahun, jam, menit, detik, dan milidetik seperti 30 Januari 2024 14:30:45.500

**TimeStamp**: Sama seperti DATETIME, tetapi dengan kelebihan diatur secara otomatis saat data dimasukkan atau diubah.
## Boolean
**BOOL / BOOLEAN / TINYINT**: Digunakan untuk menyimpan nilai boolean, yang dapat mewakili kebenaran (true) atau kesalahan (flase). 
## Tipe data Pilihan
 **Enum**: Menyimpan satu nilai dari daftar nilai yang ditentukan.
 
 **Set**: Menyimpan beberapa nilai dari daftar nilai yang ditentukan 
# Tabel

## Buat Tabel
**Struktur Query**:
```sql
CREATE TABLE [nama_table] ( 
nama_kolom1 tipe_data(ukuran) [tipe_constraint] 
nama_kolom2 tipe_data(ukuran) [tipe_constraint] 
nama_kolom3 tipe_data(ukuran) [tipe_constraint] );
```

**Contoh Query**:
```sql
CREATE TABLE Pelanggan (
id_pelanggan int(4) PRIMARY KEY NOT NULL,
nama_depan varchar(25) NOT NULL,
nama_belakang varchar(25) NOT NULL,
no_telp char(12) UNIQUE );
```

**Hasil**:
![s](asett/struktur.jpg)

**Analisis**:

**Kesimpulan**:
## Tampilkan Struktur Tabel
**Struktur Query**:
`desc [nama_table];`

**Contoh Query**:
`desc Pelanggan;`

**Contoh**:
![s](asett/struktur.jpg)

**Analisis**:

**Kesimpulan**:
## Menampilkan Daftar Tabel
**Struktur Query**:
`show tables;`

**Contoh**:
`show tables;`

**Hasil**:
![s](asett/tables.jpg)

**Analisis**:

**Kesimpulan**:
## QNA
>[! Faq]- Mengapa hanya kolom id_pelanggan yang menggunakan constraint PRIMARY KEY?
> > Untuk membedakan id Pelanggan  yang sama, mencegah duplikasi, dan mempermudah pencarian data.


> [! Faq]- Mengapa pada kolom no_telp yang menggunakan tipe data chat bukan varchar?
> > Tipe data char menyimpan data dalam karakter panjang lebih efisien. pencarian pada kolom tipe data `CHAR` dapat lebih cepat.


> [! Faq]- Mengapa hanya kolom no_telp yang menggunakan constraint UNIQUE?
> > Karna no_telp tidak ada yang sama semua pasti berbeda dan nilainya unik maka menggunakan constrains unique artinya data dalam tabel id_telpon berbeda tidak ada yang sama. 


> [! Faq]- Mengapa kolom no_telp tidak memakai constraint NOT NULL, sementara kolom lainnya menggunakan constraint tersebut?
> > Nomor telpon dianggap opsional. nomor telepon hanya menjadi wajib saat pengguna melakukan langkah-langkah tertentu, Anda mungkin tidak ingin mengharuskan pengguna mengisinya pada tahap awal.

> [! Faq]- Perbedaan PK & UNIQUE
> > PRIMERY KEY untuk membedakan data yang sama dan hanya boleh 1 dan tidak boleh tidak ada. Kalau UNiQUE sebuah kolom yang memiliki data yang berbeda atau tidak sama unique boleh 1,2,3 Dan seterusnya dan boleh tidak ada.

# Insert
## Insert 1 Data
### Struktur
```sql
Insert into [nama_tabel]
Values (nilai1, nilai2, nilai3, nilai4)
```
### Contoh
```sql
insert into Pelanggan
values (1,"muhammad","agis","08500000");
```
### Hasil
![s](asett/data1.jpg)
### Analisis

### Kesimpulan 

## Insert > 1 Data
### Struktur
```sql
Insert into [nama_table]
Values (nilai1, nilai2, nilai3, nilai4)
       (nilai1, nilai2, nilai3, nilai4)
       (nilai1, nilai2, nilai3, nilai4)
```
### Contoh
```sql
insert into Pelanggan
values (2,"muh","nur","0890000"),(3,"muh","daud","0870000"),(4,"ahmad","anugrah","08100000");
```
### Hasil
![s](asett/data2.jpg)

### Analisis 

### Kesimpulan 

## Menyebut Kolom
### Struktur
```sql
insert into [nama_table]
(Kolom1, kolom1, kolom3)
values (niali1, nilai2, nilai3);
```
### Contoh
```sql
insert into Pelanggan
(id_pelanggan,nama_depan,nama_belakang)
values (5,"muh","fadil");
```
### Hasil
![a](asett/kolom1.jpg)
### Analisis

### Kesimpulan

# Select
## Seluruh Data
### Struktur
`select * from [nama_table];`
### Contoh
`select * from Pelanggan;`
### Hasil
![a](asett/kolom1.jpg)
### Analis 

### Kesimpulan

## Data Kolom Tertentu
### Struktur
```sql
Select [nama_kolom1],[nama_kolom2],...[nama_kolomN]
From [nama_table];
```
### Contoh
`select nama_depan from Pelanggan;`
### Hasil
![a](asett/kolom2.jpg)
### Analisis

### Kesimpulan 

## Klausa Where
### Struktur
```sql
Select [nama_kolom] from [nama_table] where kondisi;
```
### Contoh
```sql
select id_pelanggan,nama_depan from Pelanggan where id_pelanggan=1;
```
### Hasil
![a](asett/where.jpg)
### Analisis

### Kesimpulan 

# Update
## Struktur
```sql
Update nama_table set nama_kolom where kondisi;
```
## Contoh
```sql
Update Pelanggan set no_telp="085326000" where id_pelanggan="1";
```
## Hasil
![a](asett/update.jpg)
## Analisis 

## Kesimpulan 

# Delete
## Struktur
```sql
Delete from nama_table where kondisi;
```
## Contoh
```sql
delete from Pelanggan where id_pelanggan="5";
```
## Hasil
![a](asett/delete.jpg)
## Analisis

## Kesimpulan 
