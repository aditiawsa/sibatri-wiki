# Dokumentasi Aplikasi Sibatri

![image](https://user-images.githubusercontent.com/74525957/194998459-b9a3bb52-e7ef-496a-8254-dd19905515ed.png)
| _`GAMBAR 1. Main Dashboard` Halaman Utama Aplikasi Sibatri Saat Pertama Dibuka_

Sibatri merupakan sistem aplikasi perangkat lunak yang berfungsi untuk meningkatkan efektifitas dan efisiensi dalam proses survei batimetri. Kata Sibatri merupakan singkatan untuk menyederhanakan kata sistem survei batimetri. Kelebihan dari perangkat lunak aplikasi ini adalah proses survei batimetri dapat dilakukan dengan lebih mudah di mana proses akuisisi data dapat dilakukan bersamaan dengan proses pengolahan data dalam menghasilkan peta batimetri secara _real-time_. Secara keseluruhan, aplikasi ini memiliki tiga fitur utama, antara lain: fitur akuisisi data, fitur validasi data, dan fitur _display_ peta batimetri yang terbagi menjadi tiga halaman dashboard.

## 1. Halaman Utama (_Main Dashboard_)

![image](https://user-images.githubusercontent.com/74525957/195000017-0d5b8810-f507-44d7-855f-0df5ec37be13.png)
| _`GAMBAR 2. Halaman Utama`Aplikasi Sibatri Saat Sedang Melakukan Proses Akuisisi Data._

Halaman utama dari aplikasi sibatri merupakan _dashboard_ yang difokuskan untuk proses survei batimetri secara _real-time_. Fitur-fitur pada halaman ini di antaranya adalah fitur perekaman data (_data logging_), _display_ data logging, _display_ peta batimetri secara _real-time_, dan _display_ jalur survei batimetri menggunakan _tiles_ berbasis Google Maps.

### Perekaman Data

Pada proses perekaman data akuisisi, terdapat beberapa pengaturan/konfigurasi masukan umpan data yang sangat penting untuk diperhatikan dan dipenuhi. Konfigurasi data yang dapat diterima oleh aplikasi sibatri sangat spesifik sehingga jika pengaturan umpan data yang diterima oleh aplikasi ini tidak sesuai maka aplikasi tidak mampu menerima dan mengolah data untuk dapat direkam dan disimpan. Di antara beberapa konfigurasi data tersebut, antara lain:

#### 1. Umpan Data Merupakan Data Serial Yang Tersusun Dari Integrasi Data Perangkat _Single Beam Echo Sounder_ (SBES) dan _Global Positioning System_ (GPS).
Data serial yang diumpankan pada aplikasi sibatri merupakan data serial yang tersusun dari integrasi data perangkat  _Single Beam Echo Sounder_ (SBES) dan _Global Positioning System_ (GPS). Data serial ini merupakan data yang berisikan ariabel-variabel yang nantinya dapat digunakan dalam fitur lain yang mencakup proses survei batimetri, seperti pengolahan data untuk menghasilkan peta batimetri ataupun pengolahan data dalam menampilkan jalur survei batimetri.

#### 2. Susunan Variabel Data Serial
Susunan variabel data serial yang diumpankan pada aplikasi sistem survei batimetri diatur secara khusus dan spesifik dengan urutaan sebagai berikut:
1. Variabel waktu --> Tipe data string
2. Variabel kedalaman --> Tipe data desimal (_float_)
3. Variabel temperatur --> Tipe data desimal (_float_)
4. Variabel jumlah satelit --> Tipe data bilangan bulat (_integer_)
5. Variabel garis lintang --> Tipe data desimal (_float_)
6. Variabel garis bujut --> Tipe data desimal (_float_)

#### 3. Setiap Variabel Dipisahkan Tanda Koma (,)

