# Background
Sebuah supermarket besar melakukan perbaikan proses bisnis dengan cara membuat sistem kasir self-service. Program ini dibuat untuk memenuhi kebutuhan proses pembuatan fitur-fitur agar sistem kasir self-service di supermarket tersebut bisa berjalan dengan lancar.

# Requirements
	1. Proses membuat ID transaksi customer
	2. Proses input nama, jumlah, dan harga atas barang yang dibeli oleh customer
	3. Proses perubahan input barang yang dibeli oleh customer:
			- Update nama barang 
			- Update jumlah barang
			- Update harga barang
	4. Proses pembatalan barang yang dibeli:
	5. Menghapus salah satu item dari nama item
	6. Menghapus semua transaksi atau reset transaksi
	7. Proses checking barang belanjaan dengan ketentuan:
			- Jika tidak ada kesalahan input, mengeluarkan pesan “Pemesanan sudah benar”
			- Jika terjadi kesalahan input, mengeluarkan pesan “Terdapat kesalahan input data”
			- Mengeluarkan output transaksi atau pemesanan barang yang sudah dibeli
	8. Setelah proses checking, dilanjutkan dengan proses perhitungan total belanja dengan ketentuan:
			- Jika total belanja di atas Rp 200.000 → diskon 5%
			- Jika total belanja di atas Rp 300.000 → diskon 8%
			- Jika total belanja di atas Rp 500.000 → diskon 10%

# Flowchart
![Python Projects](https://github.com/corneliasdrjt/cashier/assets/136590789/021b8a63-411b-4c9e-9ef7-71563260c42a)


# Functions / Attributes
  1. add_item 
    
      - Untuk proses input nama, jumlah, dan harga atas barang yang dibeli oleh customer
      - Menggunakan try and except untuk proses validasi user telah menginput jumlah dan harga barang dengan benar.

  2. show_order

      - Untuk menampilkan detail pesanan yang sudah diinput dalam bentuk Table
      - Import table dari library tabulate sehingga detail pesanan dapat ditampilkan dalam bentuk table


  3. update_item_name, update_item_qty, update_item_price 

      - Masing-masing fungsi untuk melakukan perubahan input barang yang dibeli oleh customer, dari sisi nama, jumlah / kuantitas, dan harga barang
     
  4. delete_item & reset_transaction

      - Menghapus salah satu item dari nama item
      - Menghapus semua transaksi atau reset transaksi

  5. check_order

      - Proses checking barang belanjaan yang telah diinput.
  
  6. total_order
     Setelah proses checking, dilanjutkan dengan proses perhitungan total belanja dengan ketentuan:
     - Jika total belanja di atas Rp 200.000 → diskon 5%
     - Jika total belanja di atas Rp 300.000 → diskon 8%
     - Jika total belanja di atas Rp 500.000 → diskon 10%

# Test Case
  Test Case 1 
  Menambahkan dua item baru dengan add_item

  Test Case 2 
  Menghapus salah satu item yang telah diinput menggunakan delete_item

  Test Case 3
  Menghapus semua item yang telah diinput reset_transaction



  Test Case 4
  Menghitung total belanja



# Conclusion
  Setelah dilakukan Test Case, program self service cashier dapat berjalan dengan baik, namun masih bisa dilakukan perbaikan-perbaikan atau penambahan fitur, contohnnya:
    - Ada database produk yang diinput oleh user, sehingga user misalnya hanya perlu menginput nama dan kuantitas barang, kemudian harga barang tersebut bisa langsung muncul.
    - Membuat sistem membership
    - Membuat program dengan fitur yang lebih kompleks lainnya.

