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
![flow transaction.drawio (1).png]({https://github.com/ham407/Pacman-Project-Python---Super-Cashier/blob/main/flow%20transaction.drawio%20(1).png})

## Penjelasan Codelab
* `Transaction()` : 
* `add_item()` :
* `update_item_name()` :
* `update_item_qty()` :
* `update_item_price()` :
* `delete_item()` :
* `reset_transaction()` :
* `check_order()` :
* `total_price` :
* `display_transaction()` :
* `calculate_change()` :
* `display_menu()` :
* `start()` :

## Alur Program
1. User ...
2. ..
3. ..

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
