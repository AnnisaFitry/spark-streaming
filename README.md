# spark-streaming
        Nama  : Annisa Fitri Yuliandra
        Kelas : TI 3B
        NIM   : 2041720123

## Tugas Praktikum     
1. Jelaskan perbedaan spark streaming dengan metode stateless dan stateful stream processing ? Perbedaan utama antara stateless dan stateful stream processing adalah kemampuan stateful stream processing untuk mempertahankan dan menggunakan informasi dari baris data sebelumnya. Stateless stream processing lebih sederhana dan lebih cocok untuk operasi yang tidak memerlukan informasi dari waktu sebelumnya. Sementara itu, stateful stream processing lebih kompleks dan dapat digunakan untuk pemrosesan yang melibatkan analisis temporal atau pemeliharaan status yang lebih kompleks.
2. Penjelasan sintaks kode 1:
    * sys.argv: Ini adalah sebuah list yang berisi argumen baris perintah yang diberikan saat menjalankan program Python. Argumen ini dapat digunakan untuk memberikan input atau konfigurasi tambahan kepada program.
    * sys.stderr: Ini adalah objek yang mewakili aliran standar kesalahan (stderr) pada sistem. Digunakan untuk menampilkan pesan kesalahan atau debug.
StreamingContext: Ini adalah kelas inti dalam Spark Streaming. Ini digunakan untuk menginisialisasi konteks streaming, mengatur interval waktu, dan mengontrol aliran data.
    * sc: Ini adalah objek SparkContext yang digunakan untuk berinteraksi dengan Apache Spark. Ini adalah pintu gerbang utama untuk mengakses semua fungsi Spark.
    * socketTextStream: Ini adalah metode dalam StreamingContext yang digunakan untuk membuat DStream dari aliran data teks yang diterima melalui koneksi socket.
    * reduceByKey: Ini adalah operasi pada DStream yang menggabungkan nilai-nilai yang sama berdasarkan kunci dan mengurangi data menjadi satu nilai per kunci.
    * lambda line: Ini adalah ekspresi lambda dalam Python yang digunakan untuk mendefinisikan fungsi anonim. Dalam konteks ini, line adalah parameter yang mewakili setiap baris dalam DStream.
    * awaitTermination: Ini adalah metode dalam StreamingContext yang digunakan untuk menjalankan konteks streaming sampai penghentian eksternal diterima atau konteks dihentikan secara eksplisit.
3. Penjelasan sintaks kode 2:
    * nc: Singkatan dari "netcat", ini merujuk pada utilitas command-line yang disediakan oleh sistem operasi Unix untuk membaca atau menulis data melalui koneksi jaringan menggunakan protokol TCP atau UDP. Dalam konteks streaming, nc sering digunakan untuk mengirimkan data melalui koneksi socket ke aplikasi Spark Streaming.
    * lk: Tidak ada informasi yang cukup untuk menjelaskan maksud dari "lk". Jika Anda dapat memberikan konteks atau informasi tambahan tentang penggunaan "lk", saya akan mencoba memberikan penjelasan yang sesuai.
4. Penjelasan sintaks kode 3:
    * spark-submit: Ini adalah utilitas yang disediakan oleh Apache Spark untuk mengirimkan aplikasi Spark ke cluster atau menjalankannya secara lokal. Perintah spark-submit digunakan untuk mengirimkan file aplikasi Spark (biasanya berupa file JAR atau Python) ke cluster dan menjalankan aplikasi tersebut.
    * master: Ini adalah opsi dalam perintah spark-submit yang digunakan untuk menentukan URL master Spark. URL master adalah lokasi cluster di mana aplikasi Spark akan dijalankan. Misalnya, --master yarn untuk menjalankan aplikasi di cluster YARN, atau --master local[*] untuk menjalankan aplikasi secara lokal dengan menggunakan semua core yang tersedia pada mesin.
    * local[*]: Ini adalah nilai khusus untuk opsi --master dalam perintah spark-submit. Ketika --master local[*] digunakan, itu berarti aplikasi Spark akan dijalankan secara lokal menggunakan semua core yang tersedia pada mesin, memanfaatkan semua kemampuan pemrosesan yang tersedia.
5. Penjelasan sintaks kode 4:
    * ssc.checkpoint: Ini adalah metode dalam StreamingContext yang digunakan untuk mengatur titik kontrol (checkpoint) dalam proses streaming. Titik kontrol digunakan untuk menyimpan metadata dan status dari DStream untuk memulihkan keadaan aplikasi jika terjadi kegagalan.
    * parallelize: Ini adalah metode pada SparkContext (sc) yang digunakan untuk membuat RDD (Resilient Distributed Dataset) dari koleksi data yang ada di dalam program. Metode ini mengambil koleksi data dan membaginya menjadi beberapa partisi yang didistribusikan di seluruh cluster.
    * updateStateByKey: Ini adalah operasi pada DStream yang digunakan untuk mengupdate status dari setiap kunci dalam setiap waktu yang berbeda. Metode ini memungkinkan pemeliharaan status yang kompleks dengan menggabungkan nilai-nilai baru dengan status yang ada.
    * flatMap: Ini adalah operasi pada RDD atau DStream yang diterapkan pada setiap elemen dan menghasilkan nol, satu, atau lebih elemen baru. Operasi ini berguna untuk memecah elemen yang ada menjadi elemen-elemen yang lebih kecil atau memetakan elemen ke dalam bentuk yang berbeda.
6. Penjelasan sintaks kode 5:
    * rdd.take(5): Ini adalah metode pada RDD yang mengembalikan n elemen pertama dari RDD dalam bentuk array atau list. Dalam kasus ini, metode take(5) akan mengembalikan lima elemen pertama dari RDD.
    * transform: Ini adalah metode pada DStream yang digunakan untuk menerapkan transformasi pada setiap RDD dalam DStream. Metode ini memungkinkan transformasi yang kompleks dengan menggunakan operasi pada RDD di setiap waktu dalam aliran data.
    * rdd.sortByKey(False): Ini adalah metode pada RDD yang digunakan untuk mengurutkan elemen RDD berdasarkan kunci. Dalam kasus ini, metode sortByKey(False) akan mengurutkan elemen RDD secara menurun (dalam urutan menurun) berdasarkan kunci yang ada. Argumen False menunjukkan bahwa pengurutan dilakukan dalam urutan menurun.

## Praktikum 1
### Metode 1: Mode Stateless Stream Processing
#### 1 detik
![]()
#### 5 detik
![]()

### Metode 2: Mode Stateful Stream Processing
![]()

## Praktikum 2
Melakukan Transformasi di Spark Streaming
![]()






