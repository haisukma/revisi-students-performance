# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

* Nama : Diajeng Mahai Sukma
* email : diajengmahaih@gmail.com
* ID : sukmaa

## Business Understanding
**Jaya Jaya Institut** adalah sebuah institusi pendidikan tinggi yang telah berdiri sejak tahun 2000. Selama lebih dari dua dekade, institusi ini telah berhasil mencetak banyak lulusan dengan reputasi yang sangat baik di berbagai bidang. Namun, seperti banyak institusi pendidikan lainnya, Jaya Jaya Institut juga menghadapi tantangan yang signifikan terkait dengan tingginya tingkat siswa yang tidak menyelesaikan pendidikannya alias dropout.

**Masalah dropout** ini merupakan masalah yang serius bagi institusi pendidikan, karena dropout yang tinggi dapat mempengaruhi citra institusi, mengurangi tingkat kelulusan, dan pada akhirnya berdampak pada daya tarik institusi bagi calon siswa di masa mendatang. Tingkat dropout yang tinggi juga bisa menjadi indikasi bahwa ada masalah mendasar dalam proses penerimaan siswa, pembelajaran, atau dukungan akademik yang disediakan oleh institusi.

### Permasalahan Bisnis
Masalah bisnis yang ingin diselesaikan adalah sebagai berikut:
1. Bagaimana cara mengidentifikasi mahasiswa yang berpotensi dropout sejak dini?
2. Apasaja faktor yang menyebabkan siswa tidak menyelesaikan pendidikannya (dropout)?
3. Tindakan apa yang dapat dilakukan untuk mengurangi mahasiswa dropout dan memastikan lebih banyak mahasisawa yang menyelesaikan pendidikannya?

### Cakupan Proyek
Berikut cakupan proyek yang telah dikerjakan:
* Eksplorasi dan Analysis Data : Melakukan eksplorasi pada data yang sudah diperoleh agar dapat mendapatkan gambaran umum tentang data. Selanjutnya melakukan analysis untuk mengidentifikasi faktor yang mempengaruhi mahasiswa dropout
* Visualisasi Data : Membuat dashboard laporan untuk memonitor dan menganalissis mahasiswa yang berpotensi dropout
* Model dan Rekomendasi : Membangun model klasifikasi untuk melakukan rekomendasi yang dapat dilakukan untuk mengurangi droput.

### Persiapan

Sumber data: dataset yang digunakan merupakan dataset [Jaya Jaya Institut](https://github.com/dicodingacademy/dicoding_dataset/tree/main/students_performance).

* Setup environment:
    ```
    conda create --name proyek-institusi-pendidikan python==3.9.15
    ```
* Install requirements: 
    ```
    pip install -r requirements.txt
    ```


## Business Dashboard
Berikut adalah dashboard yang telah dibuat:

Dashboard ini dirancang untuk memberikan wawasan komprehensif kepada institut terhadap faktor-faktor yang berkontribusi dengan `Status` baik dropout, enrolled, ataupun graduated. Dengan dashboard ini tim institut dapat :
1. Memantau Tingkat Dropout Secara Proaktif:
    - Melalui visualisasi persentase siswa yang dropout, enrolled, dan graduate, tim dapat memantau tren dropout secara real-time. Ini memungkinkan institusi untuk segera mengambil tindakan jika terlihat ada peningkatan signifikan dalam tingkat dropout.

2. Menganalisis Faktor-Faktor yang Mempengaruhi Dropout:
    - Dengan analisis mendalam tentang bagaimana faktor-faktor seperti nilai akademik, beasiswa, biaya pendidikan, dan kualifikasi orang tua mempengaruhi status siswa, tim dapat mengidentifikasi elemen-elemen yang paling berisiko bagi siswa. Ini memungkinkan penyesuaian kebijakan dan intervensi yang lebih tepat sasaran.

    <img src="https://raw.githubusercontent.com/haisukma/newstudents-s-performance/master/image/sukmaa-dashboard.png" width="500">

    Atau buka [tautan](https://lookerstudio.google.com/reporting/4f9dfd87-fb11-4937-ba1f-e551a2571ee9) untuk membuka dashboard yang ada di looker studio.

## Menjalankan Sistem Machine Learning
Pada proyek ini telah disediakan sebuah prototype untuk melakukan prediksi terhadap model yang sudah dibuat. Untuk menjalankan protoype secara lokal jalankan perintah berikut di terminal: 

```
streamlit run app.py
```
Atau buka pada tautan [berikut](https://revisi-students-performance-5zuzvcwrxldet2cquwprvb.streamlit.app/) untuk membuka prototype yang sudah dijalankan pada streamlit community.
 <img src="https://raw.githubusercontent.com/haisukma/newstudents-s-performance/master/image/sukmaa-prototype.png" width="500">

## Conclusion
Proyek ini bertujuan untuk mengatasi masalah utama yang dihadapi Jaya Jaya Institut terkait tingkat dropout siswa. Berikut adalah rangkuman proyek ini:

1. Bagaimana cara mengidentifikasi siswa yang berpotensi dropout sejak awal?

- Dengan mengembangkan model prediktif berbasis algoritma seperti Random Forest, Desesion Tree maupun algoritma XGBoost Jaya Jaya Institut dapat mengenali siswa yang berisiko dropout lebih dini. Model ini mampu mendeteksi siswa berisiko dengan tingkat akurasi yang baik berdasarkan data historis serta faktor-faktor yang berkaitan.
  
2. Apasaja faktor yang menyebabkan siswa tidak menyelesaikan pendidikannya (dropout)?
- Faktor yang paling berpengaruh terhadap keputusan mahasiswa untuk dropout berdasarkan analisis korelasi dan penilaian fitur dalam model prediktif menunjukkan bahwa latar belakang akademik (seperti nilai dan jumlah mata kuliah yang diambil) serta kondisi ekonomi (seperti beasiswa atau keadaan sosial-ekonomi yang kurang stabil). Contohnya siswa yang mengalami kesulitan akademik pada semester awal cenderung memiliki risiko dropout lebih tinggi.

 <img src="https://raw.githubusercontent.com/haisukma/newstudents-s-performance/master/image/sukmaa-korelasi.png" width="500">

3. Tindakan apa yang dapat dilakukan untuk mengurangi mahasiswa dropout dan memastikan lebih banyak mahasisawa yang menyelesaikan pendidikannya?

- Jaya Jaya Institut dapat mengurangi mahasiswa dropout dan memastikan lebih banyak mahasisawa yang menyelesaikan pendidikannya dengan beberapa strategi berdasarkan temuan dari model dan analisis data. Hal yang dapat dilakukan dengan menyesuaikan kurikulum untuk mengurangi beban siswa, menyediakan bimbingan akademik yang lebih intensif, dan memberikan dukungan finansial tambahan kepada siswa yang membutuhkan atau berprestasi. Analisa lebih dini dengan data dapat membantu memastikan lebih banyak siswa menyelesaikan pendidikan mereka.

### Rekomendasi Action Items
Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.
Bimbingan Akademik yang Intensif:

1. Sediakan sesi bimbingan akademik lebih intensif, terutama bagi mahasiswa yang berada dalam semester awal dan yang memiliki nilai rendah. Fokus pada memberikan dukungan di bidang yang mereka kesulitan. Mahasiswa yang mengalami masalah akademik dan pribadi, seperti yang tercermin dari faktor status pernikahan, mungkin memerlukan dukungan psikologis lebih besar. Universitas dapat menyediakan layanan konseling atau workshop terkait manajemen stres dan keterampilan belajar
   
2. Gunakan data dari analisis dropout (seperti yang terlihat dari marital status, beasiswa, atau hasil akademik) untuk mengidentifikasi mahasiswa berisiko sejak awal. Intervensi dapat dilakukan melalui konseling atau memberikan akses lebih besar ke sumber daya belajar. Buat sistem monitoring berkala untuk melihat perkembangan akademik setiap mahasiswa. Mahasiswa yang terdeteksi mengalami penurunan performa atau memiliki tanda-tanda ingin dropout dapat segera diintervensi dengan cara yang tepat.
   
3. Berdasarkan analisis penerima beasiswa, universitas perlu meningkatkan dukungan finansial, terutama bagi mahasiswa dari keluarga dengan kondisi ekonomi sulit. Tambahkan skema beasiswa atau bantuan biaya pendidikan.
   
4. Kurangi beban akademik untuk mahasiswa dengan kinerja rendah, terutama di semester awal. Misalnya, menawarkan pilihan untuk mengambil lebih sedikit mata kuliah atau memberikan opsi remedial untuk mata kuliah yang paling sering diambil oleh mahasiswa dropout, seperti yang teridentifikasi di dashboard.
   
5. Berdasarkan data mata kuliah yang paling sering diambil mahasiswa dropout (seperti Management dan Nursing), universitas dapat mereview kembali metode pengajaran dan beban kerja pada mata kuliah ini. Ini dapat berupa perubahan metode pengajaran, pengurangan beban kurikulum, atau menawarkan lebih banyak sumber belajar tambahan.