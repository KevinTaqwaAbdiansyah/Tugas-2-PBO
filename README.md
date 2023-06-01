# PENJELASAN SOURCE CODE

Source code tersebut merupakan implementasi dari tiga kelas: `Mahasiswa`, `Jurusan`, dan `Universitas`.

Kelas `Mahasiswa` memiliki atribut `nama`, `nim`, dan `jurusan`. Method `_init_` digunakan untuk menginisialisasi objek `Mahasiswa` dengan nilai-nilai atribut yang diberikan saat objek tersebut dibuat. Method `tampilkan_info` digunakan untuk mencetak informasi mahasiswa seperti nama, NIM, dan jurusan.

Kelas `Jurusan` memiliki atribut `NamaJurusan` dan `DaftarMahasiswa`. Atribut `NamaJurusan` digunakan untuk menyimpan nama jurusan, sedangkan `DaftarMahasiswa` digunakan untuk menyimpan daftar objek `Mahasiswa`. Method `_init_` digunakan untuk menginisialisasi objek `Jurusan` dengan nama jurusan yang diberikan saat objek tersebut dibuat, dan menginisialisasi `DaftarMahasiswa` sebagai list kosong. Method `tambah_mahasiswa` digunakan untuk menambahkan objek `Mahasiswa` ke dalam `DaftarMahasiswa`. Method `tampilkan_daftar_mahasiswa` digunakan untuk mencetak daftar mahasiswa dalam jurusan tersebut dengan memanggil method `tampilkan_info` dari setiap objek `Mahasiswa` dalam `DaftarMahasiswa`.

Kelas `Universitas` memiliki atribut `NamaUniversitas` dan `DaftarJurusan`. Atribut `NamaUniversitas` digunakan untuk menyimpan nama universitas, sedangkan `DaftarJurusan` digunakan untuk menyimpan daftar objek `Jurusan`. Method `_init_` digunakan untuk menginisialisasi objek `Universitas` dengan nama universitas yang diberikan saat objek tersebut dibuat, dan menginisialisasi `DaftarJurusan` sebagai list kosong. Method `tambah_jurusan` digunakan untuk menambahkan objek `Jurusan` ke dalam `DaftarJurusan`. Method `tampilkan_daftar_jurusan` digunakan untuk mencetak daftar jurusan dalam universitas tersebut dengan mencetak `NamaJurusan` dari setiap objek `Jurusan` dalam `DaftarJurusan`.

Dengan menggunakan struktur kelas di atas, kita dapat membuat objek-objek `Mahasiswa`, `Jurusan`, dan `Universitas`, dan melakukan operasi seperti menambahkan mahasiswa ke jurusan, menampilkan daftar mahasiswa dalam jurusan, dan menampilkan daftar jurusan dalam universitas.

1. Membuat objek universitas:

   universitas_xyz = Universitas("XYZ University")

   Pada baris ini, sebuah objek universitas dengan nama "XYZ University" dibuat dan disimpan dalam variabel `universitas_xyz`.

2. Membuat objek jurusan:

   jurusan_ti = Jurusan("Teknik Informatika")

   Pada baris ini, sebuah objek jurusan dengan nama "Teknik Informatika" dibuat dan disimpan dalam variabel `jurusan_ti`.

3. Menambahkan jurusan ke dalam universitas:
 universitas_xyz.tambah_jurusan(jurusan_ti)

   Pada baris ini, objek jurusan `jurusan_ti` ditambahkan ke dalam objek universitas `universitas_xyz` menggunakan metode `tambah_jurusan()`. Dengan demikian, jurusan "Teknik Informatika" menjadi salah satu jurusan yang ada di universitas "XYZ University".

4. Membuat objek mahasiswa:

   mahasiswa_andi = Mahasiswa("Kalian masing", "Kalian masing", jurusan_ti)

   Pada baris ini, sebuah objek mahasiswa dengan nama "Kalian masing" dan "Kalian masing" dibuat dan disimpan dalam variabel `mahasiswa_andi`. Objek jurusan `jurusan_ti` juga diberikan sebagai parameter saat membuat objek mahasiswa, sehingga mahasiswa tersebut terdaftar dalam jurusan "Teknik Informatika".

5. Menambahkan mahasiswa ke dalam jurusan:
 jurusan_ti.tambah_mahasiswa(mahasiswa_andi)

   Pada baris ini, objek mahasiswa `mahasiswa_andi` ditambahkan ke dalam objek jurusan `jurusan_ti` menggunakan metode `tambah_mahasiswa()`. Dengan demikian, mahasiswa "Kalian masing" menjadi salah satu mahasiswa yang terdaftar dalam jurusan "Teknik Informatika".

6. Menampilkan daftar jurusan:
 universitas_xyz.tampilkan_daftar_jurusan()
   Pada baris ini, metode `tampilkan_daftar_jurusan()` dipanggil pada objek universitas `universitas_xyz`. Metode ini akan menampilkan daftar jurusan yang ada di universitas tersebut. 

7. Menampilkan daftar mahasiswa:
   jurusan_ti.tampilkan_daftar_mahasiswa()

   Pada baris ini, metode `tampilkan_daftar_mahasiswa()` dipanggil pada objek jurusan `jurusan_ti`. Metode ini akan menampilkan daftar mahasiswa yang terdaftar dalam jurusan tersebut.

Dengan menggunakan kode di atas, kita dapat membuat tampilan objek untuk universitas, jurusan, dan mahasiswa serta menampilkan daftar jurusan dan mahasiswa yang terkait. Harap diingat bahwa kode yang diberikan adalah contoh yang tidak lengkap, sehingga perlu diimplementasikan lebih lanjut dengan menambahkan definisi kelas dan metode yang sesuai untuk setiap objek.
