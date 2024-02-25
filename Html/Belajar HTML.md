# Struktur Dasar HTML 
```html
<!DOCTYPE html>
<html>
  <head>
    <title>ini adalah judul</title>
  </head>
  
  <body>
    <p>No Body</p>
  </body>
</html>
```
![[Screenshot_2024-02-19-10-38-44-620_com.foxdebug.acodefree.jpg]]
- Tag `<!DOCTYPE html>` memberitahukan web browser bahwa dokumen HTML adalah versi 5.
- Tag pembuka `<html>` menandai awal sebuah dokumen HTML sampai dengan tag penutup `</html>`.
- Tag pembuka `<head>` berisi informasi tentang halaman HTML sampai dengan tag penutup `</head>`, biasanya dalam tag head terdapat tag `<titel>` untuk memberikan informasi judul halam HTML.
- apapun tag yang berada di antara tag pembuka `<body>` sampai dengan tag penutup `</body>` akan tampil di web browser.
# Anatomi Elemen HTML
```html
<a href="https://www.google.com">Klik Goggle</a>
```
![A|250x500](asettt/a.jpg|250)
- Tag pembuka `<a>` tag yang menandakan awalan dan `</a>` akhir URL/link.
-  atribut `href` digunakan untuk menentukan halaman web URL/link. Contoh nilai atribut https://www.google.com.
- isi konten itu untuk masuk ke URL/link yang sudah kita buat di atribut `href` yaitu "klik google"
## Tag Pembuka dan Tag Penutup
Tag pembuka dan tag penutup adalah dua bagian dari suatu elemen dalam HTML yang digunakan untuk menentukan awal dan akhir dari elemen tersebut. Tag pembuka dimulai dengan nama elemen yang diapit oleh tanda kurung sudut ("<" dan ">"). Tag penutup serupa dengan tag pembuka, tetapi memiliki karakter garis miring tambahan ("/") sebelum nama elemennya. contoh ini, `<p>` adalah tag pembuka, dan `</p>` adalah tag penutup
## Atribut Tag
Atribut tag merujuk pada informasi tambahan yang diberikan kepada elemen HTML untuk memberikan rincian atau pengaturan tertentu. Atribut dapat ditambahkan ke sebagian besar tag HTML dan berfungsi untuk mengontrol perilaku atau tampilan elemen tersebut. Contohnya, pada tag `<a>` (hipertaut), atribut `href` digunakan untuk menentukan URL tujuan. Begitu juga, pada tag `<img>`(gambar), atribut src menunjukkan sumber gambar. 
## Isi/Konten Tag
Isi atau konten tag merujuk pada teks, elemen, atau informasi yang ditempatkan di antara tag pembuka dan tag penutup dalam markup HTML. Contoh sederhana adalah tag paragraf `<p>`, di mana isi tag tersebut adalah teks yang ingin dimuat dalam paragraf. Contoh "Ini adalah contoh isi atau konten dalam tag paragraf." adalah isi atau konten yang akan ditampilkan atau diinterpretasikan oleh browser web ketika halaman HTML di-render.
# Tag Dasar
## Heading
```html
<!DOCTYPE html>
<html>
  <head>
    <title>ini adalah judul</title>
  </head>
  
  <body>
    <h1>kata kata hari ini</h1>
    <h2>word of the day</h2>
    <h3>今日の単語</h3>
    <h4>ك4لمة اليوم</h>
    <h5>Từ trong ngày</h5>
    <h6>오늘의 단어</h6>
    <p>No Body</p>
    <p>tidak ada yang tahu</p>
    <a href="https://www.google.com">Klik Goggle</a>
  </body>
</html>
```
![[Screenshot_2024-02-19-10-41-51-750_com.foxdebug.acodefree.jpg]]

- Tag `<h1>` Digunakan untuk judul utama atau level judul tertinggi
- Tag `<h2>` Menunjukkan tingkatan judul yang lebih rendah dari `<h1>` atau subjudul
- Tag `<h3>` Menunjukkan tingkatan judul yang lebih rendah atau subjudul dari `<h2>`
- Tag `<h4>` Menunjukkan tingkatan judul yang lebih rendah atau subjudul dari `<h3>`
- Tag `<h5>` Menunjukkan tingkatan judul yang lebih rendah atau subjudul dari `<h4>`
- Tag `<h6>` Menunjukkan tingkatan judul yang lebih rendah atau subjudul dari `<h5>` 
## Paragraf

```html
<!DOCTYPE html>
<html>
  <head>
    <title>ini adalah judul</title>
  </head>
  
  <body>
    <p>nama saya</p>
    <br>
    <p><b>kelas saya</b></p>
    <hr>
    <p><u>No Body</u></p>
    <p><i>tidak ada yang tahu</i></p>
    <a href="https://www.google.com">Klik Goggle</a>
  </body>
</html>
```

![[Screenshot_2024-02-19-10-43-32-802_com.foxdebug.acodefree.jpg]]
- Tag `<p>`digunakan untuk menandai paragraf pada halaman web dan di akhiri `</p>` Ini memberikan jarak antara paragraf.
- Tag `<b>` digunakan untuk membuat teks menjadi tebal (bold) dan di akhiri `</b>`.
- Tag `<u>` digunakan untuk memberi garis bawah pada teks dan di akhiri `</u>`. 
- Tag `<i>` digunakan untuk membuat teks menjadi miring (italic) dan di akhiri `</i>`.
- Tag `<br>` digunakan untuk membuat jeda baris atau perpindahan ke baris berikutnya tanpa membuat paragraf baru.
- Tag `<hr>` digunakan untuk membuat garis horizontal, yang sering digunakan pemisah visual di antara bagian-bagian pada halaman web.

### Atribut Align
```html
<html>
  <head>
    <title>hello work</title>
  </head>
  <body>
    <h3>belajar menggunakan element align</h3>
    <p align="left">saya menggunakan element align dan saya ingin meratakan ke kiri tagnya align="left".</p>
    <h2>
      <p align="right">dan saya ingin meratakan ke kanan tagnya align="right".</p>
    </h2>
    <h1>
    <p align="center">saya ingin meratakan teks ketengah tagnya align="center".</p>
    </h1>
  </body>
</html>
```

![[Screenshot_2024-02-19-10-47-17-630_com.foxdebug.acodefree.jpg]]

**Penjelasan :**

- Atribut `align="left"` Teks dalam paragraf ini akan diatur agar terletak di sebelah kanan.
- Atribut `align="right"` Teks dalam paragraf ini akan diatur agar berada di tengah.
- Atribut `align="center" `Teks dalam paragraf ini akan diatur agar berada di sebelah kiri.


## Komentar

HTML juga mempunyai tag khusus untuk komputer untuk membuat komentar di HTML kita menggunakan awalan  `<!--` dan penutup `-->`

```html
<!DOCTYPE html>
<html>
  <head>
    <title>TAYO</title>
    </head>
  <body>
    <!--ini komentar,tidak akan tampil di browser -->
    <p>ini bukan komentar,dan akan tampil di browser</p>
  </body>
</html>
```




## List

```html
<html>
  <head>
    <title>good morning</title>
  </head>
  <body>
    <h1>
      <p>Nama-Nama Hari</p>
    </h1>
    <ul>
      <li>Senin</li>
      <li>selasa</li>
      <li>rabu</li>
      <li>kamis</li>
      <li>jum`at</li>
      <li>minggu</li>
    </ul>
    <h1>
      <p>Peralatan Dapur</p></p>
    </h1>
    <ol>
      <li>pisau</li>
      <li>panci</li>
      <li>spatula</li>
    </ol>
  </body>
</html>
```
![[Screenshot_2024-02-19-10-51-53-089_com.foxdebug.acodefree.jpg]]
- Tag `<Li>` dalam HTML digunakan untuk menandai Elemen daftar (list bahan). ini dapat
## Link

```html
<!DOCTYPE html>
<html>
  <head>
    <title>ini adalah judul</title>
  </head>
  
  <body>
<h3>Menggunakan Tag Anchor</h3>
<a href="https://www.google.com" target="_blank">Klik disini untuk ke google</a><br>
<a href="halaman_lain.html">Klik disini untuk ke halaman lain yang saya buat</a>
  </body>
</html>
```


- Link dapat ditemukan di hampir semua balaman web. Link/tautan memungkinkan sebuah teks yang ketika di klik akan pindah ke haleman lainnya. HTML menggunakan tag ``<a>``untuk kepeduan ini. Link ditulis dengan ``<a>``yang merupakan singkatan card anchor (jangkar).
- Setiap tag ``<a>``setidaknya memiliki sebuah atribut href Dimana bref berisi alamat yang dituju. bref adalah singkatan dari hypertext reference.
- Atribut penting lainnya dari tag ``<a>``adalah target. Atribut target menentukan tempat untuk membuka dokumen yang ditautkan. Atribut target, memiliki beberapa nilai salah satunya blank yang berfungsi untuk membuka tautan di tab baru.


## Multimedia 
Elemen `<iframe>` dapat digunakan untuk menampilkan dokumen html lain dalam sebuah website. Mudahnya, bsa dibilang website dalam website.

>[!tip] Contoh penggunaannya seperti ini. jika kita mempunyai website sekolah, lalu di website tersebut ingin menampilkan alamat alamat dalam google maps sekolah. Agar memudahkan pengunjung website, kita bsia langsung tampilan saja halaman sekolah yang ada di google maps

Dalam tag `<iframe>` ada beberapa atribut yang penting seperti:

- `src` , untuk mencari sumber halaman html atau web yang akan ditampilkan di dalam frame
-  `width` dan `height` , untuk mengatur ukuran panjang dan lebar dari frame

contoh

```html
<iframe src="https://www.petanikode.com/" width="1300px" height="450px"></iframe>
```

hasil

![](aset/ss22.png)

### Image

```html
<!DOCTYPE html>
<html>
  <head>
    <title>ini adalah judul</title>
  </head>
  <body>
    <img src="agiss.jpg" alt="Logo" width="150" height="150">
  </body>
</html>
```
Dalam HTML, gambar didefinisikan dengan tag ing) Tag <ing adalah tag kosong. hanya berisi atribut saja, dan tidak memiliki tag penutup.

==Atribut src setidaknya mesti ada dalam tag ini untuk menentukan URL (alamat web) dari gambar yang ingin ditampilkan.==

Atribut alt menyediakan teks alternatif untuk gambar, jika pengguna karena beberapa alasan tidak dapat melihatnya (karena koneksi lambat, kesalahan pada atribut are, atau jika web browser telah disetting untuk tidak menampilkan gambar). Jika browser tidak dapat menemukan gambar, maka akan muncul nilai pada atribut.

Dalam tag ``<img>`` terdapat juga atribut width dan height untuk mengatur ukuran gambar, pada versi HTML5 standar satuan ukuran gambar adalah pixel.

- Misalnya dalam folder root terdapat file gambar bernama logo.png. Untuk menampilkan gambar tersebut kita hanya perlu mengisi nama gambar beserta jenis ekstensi file gambar ke dalam atribut src, contohnya src="logo.png".
- Untuk menampilkan gambar dari internet carilah link gambar yang akan ditampilkan lalu masukkan dalam nilai atribut src, contohnya https://namasitus.com/gambar.png.

![[IMG_20240124_080909.jpg]]


![[IMG_20240124_080829.jpg]]


## Table
Tabel dalam HTML di definisikan dengan `<table>`
- Setiap baris tabel didefinisikan dengan tag `<tr>`
- Header (judul) tabel didefinisikan dengan tag `<th>`. secara default, header tabel memiliki teks tebal dan beraada di tengah
- Data tabel/sel didefinisikan dengan tag `<td>` . Karena sel merupakan bagian terkecil dari tabel maka dari itu tag selalu berada di dalam tag `<tr>` .

contoh
```html
<table border="1">
        <tr>
            <th>no</th>
            <th>NAMA</th>
            <th>asal sekolah</th>
            <th>kelas</th>
            <th>kelamin</th>
            <th>umur</th>
        </tr>
        <tr>
            <td>1</td>
            <td>Ahmad Anugrah Satya </td>
            <td>smk negeri 7 makassar</td>
            <td>XI RPL 1</td>
            <td>laki-laki</td>
            <td>16</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Muh.Agis </td>
            <td>smk negeri 7 makassar</td>
            <td>XI RPL 1</td>
            <td>laki-laki</td>
            <td>16</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Muh.Daud Resky Jayadi </td>
            <td>smk negeri 7 makassar</td>
            <td>XI RPL 1</td>
            <td>laki-laki</td>
            <td>17</td>
        </tr>
        <tr>
            <th>1</th>
            <th>Muh.Nur Resky Alfatir </th>
            <th>smk negeri 7 makassar</th>
            <th>XI RPL 1</th>
            <th>laki-laki</th>
            <th>16</th>
        </tr>
    </table>
```

hasil
![400](aset/ss23.png)

>[!tip] Perhartikan bahwa pada tag `<table>` terdapat sebuah atribut `border`. Atribut border yang digunakan untuk memberikan nilai garis tepi dati tabel, nilai ini dalam ukuran pixel. `border="1"`, berarti kita mengistruksi kepada web browser bahwa tabel tersebut akan memiliki garis tepi sebesar 1 pixel. Jika tidak ditambahkan, secara default tabel tidak memiliki garis tepi. 

Selainitu, terdapat pula beberapa atribut tabel yang penting untuk diketahui yaitu:

- `rowspan` merupakan atribut HTML yang berfungsi untuk mengadakan beberapa baris (ke bawah)
  - `colspan` atau colomn spawn merupakan atribut HTML yang berfungsi untuk menggabungkan beberapa kolom (ke samping)
  - `width` berfungsi untuk mengatur lebar tabel yang nilainya didefinisikan dalam satuan pixel secara default.
  - `height` berfungsi untuk mengatur tinggi tabel yang nilainya didefinisikan dalam satuan pixel secara default.
  - `align` berfungsi untuk mengatur perataan teks padatabel. Nilai atribut yang dapat diberikan yaitu `left` untuk perataan teks ke kiri, `right` untuk perataan teks ke kanan, `center` untuk perataan teks ke tengah.

contoh
```html
<table border="1">
        <tr>
        <th rowspan="2">Nama</th>
        <th colspan="2">punya ktp</th>
        </tr>
        <tr>
        <th width="100">belum punya</th>
        <th width="100">sudah punya</th>
        </tr>
        <tr>
        <th>Ahmad Anugrah Satya</th>
        <th>belum</th>
        <th align="center">-</th>
        </tr>
        <tr>
            <th>Muh.Agis</th>
            <th>belum</th>
            <th align="center">-</th>
        </tr>
        <tr>
            <th>Muh.Daud Resky Jayadi</th>
            <th align="center">-</th>
            <th>sudah</th>
        </tr>
        <tr>
            <th>Muh.Nur Reksi Alfatir</th>
            <th>belum</th>
            <th align="center">-</th>
        </tr>
    </table>
```


hasil

![](aset/ss24.png)
## Video

```html
<!DOCTYPE html>
<html>
  <head>
    <title>ini adalah judul</title>
  </head>
  <body>
    <video controls width="250px" height="125px">
      <source src="bukan.mp4" type="bukan.mp4">
    </video>
  </body>
</html>
```
 Dalam tag `<video>` terdapat juga atribut   `controls` yang digunakan untuk Menambahkan kontrol pemutaran standar seperti play, pause, dan volume, dan juga di tag `<video>` ada atribut `width` dan `height` yang digunakan untuk mengatur ukuran video, pada versi HTML 5 standar satuan ukuran video adalah pixel, dan juga di dalam nya juga terdapat atribut `type` yang di gunakan untuk menentukan tipe MIME (Multipurpose Internet Mail Extensions) dari file video yang disematkan.
 dalam HTML, video didefinisikan dengan tag `<video>`, tag `<video>` adalah tag yang digunakan untuk memasukkan video kedalam web, di tag `<video>` terdapat tag khusus yang dimana tag ini tidak memiliki tag penutup yaitu `<source>` yang Digunakan untuk menyediakan beberapa sumber video dan memberi browser pilihan format yang sesuai.
 Noya: misalnya dalam folder root terdapat file video bernama video.mp4. untuk menampilkan video tersebut kita hanya perlu mengisi nama video beserta jenis ekstensi file video didalam tag `<source>` dan didalamnya atribut `src` terus juga didalam tag `<source>` kita beri juga didalamnya atribut `type` untuk menetukan tipe MIME(Multipurpose Internet Mail Extensions) di file video yang di sematkan.

![[IMG_20240127_003914.jpg]]
 
![[IMG_20240127_003853.jpg]]

## Audio 

![[IMG_20240131_131153.jpg]]
 - src digunakan untuk menentukan URL atau path ke file media yang akan dimainkan.
- `controls` yang digunakan untuk Menambahkan kontrol pemutaran standar seperti play, pause, dan volume.
- `type` digunakan untuk menentukan tipe MIME (Multipurpose Internet Mail Extensions) dari file audio yang disematkan.
- `<source>` Digunakan untuk menyediakan beberapa sumber audio dan memberi browser pilihan format yang sesuai.
 Di HTML, tag `<audio>` digunakan untuk menyematkan dan memainkan file audio di halaman web. Tag ini memungkinkan pengembang web menyertakan file audio langsung di dalam dokumen HTML, memungkinkan pemutaran langsung di halaman tanpa perlu mengarahkan pengguna ke halaman terpisah atau menggunakan pemutar audio eksternal. di dalam tag `<audio>` juga memiliki atribut yaitu `src` ,  `controls` , `type` yang memiliki fungsi masing masing.



## From

`<form> `HTML digunakan untuk mendefinisikan form yang digunakan  untuk mengumpulkan inputan dari penggunaan website. Tag ini digunakan untuk mengoleksi inputan dari user, konsep ini sama seperti konsep formulir di dunia nyata.

>[!tip] dengan kata lain tag `<form>`  merepsentikasikan sebuah "formulir" di mana satu formulir bisa dimiliki banyak kolom isian. 

Form HTML berikan elemen-elemen `form` lainnya. Elemen `<form>` digunakan untuk menampung macam-macam  elemen yang berkaitan dengan sebuah `form`, seperti `text` `fields`, `checkbox`, `radio button`, tombol `submit`, dan  banyak lagi yang dapat diedit kemudian ditulis untuk dikirim pada sebuah server untuk selanjutnya diproses guna mendapatkan informasi tertentu dari atau untuk user.
Umumnya, sebuah website selalu memiliki fitur form, contoh paling umum yang sering kita temui adalah seperti form login, form sign up, form komentar di suatu blog/media.

1. Input 
Elemen `<input>` adalah elemen `form`yang paling penting. Elemen `<input>` dapat ditampilkan dalam beberapa cara, tergantung pada nilai atribut `type` yang digunakan. Berikut adalah beberapa contoh nilai dari atribut type: 
- `text` digunakan untuk mengambil isian berupa teks. Contohnya seperti nama. 
- `password` digunakan untuk mengambil isian berupa kata sandi atau sesuatu yang bersifat rahasia. Tipe ini akan mengubah semua karakter yang diketikkan ke dalam karakter bulat. 
- `radio` digunakan sebagai kolom isian bertipe pilihan yang menawarkan beberapa opsi kepada user namun tetapi hanya satu opsi saja yang boleh dipilih. Contohnya seperti jenis kelamin atau agama. 

>[!tip] Perlu diperhatikan bahwa untuk penggunaan tipe `radio` yang berkategori set pilihan yang sama mengharuskan nilai `name` -nya juga sama. 

Opsi default dapat dilakukan dengan menambahkan atribut `checked` pada elemen opsi yang dijadikan sebagai opsi default. 

- `checkbox` digunakan untuk memberikan daftar pilihan dalam satu set opsi. User dapat memilih satu atau bahkan lebih dari satu pilihan pada tipe ini. Hal ini berbeda dengan tipe sebelumnya yaitu `radio` yang hanya memungkinkan user untuk memilih satu pilhan saja. Contoh penggunaan `checkbox` seperti daftar makanan kesukaan, daftar olahraga yang tidak disukai, dan yang semisalnya.

>[!tip] Perlu diperhatikan bahwa untuk penggunaan tipe `checkbox` yang berkategori set pilihan yang sama mengharuskan nilai `name`-nya juga sama.
>

- `number` digunakan untuk membatasi isian user hanya pada karakter numerik saja. Browser akan menambahkan dua buah tombol atas dan bawah untuk mengubah angka isian. 
Beberapa atribut untuk tipe number: 
- min - menentukan angka minimal 
- max - menentukan angka maksimal 
- step - menentukan kelipatan (nilai yang tidak sesuai kelipatan tidak bisa di-input, dan default dari atribut ini adalah 1) 

- `date` digunakan untuk memberikan isian berupa tanggal. Atribut `min`dan `max` dapat pula difungsikan pada tipe ini untuk mengatur tanggal minimal dan tanggal maksimal yang diinginkan. Nilai `min` dan `max` tersebut ditulis dengan format: `YYYY-MM-dd`.
- `file` digunakan untuk memungkinkan pengguna memuat file. Atribut `accept` juga dapat disisipkan pada tipe ini dengan maksud untuk mengatur file apa saja yang boleh di-upload. Beberapa contoh value dari atribut `accept` yaitu: 
- `accept="image/png,image/jpg, image/jpeg"` - untuk file gambar seperti png, jpg, atau jpeg 
- `accept=".pdf` - untuk file pdf
- `accept=".doc, .docx"` - untuk file `doc` atau `docx`
- `accept=".ppt, .pptx"` - untuk file `ppt` atau `pptx`

- `submit` ditampilkan dalam bentuk tombol untuk mengirim data pada `<form>` yang menjadi pembungkusnya. Atribut `value` digunakan untuk mengisi teks yang ingin ditampilkan pada tombol.
- `reset` berguna untuk mengembalikan state (keadaan) atau data dari suatu form ke nilai awalnya. Jika nilai awal sebuah input adalah kosong, maka ketika direset ia akan kembali kosong. Tapi jika nilai awalnya sudah terisi sesuatu, maka ketika direset datanya akan kembali seperti yang sudah diset sebelumnya.
- `button` berguna untuk membuat inputan berupa sebuah tombol. Tombol ini nantinya bisa difungsikan sesuai dengan keinginan dari pengembang web.

2. *Label*
Elemen `<label>` memiliki fungsi khusus untuk melabeli sebuah kolom inputan. Ketika screen reader membaca konten halaman HTML, lalu menemukan sebuah inputan, ia akan membaca label yang bersangkutan. 
Fungsi lain dari tag `<label>` adalah ketika kita mengklik label, maka browser akan meletakkan fokus pada kolom isian yang terhubung dengannya. Syarat yang perlu diperhatikan yaitu dengan menghubungkan sebuah `<label>` dan `<input>` dengan atribut for untuk label, dan atribut id pada `<input>` dengan nilai untuk kedua atribut tersebut mesti sama persis.

3. *Select*
Elemen `<select>` berguna dalam mendefinisikan sebuah tombol dropdown yang dimana user dapat memilih salah satu dari banyak pilihan.

> [!tip] - Elemen `<select>` nantinya berperan sebagai kontainer atau pembungkus dari elemen `<option>` yang berperan sebagai daftar pilihan atau opsi. 

 Elemen `<select>` hampir mirip fungsinya dengan `<input type ="radio">` akan tetapi baiknya elemen `<select>`digunakan untuk memilih satu pilihan yang terdapat banyak opsi di dalamnya, sedangkan `<input type ="radio">` lebih baiknya untuk digunakan jika user diarahkan memilih hanya satu pilihan yang opsi pilihannya tidak terlalu banyak. Contoh penggunaan elemen ini seperti memasukkan pilihan berupa asal daerah atau yang semisalnya.
 
Penting untuk diketahui bahwasanya opsi yang aktif secara default adalah adalah opsi yang pertama. Akan tetapi, kita bisa mengatur opsi mana yang aktif secara default dengan menambahkan atribut selected pada suatu `<option>` yang ingin dijadikan sebagai opsi default.

4. *Text Area*
Elemen `<textarea>` berguna untuk mengambil inputan user berupa teks yang dapat memuat lebih dari satu baris. Jika dibandingkan dengan elemen `<input>` teks biasa, elemen `<textarea>` memiliki ukuran tinggi yang lebih besar. Element `<textarea>` bisa diisi lebih dari satu baris dengan menekan enter.

Atribut yang dapat digunakan untuk mengatur kuran dari textarea yaitu rows untuk jumlah baris, sedangkan atribut cols untuk lebarnya.

5. *Button*
Elemen `<button>` yang berada di dalam sebuah form akan otomatis dianggap sama fungsinya seperti `<input type="submit">`. Jika ingin membuat tombol biasa yang tidak men-submit `<form>` dapat dilakukan dengan menambahkan atribut type="button".

Beberapa atribut yang digunakan pada contoh di atas yang perlu untuk diperjelas yaitu sebagai berikut:

- name - digunakan sebagai nama variabel yang akan diproses oleh web server (contoh menggunakan PHP)
- required - digunakan untuk memastikan bahwa pengguna harus memasukkan nilai pada input tersebut sebelum dapat melakukan proses submit formulir
- placeholder - menuliskan teks pada elemen input. Placeholder sangat bermanfaat untuk memberikan teks bantuan kepada user untuk inputan form yang kompleks
- value - menentukan nilai awal dari sebuah elemen input
- disabled - digunakan untuk menonaktifkan inputan pada elemen yang diberi atribut ini

Bagaimana Cara Memproses Form?*

Ketika sebuah <form> disubmit, baik menggunakan elemen <button> mau pun <input type="submit">, browser akan mengirimkan data tersebut kepada URL yang didefinisikan pada atribut action di dalam tag form.

Ada pun jika atribut action tidak didefinisikan, maka browser akan menggunakan URL sekarang sebagai tujuan pengiriman data.

Contoh:

```html
<h1>Formulir Pendaftaran</h1>
<form action="">
  <div>
    <label for="nama-lengkap"><b>Nama Lengkap:</b></label
    ><br />
    <input
      type="text"
      id="nama-lengkap"
      name="nama_lengkap"
      placeholder="Masukkan nama lengkap"
      required
    />
  </div>
  
  <div>
    <label for="password"><b>Password:</b></label
    ><br />
    <input
      type="password"
      id="password"
      name="password"
      placeholder="Masukkan password"
      required
    />
  </div>
  
  <div>
    <b>Jenis Kelamin:</b><br />
    <input id="lk" type="radio" name="jenis_kelamin" checked />
    <label for="lk">Laki-Laki</label>
    <input id="pr" type="radio" name="jenis_kelamin" />
    <label for="pr">Perempuan</label>
  </div>
  
  <div>
    <label for="isian-usia"><b>Usia:</b></label
    ><br />
    <input
      type="number"
      id="isian-usia"
      name="usia"
      min="17"
      max="25"
      value="19"
      required
    />
    Tahun
  </div>

  <div>
    <label for="tgl-ijazah"><b>Tanggal Ijazah:</b></label> <br />
    <input
      type="date"
      id="tgl-ijazah"
      name="tgl_ijazah"
      min="2021-01-01"
      value="2023-06-20"
      required
    />
  </div>

  <div>
    <label for="opsi-agama"><b>Agama:</b></label
    ><br />
    <select id="opsi-agama" name="agama" required>
      <option disabled>---Pilih Agama----</option>
      <option value="islam">Islam</option>
      <option value="kristen">Kristen</option>
      <option value="katolik">Katolik</option>
      <option value="hindu">Hindu</option>
      <option value="buddha">Buddha</option>
      <option value="atheis" disabled>Atheis</option>
    </select>
  </div>

  <div>
    <label for="alamat"><b>Alamat:</b></label> <br />
    <textarea
      id="alamat"
      name="alamat"
      cols="25"
      rows="5"
      placeholder="Harap masukkan alamat secara lengkap"
      required
    ></textarea>
  </div>

  <div>
    <b>Kemampuan Berbahasa Asing:*</b><br />
    <input type="checkbox" id="inggris" name="bahasa_asing" />
    <label for="inggris">Inggris</label>
    <input type="checkbox" id="arab" name="bahasa_asing" />
    <label for="arab">Arab</label>
    <input type="checkbox" id="jepang" name="bahasa_asing" />
    <label for="jepang">Jepang</label>
  </div>

  <div>
    <label for="isian-foto"><b>Foto 4x6:*</b></label
    ><br />
    <input
      type="file"
      id="isian-foto"
      name="foto"
      accept="image/png,image/jpg,image/jpeg"
    />
  </div>

  <br />
  <input type="submit" value="Kirim" />
  <input type="reset" value="Batal" />
  <i>*opsional (tidak wajib diisi)</i>
</form>
```



Pada contoh di atas, ketika form di-submit, browser akan mengirimkan data yang ada  menuju URL /proses-pendaftaran.
[12:52, 1/31/2024] taufik Asep: *Apa yang terjadi pada URL /proses-pendaftaran?*

Pada URL tersebut terdapat sebuah aplikasi/program yang berjalan di server (bukan di browser). Tugas dari program tersebut adalah mengelola data yang dikirim seperti misalnya menyimpan data tersebut ke dalam sebuah database.

Bahasa yang umum digunakan di dalam server adalah python, nodejs, PHP, dan lain sebagainya.

Untuk mendapatkan gambaran lebih jelas, sebenarnya akan dijelaskan pada modul selanjutnya yang berkaitan dengan materi PHP atau juga bisa dengan membaca tutorial berikut:
Hiu
