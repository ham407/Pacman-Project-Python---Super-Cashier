# Pacman-Project-Python---Super-Cashier

## **Background Project**
Andi, seorang pemilik supermarket besar di salah satu kota di Indonesia, memiliki visi untuk meningkatkan efisiensi dalam proses bisnisnya. Salah satu langkah yang diambil adalah dengan merancang sistem kasir self-service di supermarket miliknya. Tujuan utamanya adalah memberikan pengalaman belanja yang lebih cepat dan nyaman bagi pelanggan, di mana pelanggan dapat secara langsung memasukkan item yang dibeli, jumlahnya, harga, dan menggunakan fitur-fitur tambahan lainnya.

Selain meningkatkan pengalaman pelanggan lokal, implementasi sistem kasir self-service juga membuka peluang bagi pelanggan di luar kota untuk berbelanja secara online dari supermarket tersebut. Namun, dalam proses perancangannya, Andi menghadapi tantangan besar. Dia menyadari bahwa untuk mewujudkan sistem kasir self-service yang efisien dan berjalan lancar, diperlukan keterlibatan seorang Programmer yang memiliki kemampuan untuk mengembangkan fitur-fitur kunci serta memastikan integrasi yang sempurna antara berbagai komponen dalam sistem tersebut.

## Objectives & Feature Requuirements
### Objectives
1. Meningkatkan efisiensi proses pembayaran di supermarket dengan memperkenalkan sistem kasir self-service.
2. Menyediakan pengalaman belanja yang lebih cepat dan nyaman bagi pelanggan.
3. Memungkinkan pelanggan untuk melakukan pembelian secara mandiri dengan memasukkan item yang dibeli, jumlahnya, dan harga secara langsung.
4. Memungkinkan pelanggan dari luar kota untuk melakukan pembelian secara online melalui sistem kasir self-service.

Jika ada yang berbelanja, seperti ini journey Customer dalam membantu orang yang berlanja tersebut.
### Feature

1. Customer membuat ID transaksi customer berikut:

  a. Dengan membuat objek dari class `trnsct_123 = Transaction()`

2. Kemudian, Cutomer memasukkan nama item, jumlah item, dan harga barang:

  a. Memasukkan item yang ingin dibeli.
  `add_item([<nama item>, <jumlah item>, <harga per item>])`

3.  Ternyata ada kesalahan dalam memasukkan nama item atau jumlah item atau harga item tetapi tidak ingin menghapus itemnya, Customer bisa melakukan:

  a. Update nama item dengan method `update_item_name(<nama_item>, <update_nama_item>)`

  b. Update jumlah item dengan method:
  `update_item_qty(<nama_item>, <update_jumlah_item>)`

  c. Update harga item menggunakan method:
  `update_item_price(<nama_item>, <update_harga_item>)`

4. Jika batal membeli item belanjaan, Customer bisa melakukan:

  a. Menghapus salah satu item dari nama item dengan method `delete_item(<nama_item>)`

  Ketika menghapus salah satu nama item, maka jumlah item dan harga per item pada baris/list tersebut akan terhapus.

  b. Langsung menghapus semua transaksi atau reset transaksi dengan method `reset_transaction()`

5.   Customer sudah selesai dengan berbelanja online nya, tetapi Customer masih ragu apakah harga barang dan nama barang yang diinput sudah benar. Bisa saja Customer melakukan kesalahan dalam melakukan input, semisal sudah melakukan input harga barang tetapi lupa untuk input nama barang. Andi bisa menggunakan method `check_order()`. Terdapat ketentuan:

  a. Akan mengeluarkan pesan "**Pemesanan sudah benar**" *(bebas bisa dengan message yang lain)* jika tidak ada kesalahan input.

  b. Akan mengeluarkan pesan "**Terdapat kesalahan input data**" jika terjadi kesalahan input.

  c. Keluarkan output transaksi atau pemesana apa saja yang sudah dibeli menggunakan fungsi `tabulate`.

6. Setelah melakukan pengecekan, Customer bisa menghitung total belanja yang sudah dibeli. Andi bisa menggunakan method `total_price()`. Pada supermarket ini ternyata terdapat ketentuan:

  a. Jika total belanja Andi diatas Rp 200.000 maka akan mendapatkan diskon 5%  

  b. Jika total belanja Andi diatas Rp 300.000 maka akan mendapatkan diskon 8%

  c. Jika total belanja Andi diatas Rp 500.000 maka akan mendapatkan diskon 10%

Andi juga memberikan pesan kepada teman-teman kalau diberi kebebasan untuk menambahkan fitur yang lain apabila masih terdapat fitur yang belum tercover dalam sistem tersebut.

### Implementasi Materi
1. Primitive Data Structure
2. Boolean
3. Nested Branching
4. Composite Data structure
5. Looping
6. Function
7. Docstring
8. modular code
9. OOP (class dan method)
10. Inheritance
11. GIT
12. Try, Except dan Raise


## Flowchart
![flow transaction.drawio (1).png](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/flow%20transaction.drawio%20(1).png)


## Penjelasan Codelab
* `Transaction()` : 
* `add_item()` : Method ini digunakan untuk menambahkan item baru ke dalam transaksi. Parameter `name` adalah nama item, `qty` adalah jumlah item, dan `price` adalah harga per item. Item baru akan disimpan ke dalam list `items`
* `update_item_name()` : Method ini digunakan untuk mengupdate nama barang
* `update_item_qty()` : Method ini digunakan untuk mengupdate jumlah item untuk item yang sudah ada di dalam transaksi. Parameter `name` adalah nama item yang akan diupdate jumlahnya, dan `new_qty` adalah jumlah item baru. Method ini akan mencari item dengan nama yang sesuai dalam list `items` dan mengupdate jumlahnya.
* `update_item_price()` : Method ini digunakan untuk mengupdate harga per item untuk item yang sudah ada dalam transaksi. Parameter `name` adalah item yang akan diupdate harganya, dan `new_price` adalah harga baru yang akan digunakan. Method ini akan mencari item dengan nama yang sesuai dala list `items` dan memperbarui harga item nya.
* `delete_item()` : Method ini digunakan untuk menghapus item dari transaksi berdasarkan nama item. Parameter `name` adalah nama item yang akan dihapus. Method ini akan mencari item dengan nama yang sesuai dalam list `items` dan menghapusnya dari transaksi.
* `reset_transaction()` : Method ini digunakan untuk menghapus semua item dalam transaksi dan mengembalikan transaksi ke keadaan awal dalam list `items` yang kosong.
* `check_order()` : Method ini digunakan untuk memeriksa apakah transaksi sudah benar atau terdapat kesalahan input data. Method ini akan menelusuri setiap item dalam transaksi dan mencetak pesan kesalahan jika terdapat item dengan data yang kurang lengkap.
* `total_price` : Method ini digunakan untuk menghitung total harga belanjaan sebelum diskon. Method ini akan mengalikan jumlah item dengan harga per item untuk setiap item dalam transaksi, kemudian menambahkan semua hasilnya. Method ini juga menampilkan diskon yang diperoleh berdasarkan total belanjaannya.
* `display_transaction()` : Method ini digunakan untuk menampilkan detail transaksi belanja dalam format tabular. Method ini akan mencetak nama item, jumlah item, harga per item, dan total harga untuk setiap item dalam transaksi.
* `calculate_change()` : Method ini digunakan untuk menghitung kembalian yang harus diberikan kepada pelanggan berdasarkan jumlah uang yang dibayarkan dan total harga belanjaan. Method ini meminta pengguna memasukkan jumlah uang yang dibayarkan dan menghitung kembalian berdasarkan total belanjaan. Jika jumlah uang yang dibayarkan tidak mencukupi, method akan mencetak pesan kesalahan.
* `display_menu()` : Method ini akan menampilkan menu program untuk setiap proses yang diinginkan.
* `start()` : Method ini berguna untuk menerima masukkan input dari pengguna ketika hendak memilih menu yang ada di `display_menu()` dan memanggil method berdasarkan operasi yang dipilih.

## Alur Program
1. User dihadapkan dengan tampilan menu dan memilih aktivitas berdasarkan menu yang tersedia
2. User menambahkan item dengan memilih menu `1. Tambah Item`.
3. User melakukan input jumlah barang yang ingin ditambahkan.
4. User melakukan input nama barang,jumlah barang,harga barang yang diinginkan sebanyak jumlah item yang ingin ditambahkan.
5. User dapat melihat daftar belanja dengan menggunakan `8. Tampilkan Total Belanjaan`
   - Menampilkan daftar belanjaan dalam bentuk tabel
   - Menampilkan total harga
   - Menampilkan diskon, jika total belanjaan memenuhi kriteria diskon.
7. Jika user berubah pikiran, user dapat melakukan `2. Udate Nama Barang`, `3. Update Jumlah Qty`, dan `4. Update Harga Barang`
8. Jika user ingin membatalkan pembelian salah satu item, user dapat melakukan `hapus item` dengan menuliskan item yang ingin dihapus dari daftar belanjaan menggunakan menu `6. Reset Transaksi` 
9. Jika ingin mengecek pesanan sudah sesuai atau belum, user dapat memilih menu `7. Cek Transaksi`
10. Untuk menampilkan total harga yang dibayarkan user dapat memilih menu `8. Tampilkan Total Belanjaan`
11. Jika user sudah selesai berbelanja, user dapat memilih menu `0. Keluar`

## Uji Coba Program
### Case 1
### Menampilkan menu dan memilih aktivitas berdasarkan menu yang tersedia

![Case1](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/Case%201.png)

Menggunakan method `start()` user diminta untuk memasukkan operasi yang diinginkan. Kemudian memberikan input dalam bentuk angka

### Case 2
### Menambah item barang ke dalam daftar belanjaan
![Case 2](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/Case%202.png)

Menggunakan method `tambah barang` user diminta untuk memasukkan jumlah item barang yang diinginkan. kemudian memberikan input nama barang, jumlah qty, dan harga per masing masing barang

![menampilkan daftar belanja](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/menampilkan%20daftar%20belanja.png)

menampilkan daftar belanja sebelum di update

### Case 3
### update nama barang
user mengupdate nama barang dengan menggunakan method `update nama barang`
![Case 3](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/Case%203.png)
user diminta memasukkan nama barang yang akan diganti menjadi nama barang baru

![menampilkan nama barang baru](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/Menampilkan%20daftar%20belanja%20setelah%20update%20nama%20barang.png)
tampilan nama barang setelah di update

### Case 4
### update jumlah barang
data sebelum update jumlah barang 
![sebelum update jumlah barang](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/sebelum%20update%20qty.png)

proses data update jumlah barang
![proses update jumlah barang](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/sebelum%20update%20qty.png)

user dapat menggunakan method `update jumlah barang` untuk mengupdate jumlah barang yang diinginkan

data setelah diupdate
![setelah diupdate](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/setelah%20update%20qty.png)

### Case 5
### update harga barang
data sebelum diupdate harga barang
![data sebelum update harga barang](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/sebelum%20update%20harga.png)

proses update harga barang
![proses update harga barang](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/Proses%20update%20harga.png)

user menggunakan method `update harga barang` untuk mengupdate harga barang yang diinginkan

setelah update harga barang
![data setelah update barang](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/setelah%20update%20harga.png)

### Case 6
### Hapus barang
data sebelum dihapus
![sebelum hapus data](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/setelah%20update%20harga.png)

proses hapus 
![proses hapus](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/proses%20hapus%20data.png)

Menggunakan method `update harga barang` untuk mengupdate jumlah harga yang diinginkan

data setelah dihapus
![setelah dihapus](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/setelah%20hapus%20barang.png)



### Case 7
### reset saat transaksi
user dapat membatalkan pembelian dengan method `reset transaksi`
![reset transaksi](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/reset%20transaction.png)

### Case 8
### mengecek transaksi
proses cek transaksi dengan menggunakan method `mengecek transaksi`
![cek transaksi](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/mengecek%20transaksi.png)

## menampilkan transaksi
![tampil transaksi](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/setelah%20mengecek%20transaksi.png)

### Case 9
### total harga
menampilkan total harga 
![total harga](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/total%20harga.png)

menggunakan method `total harga` untuk menampilkan total harga yang akan dibayarkan

### Case 10
### Menampilkan  belanjaan
![tampil belanja](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/menampilkan%20daftar%20belanja%20keseluruhan.png) 

menggunakan method `menampilkan belanjaan` untuk menampilkan daftar belanjaan


### Case 11
## keluar dari menu
![keluar](https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/images/keluar.png)

menggunakan method `keluar` untuk keluar dari display menu


## Kesimpulan
Sistem kasir ini mengusung konsep _self_service_ dalam mengelola proses transaksi. Menyediakan fungsionalitas untuk melakukan transaksi belanja, termasuk menambahkan, mengupdate, menghapus item dalam transaksi, serta menghitung total harga belanjaan, pembayaran dan kembalian. Program ini dirancang untuk berinteraksi dengan pengguna melalui _interface_ teks di terminal. Sebagaimana konsep _self_service,_ user dapat menggunakan menu yang disediakan untuk melakukan operasi yang diinginkan. Dengan ini membantu user dapat dengan mudah belanja di supermarket tanpa harus datang langsung ke supermarket.

## Pengembangan Yang Diharapkan
Ada beberapa poin yang diharapkan untuk pengembangan sistem kedepannya, yaitu:
- **Database:** Menyediakan database barang/item yang disediakan oleh supermarket
- **Manajemen Inventori**: Menambahkan fungsionalitas manajemen inventori untuk melacak stok barang, mengelola perubahan harga, dan memberikan pemberitahuan ketika stok habis.
- **Autentikasi Pengguna**: Menambah fitur autentikasi user untuk mengelola transaksi hanya oleh pengguna yang terotorisasi. Ini dapat meningkatkan keamanan dan kontrol atas transaksi yang dilakukan.
- **Pencatatan Transaksi**: Fitur yang lebih lengkap dan terstruktur. Misalnya, menyimpan riwayat transaksi yang menyertakan informasi pembeli, dan mengelompokkan transaksi berdasarkan kategori.
