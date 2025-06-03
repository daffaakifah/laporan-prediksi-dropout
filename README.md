# Proyek Akhir: Menyelesaikan Permasalahan Institusi Pendidikan <br>
### Jaya Jaya Institut - Oleh Daffa Akifah

## Business Understanding
Jaya Jaya Institut merupakan institusi pendidikan tinggi yang telah berdiri sejak tahun 2000 dan dikenal luas berkat reputasinya dalam mencetak lulusan berkualitas. Namun, di balik prestasi tersebut, institusi ini menghadapi tantangan serius berupa tingginya angka siswa yang tidak menyelesaikan studi alias dropout. Fenomena ini menjadi perhatian utama karena dapat berdampak negatif terhadap citra institusi, efektivitas proses belajar-mengajar, serta efisiensi penggunaan sumber daya.

Tingginya tingkat dropout tidak hanya merugikan institusi, tetapi juga para siswa yang gagal meraih gelar dan masa depan yang lebih baik. Oleh karena itu, Jaya Jaya Institut berupaya untuk mendeteksi secara dini siswa yang berpotensi mengalami dropout. Dengan deteksi dini, institusi dapat memberikan pencegahan, penanganan, dan bimbingan khusus agar siswa tersebut tetap termotivasi dan mampu menyelesaikan pendidikannya.

Sebagai bagian dari upaya ini, Jaya Jaya Institut menyediakan dataset performa siswa sebagai upaya untuk mendapatkan solusi berbasis data science. Solusi yang diharapkan meliputi pembuatan model prediksi dropout serta dashboard interaktif yang dapat membantu pihak institusi dalam memahami pola data, memonitor performa mahasiswa secara real-time, dan mengambil keputusan berbasis data untuk menekan angka dropout.

### Permasalahan Bisnis
Berikut adalah permasalahan bisnis utama yang dihadapi oleh Jaya Jaya Institut dan menjadi fokus penyelesaian dalam proyek ini: <br>
1. **Tingginya Tingkat Dropout Siswa** <br>
   Jaya Jaya Institut menghadapi tantangan serius berupa tingginya angka siswa yang tidak menyelesaikan studi (dropout). Hal ini berdampak negatif pada citra institusi, efektivitas     proses belajar-mengajar, serta efisiensi penggunaan sumber daya.
2. **Kurangnya Pemahaman Faktor Penyebab Dropout** <br>
   Pihak institusi belum memiliki pemahaman yang mendalam mengenai faktor-faktor utama yang menyebabkan siswa mengalami dropout, sehingga sulit untuk melakukan pencegahan dan   penanganan yang tepat dan efektif.
3. **Kesulitan dalam Monitoring dan Pengambilan Keputusan** <br>
   Institusi kesulitan dalam memonitor performa siswa secara real-time dan mengidentifikasi siswa yang berisiko tinggi dropout tanpa alat bantu visualisasi dan  analisis data yang memadai.
4. **Kebutuhan Model Prediksi untuk Identifikasi Risiko Dropout** <br>
   Institusi membutuhkan model prediksi yang dapat mengidentifikasi siswa yang berpotensi tinggi mengalami dropout, sehingga pencegahan dan penanganan serta bimbingan dapat diberikan lebih awal untuk meningkatkan tingkat kelulusan.
5. **Optimalisasi Pengelolaan Sumber Daya Pendidikan** <br>
   Dengan memahami faktor-faktor yang mempengaruhi dropout dan memonitor kondisi siswa secara efektif, institusi dapat mengoptimalkan strategi pengelolaan sumber daya, termasuk kebijakan akademik, bimbingan, dan dukungan siswa.

### Cakupan Proyek
#### Tujuan Penyelesaian
1. **Mengidentifikasi faktor-faktor utama yang mempengaruhi dropout siswa di Jaya Jaya Institut.** 
2. **Membuat dashboard interaktif** yang menampilkan indikator kunci dan visualisasi terkait performa siswa serta risiko dropout untuk membantu manajemen dan guru dalam pengambilan keputusan.  
3. **Mengembangkan model prediksi dropout** yang akurat untuk mengantisipasi risiko siswa tidak menyelesaikan studi.  
4. **Memberikan rekomendasi strategis berbasis data** untuk menurunkan tingkat dropout dan meningkatkan tingkat kelulusan siswa.

#### Batasan Proyek
1. Proyek ini fokus pada analisis data historis dan prediksi dropout berdasarkan data yang tersedia.
2. Tidak mencakup intervensi langsung atau implementasi kebijakan akademik.
3. Model prediksi bersifat probabilistik dan memerlukan evaluasi serta penyempurnaan berkelanjutan untuk menjaga akurasi di masa depan.

#### Hasil yang Diharapkan
1. Pemahaman yang lebih baik tentang faktor-faktor yang mempengaruhi dropout siswa.
2. Dashboard monitoring yang efektif dan mudah digunakan oleh pihak institusi.
3. Model prediksi yang dapat membantu mengidentifikasi siswa berisiko tinggi untuk dropout.
4. Rekomendasi strategis berbasis data untuk meningkatkan tingkat kelulusan dan menurunkan angka dropout.

### Persiapan
#### Sumber data
Dataset yang digunakan dalam proyek ini adalah dataset dari instruksi submission yaitu dataset [Performa Siswa Jaya Jaya Institut](https://github.com/dicodingacademy/dicoding_dataset/blob/main/students_performance/data.csv).

#### Setup environment
1. Menjalankan notebook.ipynb <br>
   - File notebook.ipynb dapat dijalankan dalam visual studio atau IDE sejenis.
   - Pastikan dependensi, paket, dan library yang dibutuhkan telah tersedia. Daftar dependensi lengkap dapat dilihat pada file 
     requirements.txt yang disediakan dalam proyek. <br>
   - Jalankan seluruh isi notebook.ipynb di Google Colab atau IDE sejenis.
     Ini akan menampilkan hasil analisis data, temuan, pemodelan untuk prediksi data, serta insight yang diperoleh dari eksplorasi dan pemodelan data.
2. Menjalankan app.py <br>
   - File app.py dapat dijalankan dalam visual studio atau IDE sejenis.
   - Pastikan semua dependensi sudah terinstal, terutama streamlit. Gunakan perintah berikut untuk instalasi jika belum:
       ```
        pip install -r requirements.txt
        ```
   - Pastikan file app.py, model.pkl, dan file dataset 'data_enrolled.csv' berada dalam folder/direktori yang sama.
   - Jalankan aplikasi dashboard dengan perintah berikut di terminal atau command prompt:
       ```
       streamlit run app.py
       ```
    - Hasil prediksi serta dari model yang dikembangkan dalam proyek ini dapat langsung diakses di [Prediksi Dropout Siswa](https://prediksi-dropout-daffaab.streamlit.app/).
 3. Menjalankan Dashboard di Looker Studio
    - Menyiapkan data yang perlu digunakan yaitu dataset 'data_dropout_graduated.csv'
    - Buka looker studio (lookerstudio.google.com)
    - Upload dataset bisa digunakan dengan opsi pilihan Upload File CSV.
    - Pilih Visualisasi yang cocok dan sesuai dengan data.
    - Dashboard yang sudah dibuat dengan langkah-langkah di atas dalam proyek ini dapat diakses [dashboard-dropout-graduate](https://lookerstudio.google.com/reporting/36b418df-6fd8-47ad-888b-99a3ea0d5259).
    - Dashboard Looker Studio ini akan menjadi pusat monitoring real-time untuk Institusi berdasarkan data prediksi dan data historis.

## Business Dashboard
#### Ringkasan Dashboard
Dashboard ini memantau performa siswa Jaya Jaya Institut dengan fokus pada status kelulusan dan dropout. Dataset mencakup 3.630 siswa yang dianalisis berdasarkan berbagai indikator kunci. Dari total tersebut, 60.9% siswa lulus (graduate) dan 39.1% mengalami dropout. Dashboard menyediakan informasi visual yang menggambarkan perbedaan performa akademik, kepatuhan pembayaran, serta penerimaan beasiswa antara kelompok graduate dan dropout. Dashboard dapat diakses pada link berikut [dashboard-dropout-graduate](https://lookerstudio.google.com/reporting/36b418df-6fd8-47ad-888b-99a3ea0d5259)

#### Faktor Utama Dropout
Beberapa faktor utama yang berpengaruh terhadap dropout siswa adalah:
- Tingkat Penyelesaian Tahun Pertama: Siswa yang menyelesaikan 90% unit kurikulum di tahun pertama berpeluang lulus, sedangkan yang hanya menyelesaikan sekitar 34% unit cenderung dropout.
- Pembayaran Biaya Tepat Waktu: Siswa yang tepat waktu membayar biaya lebih besar kemungkinannya untuk lulus (graduate), sementara siswa yang terlambat atau tidak membayar tepat waktu cenderung mengalami dropout.
- Rata-Rata Nilai Tahun Pertama: Siswa yang lulus memiliki nilai rata-rata di tahun pertama (semester 1 & 2) sebsesar (63,39), jauh lebih tinggi dibandingkan siswa yang dropout dengan rata-rata (38,95).
- Penerima Beasiswa: Siswa yang menerima beasiswa memiliki tingkat kelulusan yang lebih tinggi dibandingkan yang tidak menerima beasiswa.
- Jumlah Unit Kurikulum Tahun Pertama yang diterima: Siswa dengan jumlah unit kurikulum yang diterima pada tahun pertama yang sedikit memiliki kemungkinan untuk dropout.

#### Distribusi dan Pola Siswa Dropout
- Siswa yang lulus lebih sering membayar biaya tepat waktu dibanding siswa yang dropout.
- Siswa dropout lebih banyak tidak membayar tepat waktu.
- Penerima beasiswa memiliki peluang lebih besar untuk lulus.
- Semakin tinggin tingkat penyelesaian unit kurikulum pada tahun pertama cenderung untuk lulus

#### Analisis Kurikulum Tahun Pertama
- Siswa yang mengikuti dan menyelesaikan unit kurikulum antara 10-15 unit pada tahun pertama lebih banyak ditemukan di kedua kelompok, namun nilai dan tingkat penyelesaian unit sangat membedakan antara graduate dan dropout.
- Tingkat penyelesaian unit kurikulum pada tahun pertama graduate sangat tinggi (90%), sedangkan dropout sangat rendah (34%).
- Tingkat unit kurikulum yang disetujui pada tahun pertama pada siswa dropout cenderung lebih sedikit dibandingkan yang graduate.
  
#### Prediksi Model
##### Performa model
Model yang digunakan menggunakan Model Gradient Boosting mneghasilkan akurasi 90.77%, dengan hasil prediksi sebagai berikut: <br>
![image](https://github.com/user-attachments/assets/bec89bc7-a7ce-4c87-b05f-4234f3940c74) <br>

Model Gradient Boosting berhasil mengklasifikasikan dengan cukup baik, dengan 237 Dropout dan 422 Graduate yang terdeteksi benar, serta kesalahan prediksi yang relatif kecil, yaitu 40 Dropout salah diklasifikasikan sebagai Graduate dan 27 Graduate salah diklasifikasikan sebagai Dropout.


##### Contoh tampilan hasil prediksi berdasarkan faktor di app.py
- Halaman awal dan header
![image](https://github.com/user-attachments/assets/c4d66a01-ca74-4e1c-8fd6-55aebcb1a85f)

- Prediksi siswa yang berstatus enrolled:
  ![image](https://github.com/user-attachments/assets/d7b5638a-e69f-4e30-8760-ccb43b495c67) <br>

  Prediksi siswa yang akan dropout berdasarkan dataset data_enrolled.csv

- Prediksi siswa dropout berdasarkan input
  ![image](https://github.com/user-attachments/assets/c2a074aa-d346-40de-9a9f-8fd91ed9dc34) <br>
  ![image](https://github.com/user-attachments/assets/3ef3e84a-f186-4226-a8c5-a6dc7e777fdf) <br>
  ![image](https://github.com/user-attachments/assets/ea986bd0-acad-4425-bac9-0f3f54de9faf) <br>

  Prediksi siswa yang akan dropout berdasarkan data dari input pengguna serta rekomendasi aksi lanjutan apabila siswa tersebut terindikasi akan dropout.
  
## Conclusion
### Faktor penting
Berikut adalah poin-poin penting yang dihasilkan dari analisis data dan pemodelan:
- Tingkat Penyelesaian Tahun Pertama menjadi indikator penting. Mahasiswa yang menyelesaikan sekitar 90% unit kurikulum tahun pertama berpeluang lulus, sementara mahasiswa yang menyelesaikan sekitar 34% unit cenderung dropout.
- Rata-rata Nilai Tahun Pertama juga sangat berpengaruh. Mahasiswa dengan nilai tahun pertama tinggi (sekitar 63,35) memiliki peluang lulus yang lebih besar dibandingkan mahasiswa dengan nilai rendah (sekitar 32,89) yang cenderung dropout.
- Pembayaran Biaya Tepat Waktu adalah faktor yang signifikan yang memengaruhi status mahasiswa. Mahasiswa yang membayar biaya tepat waktu memiliki peluang lebih besar untuk lulus, sedangkan mahasiswa yang terlambat atau tidak membayar tepat waktu cenderung mengalami dropout.
- Penerima Beasiswa meningkatkan kemungkinan kelulusan. Mahasiswa penerima beasiswa memiliki tingkat kelulusan yang lebih tinggi dibandingkan yang tidak menerima beasiswa.
- Nilai Masuk juga sedikit berpengaruh, dengan mahasiswa yang lulus memiliki nilai masuk rata-rata lebih tinggi (64,4) dibandingkan yang dropout (62,48).
- Dari distribusi data, mahasiswa yang membayar tepat waktu dan menerima beasiswa memiliki peluang lebih besar untuk berhasil, sedangkan pembayaran yang terlambat terhubung dengan risiko dropout yang tinggi.
- Fokus pada tahun pertama sangat penting karena nilai dan penyelesaian tahun pertama menjadi salah satu faktor untuk memprediksi keberhasilan atau kegagalan mahasiswa dalam masa studi mereka.

### Rekomendasi Action Items 
Rekomendasi action items untuk mengatasi tingkat dropout dan meningkatkan tingkat kelulusan siswa:
1. Bantuan Akademik <br>
Berikan bimbingan belajar tambahan secara intensif bagi siswa dengan nilai rendah atau yang menunjukkan tanda-tanda kesulitan akademis. Sediakan sesi konsultasi akademik rutin untuk membantu siswa merencanakan dan memperbaiki strategi belajarnya. Selain itu, lakukan monitoring progres belajar secara berkala agar setiap kendala akademik dapat segera terdeteksi dan diatasi secara tepat waktu.
2. Dukungan Finansial <br>
Tinjau kembali dan perluas kemungkinan pemberian siswa maupun bantuan biaya khususnya bagi siswa yang memiliki kendala finansial. Dukungan finansial ini tidak hanya mengurangi beban ekonomi siswa, tetapi juga dapat meningkatkan motivasi dan fokus mereka dalam menyelesaikan pendidikan. Pastikan proses pengajuan dan pencairan bantuan biaya ini mudah diakses dan tidak berbelit.
3. Konseling Psikologis <br>
Sediakan layanan konseling psikologis yang mudah dijangkau untuk siswa yang menghadapi masalah pribadi, stres, atau kehilangan motivasi. Konseling ini bertujuan memberikan dukungan mental dan emosional agar siswa tetap kuat dan termotivasi menghadapi tantangan selama masa pendidikan. Jangan lupa untuk mengedukasi siswa mengenai pentingnya kesehatan mental sebagai bagian dari kesuksesan akademik.
4. Peningkatan Keterlibatan <br>
Ajak siswa untuk aktif berpartisipasi dalam berbagai kegiatan kampus seperti organisasi, kelompok studi, maupun kegiatan sosial. Keterlibatan ini dapat memperkuat rasa kebersamaan dan dukungan antar sesama siswa sehingga menciptakan lingkungan belajar yang positif dan menyenangkan. Siswa yang terlibat secara aktif diharapkan cenderung memiliki semangat yang lebih tinggi dan risiko dropout yang lebih rendah.

### Kesimpulan akhir
Laporan ini dilatarbelakangi oleh Jaya Jaya Institut yang menghadapi tantangan serius dengan tingginya angka siswa yang dropout, yang berdampak negatif pada citra dan efektivitas institusi. Untuk mengatasi hal ini, institusi berfokus pada deteksi dini siswa berisiko melalui analisis data performa dan menyediakan model prediksi serta dashboard interaktif. Dari hasi; analisis ditemukan faktor utama dropout meliputi aspek akademik dan finansial, sehingga rekomendasi aksi meliputi bantuan belajar, dukungan biaya, layanan konseling, dan peningkatan keterlibatan kampus. Dengan strategi ini, diharapkan tingkat kelulusan meningkat dan angka dropout dapat ditekan secara signifikan.
