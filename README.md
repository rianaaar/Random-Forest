<h2> Classification of boarding house type using random forest </h2>

<h3> Dataset </h3>
Data yang digunakan pada analisis ini adalah data karakteristik kost - kost an yang terdiri dari 17 Variable yaitu sebagai berikut :<br>
<ul>
1.Id : id kost <br>
2.fac_1 - fac_8 : fasilitas kost <br>
3.poi_1 : jarak ke POI 1 <br>
4.poi_2 : jarak ke POI 2 <br>
5.poi_3 : jarak ke POI 3 <br>
6.size : luas kamar <br>
7.room_count : jumlah kamar <br>
8.total_call : jumlah pencarian ke kost tersebut <br>
9.gender : jenis gender yang ditampung oleh kost tersebut </ul>

<h3> Benefits of Analysis </h3>
Pertumbuhan sektor jasa ini telah berkembang ke berbagai bidang usaha, salah satunya adalah usaha rumah kost. Banyak faktor yang menjadi pertimbangan dalam memilih rumah kost misalnya lokasi yang strategis seperti dekat dengan kampus, tempat makan, warnet, fotocopy, shopping center, ataupun tempat-tempat hiburan lainnya. Oleh karena itu, untuk membangun kos kosan harus ditentukan apakah di suatu area itu cocok untuk dibangun kos putra, putri, atau campur berdasarkan faktor-faktor tersebut. Untuk mengetahui di suatu area itu cocok untuk dibangun kos putra, putri atau campur dilakukan pemodelan menggunakan algoritma random forest
<h3> Result </h3>
<p align="center">
<img src="fitur_imp.png">
<img src="tree.png">
</p>
Penjelasan rules dari Tree :<br>
<ul>
- tidak terdapat fasilitas 4 (fac_4)<br>
- jarak ke poi 3 >= 14610 <br>
- total pencarian < 4<br>
- harga bulanan < 425 000 <br>
maka jenis kosannya adalah untuk Putri</ul>
<ul>
- tidak terdapat fasilitas 4 (fac_4)<br>
- jarak ke poi 3 <= 14610<br>
- harga bulanan >= 1.275.000 <br>
- total pencarian < 4 <br>
maka jenis kosannya adalah utuk putra </ul>
<ul>
- tidak terdapat fasilitas 4 (fac_4) <br>
- jarak ke poi 3 <= 14610 <br>
- harga bulanan >= 1.275.000 <br>
- total pencarian > 4 atau <br>
- harga bulanan >= 425000 <br>
maka jenis kosannya adalah untuk campuran </ul>
</p>
<h3> Conclusion </h3>
Hasil diatas menunjukan bahwa jenis kosan sangat bergantung dengan harga bulanan kosan, ukuran kosan, faktor 4 ( fasilitas ke 4), jarak ke poi ke 3 dan banyak pencarian.

