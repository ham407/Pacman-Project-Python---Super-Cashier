# Pacman-Project-Python---Super-Cashier

## **Background Project**
Andi adalah seorang pemilik supermarket besar di salah satu kota di Indonesia. Andi memiliki rencana untuk melakukan prerbaikan proses bisni, yaitu Andi akan membuat sistem kasir yang *self-service* di supermarket miliknya. Sehingga customer bisa langsung memasukkan item yang dibeli, jumlah item yang dibeli, dan harga item yang dibeli dan fitur yang lain.

Sehingga customer yang tidak berada di kota tersebut bisa membeli barang dari supermarket tersebut. Setelah Andi melakukan riset, ternyata Andi memiliki masalah, yaitu Andi membutuhkan Programmer membuatkan fitur-fitur agar bisa sistem kasir *self-service* di supermarket tersebut bisa berjalan dengan lancar.

## Object & Feature Requuirements
### Object
Akhirnya Andi meminta tolong kepada teman-teman selaku programmer Python untuk membuatkan program yang menyelesaikan problem tersebut.

Jika ada yang berbelanja, begini journet Customer dalam membantu orang yang berlanja tersebut.
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

4. Jika bata membeli item belanjaan, Customer bisa melakukan:

  a. Menghapus salah satu item dari nama item dengan method `delete_item(<nama_item>)`

  Ketika menghapus salah satu nama item, maka jumlah item dan harga per item pada baris/list tersebut akan terhapus.

  b. Langsung menghapus semua transaksi atau reset transaksi dengan method `reset_transaction()`

5.   Customer sudah selesai dengan berbelanja online nya, tetapi Customer masih ragu apakah harga barang dan nama barang yang diinput sudah benar. Bisa saja Customer melakukan kesalahan dalam melakukan input, semisalh sudah melakukan input harga barang tetapi lupa untuk input nama barang. Andi bisa menggunakan method `check_order()`. Terdapat ketentuan:

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
* `add_item()` : Method ini diguakan untuk menambahkan item baru ke dalam transaksi. Parameter `name` adalah nama item, `qty` adalah jumlah item, dan `price` adalah harga per item. Item baru akan disimpan ke dalam list `items`
* `update_item_name()` : Method ini digunakan untuk mengupdate 
* `update_item_qty()` : Method ini digunakan untuk mengupdate jumlah item untuk item yang sudah ada di dalam transaksi. Parameter `name` adalah nama item yang akan diupdate jumlahnya, dan `new_qty` adalah jumlah item baru. Method ini akan mencari item dengan nama yang sesuai dalam list `items` dan mengupdate jumlahnya.
* `update_item_price()` : Method ini digunakan untuk mengupdate harga per item untuk item yang sudah ada dalam transaksi. Parameter `name` adalah item yang akan diupdate harganya, dan `new_price` adalah harga baru yang akan digunakan. Method ini akan mencari item dengan nama yang sesuai dala list `items` dan memperbarui harga item nya.
* `delete_item()` : Method ini digunakan untuk menghapus item dari transaksi berdasarkan nama item. Parameter `name` adalah nama item yang akan dihapus. Method ini akan mencari item dengan nama yang sesuai dalam list `items` dan menghapusnya dari transaksi.
* `reset_transaction()` : Method ini digunakan untuk menghapus semua item dalam transaksi dan mengembalikan transaksi ke keadaan awal dalam list `items` yang kosong.
* `check_order()` : Method ini digunakan untuk memeriksa apakah transaksi sudah benar atau terdapat kesalahan input data. Method ini akan menelusuri setiap item dalam transaksi dan mencetak pesan kesalahan jika terdapat item dengan data yang kurang lengkap.
* `total_price` : Method ini digunakan untuk menghitung total harga belanjaan sebelum diskon. Methid ini akan mengalikan jumlah item dengan harga per item untuk setiap item dalam transaksi, kemudian menambahkan semua hasilnya. Method ini juga menampilkan diskon yang diperoleh berdasarkan total belanjaannya.
* `display_transaction()` : Method ini digunakan untuk menampilkan detail transaksi belanja dalam format tabular. Method ini akan mencetak nama item, jumlah item, harga per item, dan total harga untuk setiap item dalam transaksi.
* `calculate_change()` : Method ini digunakan untuk menghitung kembalian yang harus diberikan kepada pelanggan berdasarkan jumlah uang yang dibayarkan dan total harga belanjaan. Method ini meminta pengguna memasukkan jumlah uang yang dibayarkan dan menghitung kembalian berdasarkan total belanjaan. Jika jumlah uang yang dibayarkan tidak mencukupi, method akan mencetak pesan kesalahan.
* `display_menu()` : Method ini akan menampilkan menu program untuk setiap proses yang diinginkan.
* `start()` : Method ini berguna untuk menerima masukkan input dari pengguna ketika hendak memilih menu yang ada di `display_menu()` dan memanggil method berdasarkan operasi yang dipilih.

## Alur Program
1. User dihadapkan dengan tampilan menu dan memilih aktivitas berdasarkan menu yang tersedia
2. user menambahkan item dengan memilih menu `tambah item`
3. user  melakukan input jumlah barang yang ingin ditambahkan
4. user  melakukan input nama barang,jumlah barang,harga barang yang diinginkan
6. user dapat menampilkan daftar belanja dengan menggunakan `tampilkan belanjaan`
   - menampilkan daftar belanjaan dalam bentuk tabel
   - menampilkan total harga 
7. user dapat menambahkan barang dengan menggunakan `tambah barang`
   - input "nama barang yang ingin ditambahkan"
8. jika terjadi kesalahan input, user dapat `mengupdate nama barang, jumlah qty, dan harga barang`
9. jika user ingin membatalkan membeli item, user dapat melakukan `hapus item`
 - hapus item 1
 - `reset transaction`(menghapus seluruh item)   
10. jika ingin mengecek pesanan sudah sesuai atau belum, user dapat memilih menu `mengecek transaksi`
11. untuk menampilkan total harga yang dibayarkan user dapat memilih menu `total harga`
12. jika user sudah selesai berbelanja, user dapat memilih menu `keluar`

## Uji Coba Program
### Case 1
.....
### Case 2
.....
### Case 3
.....
### Case 4
.....
### Case 5
.....
### Case 6
.....
### Case 7
.....

## Kesimpulan
...

## Perbaikan Yang Diharapkan
...
