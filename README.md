1. **Performance Testing (JMeter) vs Profiling (IntelliJ Profiler)**
   Perbedaan utama antara performance testing menggunakan JMeter dan profiling menggunakan IntelliJ Profiler terletak pada pendekatan analisis yang digunakan. JMeter merupakan metode external/black-box testing yang menilai performa aplikasi dari sisi luar tanpa melihat implementasi kode. Fokusnya adalah pada bagaimana sistem berperilaku di bawah beban, seperti jumlah pengguna, waktu respons, throughput, dan tingkat error. Sebaliknya, IntelliJ Profiler merupakan metode internal/white-box analysis yang menganalisis aplikasi dari dalam saat runtime. Profiler ini digunakan untuk memahami secara detail bagian kode, proses, atau query yang menyebabkan penurunan performa.


2. **Identifikasi Titik Lemah melalui Profiling**
   Proses profiling membantu dalam mengidentifikasi titik lemah dalam aplikasi dengan memberikan visibilitas yang lebih dalam terhadap eksekusi program. Melalui visualisasi seperti flame graph atau call tree, developer dapat mengetahui method mana yang paling banyak menggunakan CPU atau memori. Selain itu, profiling juga membantu mendeteksi masalah seperti memory leak, yaitu kondisi ketika objek terus dibuat tetapi tidak dihapus. Dengan demikian, profiling tidak hanya menunjukkan bahwa suatu fitur lambat, tetapi juga menjelaskan penyebab spesifik di balik lambatnya eksekusi tersebut


3. **Efektivitas IntelliJ Profiler**
   IntelliJ Profiler menurut saya cukup efektif dalam membantu analisis dan identifikasi bottleneck pada kode aplikasi. Hal ini karena profiler tersebut terintegrasi langsung dengan IDE sehingga hasil analisis dapat langsung dikaitkan dengan source code. Selain itu, penggunaan Async Profiler dengan overhead yang rendah membuat proses pengamatan tidak terlalu mengganggu performa aplikasi, sehingga hasil yang diperoleh tetap cukup representatif terhadap kondisi sebenarnya.


4. **Tantangan Utama dan Solusi**
   Dalam proses performance testing dan profiling, terdapat beberapa tantangan yang umum dihadapi. Salah satunya adalah munculnya Heisenbug, yaitu kondisi ketika masalah performa tidak terlihat saat profiling dilakukan karena perubahan perilaku sistem akibat profiler itu sendiri. Tantangan lainnya adalah perbedaan hasil antara lingkungan pengembangan dan produksi. Hal ini dapat diatasi dengan menggunakan metode sampling untuk mengurangi overhead serta menggunakan Docker atau simulasi lingkungan produksi agar kondisi pengujian lebih realistis.


5. **Keunggulan IntelliJ Profiler**
   Manfaat utama penggunaan IntelliJ Profiler adalah kemampuan untuk memberikan gambaran yang jelas mengenai bagian kode yang paling berat dalam aplikasi. Visualisasi seperti flame graph memudahkan identifikasi hotspot secara cepat, sementara fitur thread analysis membantu mendeteksi masalah seperti deadlock. Selain itu, integrasi langsung dengan source code memungkinkan developer untuk melakukan perbaikan secara lebih efisien tanpa perlu melakukan proses debugging yang kompleks.


6. **Ketidaksesuaian Hasil JMeter dan Profiler**
   Jika hasil profiling menggunakan IntelliJ Profiler tidak sepenuhnya konsisten dengan hasil performance testing menggunakan JMeter, maka kemungkinan besar masalah tidak berasal dari kode aplikasi, melainkan dari faktor eksternal. Contohnya adalah keterbatasan database, konfigurasi connection pool yang tidak optimal, latensi jaringan, atau proses garbage collection yang intensif. Dalam situasi seperti ini, analisis perlu diperluas ke lapisan infrastruktur dan konfigurasi sistem, bukan hanya pada level kode.


7. **Strategi Optimasi dan Menjaga Fungsionalitas**
   Strategi optimasi yang dilakukan setelah analisis biasanya mencakup perbaikan pada level database dan kode program. Pada sisi database, optimasi dapat dilakukan dengan menambahkan index, memperbaiki query, atau menghindari masalah N+1 menggunakan JOIN FETCH. Pada sisi kode, optimasi dapat dilakukan dengan penggunaan struktur data yang lebih efisien serta menghindari operasi yang tidak perlu. Untuk memastikan bahwa perubahan tidak mempengaruhi fungsionalitas aplikasi, dilakukan unit testing sebelum dan sesudah optimasi. Selain itu, regression testing menggunakan JMeter juga dapat digunakan untuk memastikan bahwa peningkatan performa tidak mengubah perilaku sistem secara keseluruhan.



-----
**(all-student-name)**
   <img width="1600" height="1036" alt="image" src="https://github.com/user-attachments/assets/09f342a4-31a6-49c5-b115-55f9c0e9c985" />


   <img width="1600" height="643" alt="image" src="https://github.com/user-attachments/assets/a36c5079-ba1c-4778-9cbc-840b0e9e78ec" />



-----
**(highest-gpa)**
<img width="1600" height="1040" alt="image" src="https://github.com/user-attachments/assets/5c65d034-dbf3-4bff-ad15-9cb2e51c70ad" />


<img width="1600" height="451" alt="image" src="https://github.com/user-attachments/assets/21db8b7c-970a-491f-83f4-6642a9626f53" />



