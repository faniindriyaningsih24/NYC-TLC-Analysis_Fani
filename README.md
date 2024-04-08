# Capstone_Module2_NYC_TLC_Record
Data analisis tentang dataset NYC-TLC-Record

# Background / Latar Belakang
New York City Taxi and Limousine Commission (TLC),yang dibentuk pada tahun 1971, adalah lembaga yang bertanggung jawab atas lisensi dan regulasi taksi Medallion (Kuning) Kota New York, kendaraan sewa (layanan dasar komunitas, mobil hitam, dan limusin mewah), van komuter, dan kendaraan paratransit.

TLC berdiri dari zaman dimana teknologi belum banyak dimanfaatkan dalam kehidupan sehari-hari hingga bertahan di era modern seperti ini, dimana teknologi banyak sekali dimanfaatkan dalam kehidupan sehari-hari. Penggunaan teknologi pun diterapkan TLC pada `trip type`. Namun fenomenanya tingginya frekuensi pada salah satu `trip type` disuatu wilayah, tidak berpengaruh terhadap besarnya `rata-rata total amount`.


Sumber dapat diakses pada link berikut [klik link](https://www.nyc.gov/site/tlc/about/about-tlc.page).

# Problem Statement / Pernyataan Masalah

Tingginya frekuensi pada salah satu `trip type`, tidak berpengaruh terhadap besarnya `rata-rata total amount`.

Trip type memiliki 2 tipe perjalanan, yaitu :
<br>`1 = Street-hail` : Tipe perjalanan ini penumpang memberhentikan taxi dengan cara angkat tangan dengan artian bahwa penumpang ingin menaiki taxi.

<br>`2 = Dispatch` : Tipe perjalan ini penumpang menggunakan layanan taxi yang diatur melalui panggilan telepon atau aplikasi pemesanan taxi.

Wilayah pada perjalanan taxi di TLC terbagi 6 wilayah, yaitu:
<br>1. Brooklyn
<br>2. Bronx
<br>3. EWR (Newark Liberty International Airport)
<br>4. Manhattan
<br>5. Staten Island
<br>6. Queens

# Goal / Tujuan
Dengan perusahaan dapat menganalisa keterkaitan `trip type` pada setiap wilayah dengan `rata rata total amount`, perusahaan dapat memiliki strategi bisnis terupdate dengan menyesuaikan fenomena real yang didapatkan.

## Secara garis besar :

    * Frekuensi trip type didominasi oleh trip type `1 = Street Hail` dengan percentage of total `98%` sendangkan trip type `2 = Dispatch` dengan percentage of total hanya `2%`.
    * Catatan perjalan terbanyak di borough `Manhattan` dan `Queens` tetapi `rata rata trip distance` tidak terlalu tinggi dan ini memungkinkan akan mempengaruhi `total amount` yang didapat setiap perjalanan.
    * Wilayah Manhattan dengan rata-rata total amount street hail paling rendah sebesar 20.61 USD dari wilayah lainnya dan dibawah rata-rata total amount street hail. Tip amount Manhattan tertinggi kedua sebesar 2.28 USD dari wilayah lainnya. Penumpang di wilayah Manhattan cukup royal dan banyak menggunakan kartu debit/kredit. Congestion surcharge tertinggi di wilayah Manhattan sebesar 1.05 USD mencerminkan Manhattan wilayah dengan Tingkat kemacetan yang tinggi.
    * Wilayah Manhattan dengan rata-rata total amount dispatch paling rendah sebesar 23.615 USD dari wilayah lainnya dan dibawah rata-rata total amount dispatch. Tip amount Manhattan hanya sebesar 0.86 USD dari wilayah lainnya. Penumpang pemesanan dispatch di wilayah Manhattan tidak terlalu royal dan penggunaan kartu debit/kredit masih kurang. Congestion surcharge tertinggi di wilayah Manhattan sebesar 0.45 USD mencerminkan Manhattan wilayah dengan Tingkat kemacetan yang tinggi.
    * Total pickup tertinggi pada trip type street hail di hari Tuesday/selasa sebesar 11028.
    Total pickup tertinggi pada trip type dispatch di hari Sunday/minggu sebesar 265.
    Terlihat pola penggunaan trip type street hail banyak digunakan pada weekday/hari kerja, sedangkan trip type dispatch banyak digunakan pada weekend/hari libur    
    

# Kesimpulan
**Number of Trip Type**
* Frekuensi trip type didominasi oleh trip type `1 = Street Hail` dengan percentage of total `98%` sendangkan trip type `2 = Dispatch` dengan percentage of total hanya `2%`.
* Kota new york dikenal sebagai kota dunia yang paling sibuk dan banyak sekali pusat distrik disana, namun pemesanan secara `street hail` paling banyak digunakan oleh pengguna TLC Trip.
* Berdasarkan Number of trip type didapat 2 borough dengan kepadatan tranportasi yang tinggi yaitu `Manhattan` dan `Queens`. Percent of total `Manhattan` dengan `Street Hail` sebesar `57.64%` dan `Queens` dengan `Street Hail` `25.41%`.
* `Dispatch` didominasi borough `Queens` dengan percent of total `1.03%` dan `Brooklyn` dengan percent of total `0.42%`. 

**Trip Distance**
* Rata rata trip distance berdasarkan street hail, `Bronx` dengan rata rata trip distance sejauh `116.03` paling tinggi, padahal sebelumnya jika dilihat dari number of street hail `Manhattan` tertinggi tetapi rata rata trip distance `Manhattan` ke-3. Menandakan bahwa karakteristik perjalanan di `Manhattan` yaitu penjelanan jarak dekat.  
* Rata rata trip distance berdasarkan dispatch,  `Brooklyn` dengan rata rata trip distance sejauh `3.63` paling tinggi, padahal sebelumnya jika dilihat dari number of street hail `Queens` tertingi tetapi rata rata trip distance `Queens` ke-3. Menandakan bahwa karakteristik perjalanan di `Queens` yaitu penjelanan jarak dekat.
* Catatan perjalan terbanyak di borough `Manhattan` dan `Queens` tetapi `rata rata trip distance` tidak terlalu tinggi dan ini memungkinkan akan mempengaruhi `total amount` yang didapat setiap perjalanan.

**Tip Amount**
* Berdasarkan trip type street hail, borough `Brooklyn` memiliki rata rata `tip amount``tertinggi` yaitu `2.73`. Jika dikorelasikan data sebelumnya rata rata trip distance `Brooklyn` yaitu `12.89` di urutan ke-2 maka mencerminkan behaviour penumpang trip type street hail di borough `Brooklyn` cukup royal kepada driver.
* Berdasarkan trip type street hail, borough `Bronx` memiliki rata rata `tip amount``terendah` yaitu `0.73`. Jika dikorelasikan data sebelumnya rata rata trip distance `Bronx` yaitu `116.03` di urutan ke-1 maka mencerminkan behaviour penumpang trip type street hail di borough `Bronx` tidak cukup royal kepada driver.
* Menghiligh borough `Queens` yang memiliki rata rata tip amount ke-3 berdasarkan street hail dan dispatch mencerminkan behaviour penumpang di `Queens` cukup royal. 

**Fare Amount**
* Pada trip type `Street hail`, borough `Staten Island` memiliki rata rata fare amount sebesar `24.35` `tertinggi` dikarenakan staten island merupakan daerah pinggiran new york namun sangat ekslusif dari segi pariwisata.
* Pada trip type `Dispatch`, borough `EWR` memiliki rata rata fare amount sebesar `180.0` `tertinggi` dikarenakan tarif dasar ke airport international ada biaya tambahan airport.
* Melihat rata rata fare amount paling rendah yaitu borough `Manhattan`. `Manhattan` banyak perjalanan dalam kota atau sekitarnya hanya melibatkan jarak pendek. Ini dapat menghasilkan fare amount yang relatif rendah meskipun tertinggi dalam frekuensi  perjalanan.

**Congestion Surcharge**
* Tiga borough dengan `rata rata congestion surcharge` tertinggi berdasarkan pemesanan trip type `street hail` di setiap `borough`:
  <br>1.`Manhattan` sebesar `1.05`.
  <br>2.`Brooklyn` sebanyak `0.37`.
  <br>3.`Queens` sebanyak `0.1`.

* Tiga borough dengan `rata rata congestion surcharge` tertinggi berdasarkan pemesanan trip type `dispatch` di setiap `borough`:
  <br>1.`Manhattan` sebesar `0.45`.
  <br>2.`Brooklyn` sebanyak `0.4`.
  <br>3.`Queens` sebanyak `0.09`.

* Melihat rata rata congestion surcharge 3 tertinggi berdasarkan street hail dan dispatch diisi oleh borough yang sama. Data tersebut mencerminkan bahwa borough tersebut merupakan daerah dengan kemacetan yang tinggi.

**Total Amount**
* Total amount tertinggi pada Trip Type street hail yaitu borough `Staten Island` sebesar `30.84`. 
* Total amount tertinggi pada Trip Type dispatch yaitu borough `EWR` sebesar `200.0`. 
* Melihat rata rata fare amount paling rendah yaitu borough `Manhattan` berdasarkan trip type street hail sebesar `20.61` dan dispatch sebesar `23.65` mencerminkan bahwa di Manhattan perjalanan taxi cenderung lebih murah atau kurang menghasilkan pendapatan dibandingkan dengan borough lainnya. 
* Kepadatan populasi yang tinggi di Manhattan, di mana perjalanan taxi mungkin lebih sering digunakan untuk perjalanan jarak pendek di sekitar wilayah tersebut. 
* Trip type `street hail` lebih umum digunakan untuk perjalanan jarak pendek di sekitar wilayah Manhattan. 
* Ini menunjukkan bahwa orang-orang cenderung menggunakan taksi secara spontan di jalanan Manhattan untuk perjalanan singkat atau tujuan terdekat.
* Disebabkan oleh kepadatan populasi yang tinggi dan infrastruktur transportasi yang padat di Manhattan, membuat penggunaan taksi untuk perjalanan jarak pendek menjadi lebih praktis dan efisien.

**Dayname**
* Total pickup tertinggi pada trip type street hail di hari `Tuesday/selasa` sebesar `11028`.
* Total pickup tertinggi pada trip type dispatch di hari `Sunday/minggu` sebesar `265`.
* Terlihat perbedaan signifikan bahwa penggunaan trip type street hail banyak digunakan pada weekday/hari kerja, sedangkan trip type dispatch banyak digunakan pada weekend/hari libur. 

# Rekomendasi

* **Penerapan diferensiasi tarif pada borough yang padat transportasi**
<br> Melihat tingginya pemesanan secara trip type street hail di borough manhattan sebesar 57.65% dan queens sebesar 25.41% mencerminkan 2 borough ini sangat padat transportasi , maka perlu adanya diferensiasi tarif seperti peningkatan fare amount pada borough yang padat transportasi agar menunjang kenaikan total amount pada setiap driver di borough tersebut. 
* **Meningkatkan layanan pada borough dengan persentase trip type dispatch yang tinggi**
<br> Walupun persentase antara street hail dan dispatch itu 98% banding 2%. 2% ini dapat terlihat peluang untuk meningkatkan layanan dispatch pada borough yang memiliki persentase dispatch tertinggi. Pada kasus ini borough Queens memiliki persentase dispatch tertinggi sebesar 1.038%. Jika pelayanan dispatch pada borough ini ditingkatkan maka akan menunjang pertambahan penumpang dan meningkatkan rata rata total amount yang di dapat driver. Cara ini dapat di implementasikan pada borough lainnya dengan menargetkan peningkatan penggunaan dispatch pada setiap borough di new york city.
* **Penerapan strategi bisnis berdasarkan hari**
<br> Telah terlihat pola penggunaan street hail dan dispatch dalam seminggu. Street hail rata rata digunakan pada weekday/hari kerja dan dispatch rata rata digunakan pada weekend/hari libur. Dengan mengetahui pola ini, perusahaan dapat membuat strategi bisnis berdasarkan hari, seperti promosi untuk pengguna taxi daily (target karyawan kantoran) dan promosi untuk penguna taxi dengan distance jauh , karna biasanya hari libur dipakai untuk perjalanan ke wilayah dengan distance yang jauh. Wilayah yang dapat diimplementasi dengan strategi bisnis pememberian promo di hari kerja seperti queens yang memiliki penggunaan trip type dispatch tertinggi yaitu 1.04%. Atau wilayah yang dapat diimplementasi dengan strategi bisnis berdasarkan hari dan trip distance ini seperti brooklyn yang memiliki rata rata trip ditasnce tertinggi yaitu 3.6 miles. Dengan mengetahui pola berdasarkan hari, dapat menunjang peningkatan rata rata total amount driver. 
