# LAPORAN MINI PROJECT 2 PEMROGRAMAN BERORIENTASI OBJEK
## SISTEM MANAJEMEN CV MANDIRI PRIMA KREATIF

--------------


Nama : Elena Dementieva

NIM : 2509116008

Kelas : Sistem Informasi A'25

--------------

## BAB I PENDAHULUAN

### 1.1 Deksripsi Program

Sistem Manajemen CV Mandiri Prima Kreatif merupakan program berbasis Java yang dibuat untuk membantu mengelola data pada CV Mandiri Prima Kreatif yang bergerak di bidang elektronik dan pengadaan barang.

Program ini digunakan untuk mengelola tiga jenis data, yaitu data barang, data pemasok, dan data pengadaan. Pengelolaan data dilakukan dengan menerapkan konsep CRUD (Create, Read, Update, Delete), sehingga user dapat menambahkan, menampilkan, memperbarui, dan menghapus data.

Program dibuat dengan menerapkan konsep Pemrograman Berorientasi Objek (PBO), seperti class, object, constructor, access modifier, encapsulation, ArrayList, percabangan, input, perulangan, dan validasi input.

Program terdiri dari satu class entry point yaitu SistemmanajemenCVMPK serta empat class pendukung yaitu Service, Barang, Pemasok, dan Pengadaan.

--------------

## BAB II ALUR PROGRAM

Program dijalankan melalui class "SistemmanajemenCVMPK" yang berada pada package "view"

<img width="439" height="56" alt="image" src="https://github.com/user-attachments/assets/6fd94327-82b5-4ba9-9776-420a5371dbce" />


Saat program dijalankan, pengguna akan diberikan menu utama dari Sistem manajemen CV mandiri prima kreatif, yaitu;

<img width="876" height="270" alt="image" src="https://github.com/user-attachments/assets/d258d6db-eb99-47d7-90dd-323ea6bb2f16" />

Pengguna dapat memilih menu dengan memasukkan pilihan angka yang valid sesuai dengan kebutuhannya masing - masing.

### 2.1 Kelola Data Barang

Pada menu kelola data barang, terdapat beberapa pilihan yang dapat dipilih oleh user yaitu;

<img width="879" height="306" alt="image" src="https://github.com/user-attachments/assets/5c668b69-ff34-468e-8c91-8be7f50cf2d9" />

Lalu data barang terbagi ke dalam dua jenis yaitu;

- Barang Elektronik
- Barang Non - Elektronik

Barang elektronik memiliki atribut tambahan berupa garansi sesuai yang berfungsi sebagai jaminan ketahanan dari kualitas produk elektronik, sedangkan barang non-elektronik memiliki atribut tambahan berupa kategori yang berfungsi untuk mengategorikan produk tersebut sesuai fungsinya.

Saat fitur tampilkan barang dijalankan, data barang akan secara otomatis dikelompokkan oleh sistem berdasarkan jenis barang yang telah ditentukan saat pendataan barang masuk.

<img width="859" height="782" alt="image" src="https://github.com/user-attachments/assets/6fa48f46-f4e9-43b4-b833-9d554f4fbf63" />

### 2.2 Kelola Data Pemasok

Pada menu kelola data pemasok, terdapat beberapa pilihan yang dapat dipilih oleh user yaitu;

<img width="632" height="192" alt="image" src="https://github.com/user-attachments/assets/da1a9b27-7c4c-460d-8685-f2524a736ed8" />

Data pemasok terdiri dari ID pemasok, nama pemasok, alamat, dan nomor telepon.

### 2.3 Kelola Data Pengadaan

Pada menu kelola data pengadaan, terdapat beberapa pilihan yang dapat dipilih oleh user yaitu;

<img width="632" height="192" alt="image" src="https://github.com/user-attachments/assets/78d01fd9-7039-4dc2-87a0-82e1075a1dba" />

Data pengadaan terdiri dari ID pengadaan, tanggal pengadaan, dan alamat pengadaan. Lalu, program juga melakukan validasi terhadap format tanggal pengadaan agar tanggal yang dimasukkan sesuai dengan format "DD/MM/YYYY".

### 2.4 Keluar

Jika pengguna memilih menu keluar, maka program akan menghentikan proses dan menampilkan pesan bahwa program telah selesai digunakan.


<img width="503" height="217" alt="image" src="https://github.com/user-attachments/assets/055a8eb2-74b6-4d1c-81c2-603c422b4adc" />

------------------

## BAB III VALIDASI INPUT

Validasi input diterapkan pada class "Service" yang berada pada package controller, adapun terdapat beberapa validasi yang diterapkan pada sistem antara lain;

- ID wajib diisi.
- ID harus berupa angka.
- ID harus lebih dari 0.
- ID tidak boleh sama dengan ID yang sudah digunakan.
- Nama tidak boleh kosong.
- Stok harus berupa angka.
- Stok tidak boleh kurang dari 0.
- Jenis barang hanya dapat memilih pilihan yang tersedia.
- Garansi tidak boleh kosong.
- Kategori tidak boleh kosong.
- Nomor telepon tidak boleh kosong.
- Nomor telepon hanya boleh berisi angka.
- Tanggal pengadaan wajib diisi.
- Format tanggal harus "DD/MM/YYYY"
- Alamat tidak boleh kosong.
- Menu tidak tersedia.

### 3.1 Validasi Input Kelola Data Barang

#### 3.1.1 Validasi input pada tambah barang


<img width="360" height="528" alt="image" src="https://github.com/user-attachments/assets/e503a37b-3fbd-424e-bb8a-89b0def30c53" />


### 3.2 Validasi Input Kelola Data Pemasok

#### 3.2.1 Validasi input pada tambah pemasok


<img width="582" height="500" alt="image" src="https://github.com/user-attachments/assets/fd036ec8-2373-4fab-9c58-1328f7e08838" />



### 3.3 Validasi Input Kelola Data Pengadaan

#### 3.3.1 Validasi input pada tambah pengadaan


<img width="582" height="500" alt="image" src="https://github.com/user-attachments/assets/4a8ef07e-5117-4b45-b54c-71d224db671d" />


Program juga menggunakan "try catch" untuk menangani kesalahan ketika input yang seharusnya berupa angka diisi dengan data lain, lalu terdapat beberapa contoh penerapan validasi input terdapat pada method "Tambah Barang",
"Tambah Pemasok", dan "Tambah Pengadaan".

## BAB IV ACCESS MODIFIER

Program menerapkan access modifier "Private" pada atribut di dalam setiap class yang tersedia pada sistem.

Contohnya pada class "Barang" yaitu;





























