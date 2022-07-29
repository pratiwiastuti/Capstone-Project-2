# Capstone-Project-2 by Pratiwi Astuti
----
# Crimes in Boston
## Latar Belakang
Departemen Kepolisian Boston (BPD) melaporkan bahwa banyaknya laporan insiden kajahatan baru dan telah mendokumentasikan rincian awal seputar insiden yang telah ditanggapi. BPD sudah memiliki kumpulan data kejahatan dan mereka ingin menganalisa apa saja yang harus di tingkatkan agar dapat mengurangi tindak kriminal dan menangkap pelaku kejahatan tersebut.
----
## Rumusan Masalah
- Kejahatan apa saja yang sering terjadi?
- Dimana kejahatan paling mungkin terjadi?
- Apakah frekuensi kejahatan berbuah seiring waktu?
----
## Data
Data dapat diakses di [sini](https://www.kaggle.com/datasets/AnalyzeBoston/crimes-in-boston). Berikut tahapan pengolahan data.
----
## Data Understanding dan cleaning
Dalam tahap ini kita cek data yang ada dan missing value perkolom. Selanjutnya kita dapat tangani data seperti anomali atau missing value. Dalam proses ini kita menerapkan 2 cara untuk missing value yaitu dengan mengisi data yang kosong seperti kolom SHOOTING dan mengapus data dengan missing value.
----
## Data Analysis
Setelah data bersih, tahap selanjutnya adalah menganalisa data agar dapat menjawab rumusan masalah yang ada. Dalam tahap ini, analisa menggunakan statistika deskriptif. Menurut [wikipedia](https://id.wikipedia.org/wiki/Statistika_deskriptif), statistika deskriptif adalah  metode-metode yang berkaitan dengan pengumpulan dan penyajian suatu himpunan data sehingga memberikan informasi yang berguna. Berikut analisa yang dilakukan:
### Berdasarkan nomor kejadian:  `INCIDENT_NUMBER`, `OCCURED_CODE_GROUP`, `OCCURED_ON_DATE`, `YEAR`, and `MONTH`.

Analisa ini untuk menjawab pertanyaan: *Kapan tindak kejahatan paling banyak terjadi?*
Hasil analisa dapat dilihat dari gambar:
![image](https://user-images.githubusercontent.com/107948562/181715259-98e39187-1eb2-4ad8-ab52-d856e29ee0b8.png), ![image](https://user-images.githubusercontent.com/107948562/181715793-37c48856-baf6-43b3-abe9-960b35bbc63b.png)
### Berdasarkan tempat kejadian:  `INCIDENT_NUMBER`, `DISTRICT`, `STREET`

Kita akan melihat dimana kejahatan sering terjadi dalam rentar waktu 2015 - 2018 dan ini akan menjawab pertanyaan: *Dimana tindak kejahatan paling banyak terjadi?*
Hasil analisa dapat dilihat dari visualisasi berikut:
![image](https://user-images.githubusercontent.com/107948562/181716192-e904b27d-78fa-40a9-8f65-ae3bd8a5ce48.png), ![image](https://user-images.githubusercontent.com/107948562/181716331-6f932bf2-63dc-4ba4-b007-e67bfc74d78d.png).
### Berdasarkan jenis kejahatan:  `OFFENSE_CODE_GROUP`, `DISTRICT`, `YEAR`, `MONTH`

Kita akan melihat jenis kejahatan apa saja yang sering terjadi dalam rentan waktu 2015 - 2018 dan ini akan menjawab pertanyaan: *Jenis kejahatan apa yang paling banyak terjadi?*
Berikut visualisasi dari data tersebut.
![image](https://user-images.githubusercontent.com/107948562/181716566-669bb382-c4e7-4fe2-907c-4f0b681c46cc.png).
----
## Kesimpulan dan Rekomendasi
Dari analisa yang telah kita lakukan, kita dapat membuat kesimpulan sebagai berikut:<br>
- Dari data diketahui bahwa kita memiliki 263,241 kasus pelanggaran kejahatan dari rentan tahun 2015-2018. Pelanggaran ini memiliki *INCIDENT_NUMBER* yang berbeda untuk tiap kasusnya.
- Kejahatan paling banyak terjadi pada tahun 2017, namun dalam dalam 2015 dan 2018 kita tidak memiliki data yang lengkap karena data tidak dihitung selama 1 tahun full.
- Frekuensi terjadinya kejahatan paling tinggi yaitu pada bulan Agustus.
- Frekunsi tertinggi terjadinya kejahatan dari sisi waktu/jam paling tinggi yaitu jam 17.00, kemudian disusul dengan jam 16.00 dan 18.00 .
- Persebaran terjadinya kejahatan di Boston apabila dilihat dari sisi hari yaitu persebaran hampir rata antara dengan nilai 12 - 15%, namun tertinggi terjadi pada hari Jumat dengan 15.2%.
- Kasus kejahatan tertinggi terjadi di jalan Washington ST dengan district B2.
- Kasus kejahatan yang paling sering terjadi adalah Motor Vehicle Accident Response.
- Part Three adalah UCR dengan kasus paling banyak selama 2015 - 2018.

**Rekomendasi**
1. Anggota kepolisian harus lebih fokus dengan kejahatan Motor Vehicle Accident Response karena merupakan kejahatan dengan kasus tertinggi. Kemudian dapat fokus kepada kejahatan seperti 
Larceny, Medical Assistance, Investigate Person, Vandalism,  Simple Assault, Verbal Disputes, Towed, Drug, Violation.
2. Kepolisian harus lebih menambahkan personil terutama pada district B2.
3. Memberikan himbauan kepada masyarakat sekitar untuk lebih berhati-hati terutama pada jam rawan dari jam 16.00 sampai malam hari.
4. Lebih ketat dalam menjaga jalan Washington St.

Dengan analisis ini diharapkan dapat membatu mengurangi tindak kejahatan di Boston.


