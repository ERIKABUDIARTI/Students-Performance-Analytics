# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan *Edutech*

## ***Business Understanding***

Bisnis *edutech* merupakan bagian dari sektor edukasi yang memanfaatkan teknologi *digital* untuk menyediakan solusi pendidikan inovatif. Dengan perkembangan teknologi *digital*, internet, dan perangkat *mobile*, *edutech* telah mengalami perkembangan pesat karena memungkinkan akses pendidikan yang lebih mudah, terjangkau, dan terpersonal secara global. Berikut adalah beberapa poin lebih detail mengenai perkembangan dan potensi bisnis pendidikan berbasis teknologi (*edutech*):

### Aksesibilitas Global 
Salah satu keunggulan utama *edutech* adalah kemampuannya untuk menyediakan akses pendidikan ke seluruh dunia. Dengan adanya internet, orang-orang dari berbagai latar belakang dan lokasi geografis dapat mengakses materi pembelajaran tanpa batasan fisik. Hal ini membuka pintu bagi pendidikan yang lebih inklusif dan merata di seluruh dunia.

### Pembelajaran Interaktif 
*Edutech* menyediakan *platform* pembelajaran yang interaktif dan menarik. Berbagai fitur seperti video pembelajaran, simulasi, *game* edukatif, dan diskusi *daring* meningkatkan keterlibatan siswa dalam proses pembelajaran. Ini membantu meningkatkan pemahaman dan retensi materi pelajaran.

### Pembelajaran Adaptif 
Fitur kunci *edutech* adalah kemampuannya untuk menyediakan pembelajaran yang adaptif. *Platform edutech* menggunakan teknologi seperti kecerdasan buatan (*AI*) dan analisis data untuk memahami gaya belajar dan kebutuhan individual siswa. Dengan demikian, siswa dapat belajar sesuai dengan kecepatan dan gaya belajar mereka sendiri.

### Personalisasi 
*Edutech* memungkinkan personalisasi pembelajaran yang lebih baik. Dengan menganalisis data tentang kemajuan belajar dan preferensi siswa, *platform edutech* dapat menyajikan materi yang sesuai dengan kebutuhan individu. Ini memungkinkan pengalaman belajar yang lebih efektif dan efisien.

### Peluang Bisnis 
Pertumbuhan pesat dalam pendidikan berbasis teknologi (*edutech*) menawarkan banyak peluang bisnis yang menjanjikan. Mulai dari pengembangan *platform* pembelajaran, konten *digital*, solusi manajemen sekolah, hingga pelatihan guru dan konsultasi edukasi, ada banyak area di mana perusahaan dapat berinovasi dan berkontribusi dalam transformasi pendidikan global.

### Kolaborasi dengan Institusi Pendidikan 
Banyak perusahaan bekerja sama dengan institusi pendidikan formal seperti sekolah dan perguruan tinggi untuk menyediakan solusi pendidikan yang terintegrasi. Ini menciptakan peluang kolaborasi yang saling menguntungkan dan memperluas jangkauan bisnis pendidikan berbasis teknologi (*edutech*).


## **Permasalahan Bisnis**

Jaya Jaya Institut merupakan salah satu institusi pendidikan perguruan berciri khas *EduTech* yang telah berdiri sejak tahun 2000. Hingga saat ini ia telah mencetak banyak lulusan dengan reputasi yang sangat baik. Akan tetapi, terdapat banyak juga siswa yang tidak menyelesaikan pendidikannya alias *dropout*.

Jumlah *dropout* yang tinggi ini tentunya menjadi salah satu masalah yang besar untuk sebuah institusi pendidikan. Oleh karena itu, Jaya Jaya Institut ingin mendeteksi secepat mungkin siswa yang mungkin akan *dropout* sehingga dapat diberi bimbingan khusus.


## **Cakupan Proyek**

Untuk mengatasi permasalahan *dropout* siswa dalam pendidikannya, akan digunakan pendekatan dan metode/teknik berikut:

### Pemahaman Data (*Data Understanding*)
- Mengumpulkan data historis mengenai informasi profil siswa, performa belajar siswa dan faktor-faktor lain yang terkait.
- Mempelajari tipe dan karakteristik *dataset*.

### Persiapan Data (*Data Preparation*)
- Membersihkan dan mengolah data untuk mengatasi *missing values*, data duplikat, dan masalah lain yang mungkin mempengaruhi kualitas analisis.
- Melakukan proses transformasi data seperti *encoding* kategori, normalisasi, dan pemilihan fitur yang relevan untuk analisis.
- Menjelajahi korelasi antar variabel untuk memahami hubungan di antara variabel-variabel tersebut.

### *Machine Learning Modeling*
- Memisahkan data menjadi *training set* dan *testing set*.
- Melatih beberapa model menggunakan *training set*, dengan variabel target *status* dan variabel fitur yang relevan.
- Menyesuaikan *hyperparameter* model dan melakukan validasi model.

### *Evaluation*
- Menggunakan *testing set* untuk mengevaluasi kinerja model dengan metrik yang sesuai seperti *accuracy*, *precision*, *recall* dan *F1-score*.

### *Deployment*
- Menjalankan model *Logistic Regression* yang telah dibuat ke dalam lingkup produksi sehingga *user* dapat berinteraksi dengan model.


## **Persiapan**

Sumber data: 
UCI Machine Learning Repository https://doi.org/10.24432/C5MC89

*Setup environment*:
```
pip install numpy pandas matplotlib seaborn scikit-learn==1.6.1 joblib==1.4.2 streamlit==1.34.0
```


## ***Business Dashboard***

*Dashboard* dibuat dengan menggunakan *Google Looker Studio* untuk menampilkan distribusi data dan pengaruh variabel-variabel data terhadap *Student Performance*. *Dashboard* dapat diakses pada *link* berikut ini:
```
https://lookerstudio.google.com/reporting/6f1ee678-dc05-4167-9fbd-7521390e018d
```
![erika_budiarti-dashboard](https://raw.githubusercontent.com/ERIKABUDIARTI/Students-Performance-Analytics/main/erika_budiarti-dashboard.png)


## **Menjalankan Sistem *Machine Learning***

*Prototype* Sistem *Machine Learning* ini dibuat dengan *Streamlit* yang dapat diakses pada *link* berikut ini:
```
https://students-performs.streamlit.app/
```
![erika_budiarti-streamlit](https://raw.githubusercontent.com/ERIKABUDIARTI/Students-Performance-Analytics/main/erika_budiarti-streamlit.png)

Cara menjalankan Aplikasinya adalah sebagai berikut
1. Isi form sesuai data mahasiswa, seperti *Tuition Fees*, *Scholarship Holder*, *Gender*, *Attendance*, dan seterusnya
2. Klik tombol *Click Here to Predict*
3. Hasil prediksi akan muncul di bawahnya (*Graduate* / *Not Graduate*). 


## ***Conclusion***

- Komposisi siswa terdiri dari 66% Laki-laki dan 34% Perempuan dengan distribusi usia tertinggi pada rentang 17-23 tahun.
- Tingkat kelulusan siswa (*Graduation Rate*) sebesar 60.85%% sedangkan tingkat ketidaklulusan (*Dropout Rate*) sebesar 39,14% dari 3.630 siswa
- Tingkat ketidaklulusan cukup seimbang antara siswa Laki-laki (19.83%) dan siswa Perempuan (19.31%)
- Dari 969 penerima beasiswa terdapat 134 siswa yang *dropout* (13.83%) dan 835 siswa yang berhasil lulus (86.17%)
- Dari 1.421 siswa yang *dropout* terdapat 1.214 siswa (85.43%) yang mengikuti kelas pagi dan 207 siswa (14.57%) yang mengikuti kelas malam
- Selain itu, faktor *curricular units* dan *tuition fees* juga cukup berpengaruh pada tingkat kelulusan siswa.


### **Rekomendasi *Action Items***

Beberapa rekomendasi *action items* yang harus dilakukan institusi guna menyelesaikan permasalahan atau mencapai target mereka.

- Memberikan bimbingan dan dukungan tambahan kepada siswa penerima beasiswa untuk membantu mereka mengatasi tantangan akademik dan non-akademik.
- Meninjau kembali kurikulum yang ada untuk memastikan bahwa apakah masih relevan, menantang, dan sesuai dengan kebutuhan siswa.
- Menyediakan tutor atau mentor, kelas remedial, bimbingan akademik, dan dukungan psikologis bagi siswa yang membutuhkannya.
- Mengembangkan program pendidikan / kelas alternatif yang dapat menjangkau siswa yang mungkin kesulitan menghadiri kelas pada waktu reguler, seperti program jarak jauh.
