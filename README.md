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
			- Menghapus salah satu item dari nama item
			- Menghapus semua transaksi atau reset transaksi
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
     
     <img width="805" alt="Screenshot 2023-07-07 at 16 20 12" src="https://github.com/corneliasdrjt/cashier/assets/136590789/43b0b042-6f10-462f-a135-d46d0f4cfbf9">

      - Untuk proses input nama, jumlah, dan harga atas barang yang dibeli oleh customer
      - Menggunakan try and except untuk proses validasi user telah menginput jumlah dan harga barang dengan benar.

  3. show_order
     
     <img width="705" alt="Screenshot 2023-07-07 at 16 21 00" src="https://github.com/corneliasdrjt/cashier/assets/136590789/f1dcb50a-672a-414a-bcbf-5390c5c75c3b">

      - Untuk menampilkan detail pesanan yang sudah diinput dalam bentuk Table
      - Import table dari library tabulate sehingga detail pesanan dapat ditampilkan dalam bentuk table


  5. update_item_name, update_item_qty, update_item_price
     
     <img width="488" alt="Screenshot 2023-07-07 at 16 21 30" src="https://github.com/corneliasdrjt/cashier/assets/136590789/06c80bd9-d0a0-409b-9f5c-fe27e306f2fd">

      - Masing-masing fungsi untuk melakukan perubahan input barang yang dibeli oleh customer, dari sisi nama, jumlah / kuantitas, dan harga barang
     
  7. delete_item & reset_transaction

     <img width="768" alt="Screenshot 2023-07-07 at 16 21 45" src="https://github.com/corneliasdrjt/cashier/assets/136590789/841b8510-125d-4457-8846-fec0e599a6fc">
     <img width="657" alt="Screenshot 2023-07-07 at 16 21 59" src="https://github.com/corneliasdrjt/cashier/assets/136590789/0e42f8e4-c828-4bdf-80bf-18015bde9e1b">

      - Menghapus salah satu item dari nama item
      - Menghapus semua transaksi atau reset transaksi

  9. check_order
     
     <img width="732" alt="Screenshot 2023-07-07 at 16 22 07" src="https://github.com/corneliasdrjt/cashier/assets/136590789/e905605d-afcc-460e-a403-6d6a0b4ba94c">

      - Proses checking barang belanjaan yang telah diinput.
  
  10. total_order
      
      <img width="904" alt="Screenshot 2023-07-07 at 16 22 20" src="https://github.com/corneliasdrjt/cashier/assets/136590789/9ed095fe-86a2-4552-ad0b-040aa0221038">

     Setelah proses checking, dilanjutkan dengan proses perhitungan total belanja dengan ketentuan:
     - Jika total belanja di atas Rp 200.000 → diskon 5%
     - Jika total belanja di atas Rp 300.000 → diskon 8%
     - Jika total belanja di atas Rp 500.000 → diskon 10%

# Test Case
  Test Case 1 
  Menambahkan dua item baru dengan add_item
  <img width="553" alt="Screenshot 2023-07-07 at 16 08 41" src="https://github.com/corneliasdrjt/cashier/assets/136590789/870cbef3-d1a7-4410-801d-d0ac500fe011">

  Test Case 2 
  Menghapus salah satu item yang telah diinput menggunakan delete_item
  <img width="541" alt="Screenshot 2023-07-07 at 16 08 54" src="https://github.com/corneliasdrjt/cashier/assets/136590789/a6d57050-f345-48a3-bb62-d1c69ee40f21">
  
  Test Case 3
  Menghapus semua item yang telah diinput reset_transaction
  <img width="556" alt="Screenshot 2023-07-07 at 16 13 27" src="https://github.com/corneliasdrjt/cashier/assets/136590789/cbb68a43-f2ff-43ba-8c7e-93e0b0638f48">

  Test Case 4
  Menghitung total belanja
  <img width="796" alt="Screenshot 2023-07-07 at 16 13 37" src="https://github.com/corneliasdrjt/cashier/assets/136590789/fea1af40-5250-4dd0-91a3-2dadd7fcb70c">


# Conclusion
  Setelah dilakukan Test Case, program self service cashier dapat berjalan dengan baik, namun masih bisa dilakukan perbaikan-perbaikan atau penambahan fitur, contohnnya:
  - Ada database produk yang diinput oleh user, sehingga user misalnya hanya perlu menginput nama dan kuantitas barang, kemudian harga barang tersebut bisa langsung muncul.
  - Membuat sistem membership
  - Membuat program dengan fitur yang lebih kompleks lainnya.

