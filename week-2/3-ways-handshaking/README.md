# 3 Ways Handshaking

<div align="center">
<img src="assets/3-ways-handshaking.jpg">
<p><strong>Gambar:</strong> 3 Ways Handshasking</p>
</div>

Konsep "3-way handshake" (tiga cara berjabat tangan) adalah metode yang digunakan dalam protokol TCP (Transmission Control Protocol) untuk memastikan pembuatan koneksi yang andal antara dua perangkat dalam jaringan. Konsep ini terlibat dalam tahap pembentukan koneksi, transfer data, dan pengakhiran koneksi. Mari kita bahas setiap tahapnya:

### 1. Connection Establishment (Pembentukan Koneksi):
Pada tahap ini, perangkat pengirim ingin memulai koneksi dengan perangkat penerima. Proses 3-way handshake melibatkan tiga langkah sebagai berikut:

-  #### 1.1 Langkah 1 (SYN): 
   Perangkat pengirim mengirimkan paket yang berisi flag SYN (synchronize) ke perangkat penerima. Flag ini menunjukkan bahwa perangkat pengirim ingin memulai koneksi.

-  #### 1.2 Langkah 2 (SYN-ACK): 
   Perangkat penerima menerima paket SYN dan merespons dengan mengirimkan balasan yang berisi flag SYN dan flag ACK (acknowledge). Flag SYN menunjukkan bahwa penerima setuju untuk memulai koneksi, dan flag ACK menunjukkan bahwa penerima menerima permintaan SYN dari perangkat pengirim.

-  #### 1.3 Langkah 3 (ACK): 
   Perangkat pengirim menerima balasan SYN-ACK, dan mengirimkan paket ACK sebagai konfirmasi bahwa penerima juga setuju untuk memulai koneksi. Setelah ini, koneksi dianggap berhasil dibentuk.

### 2. Data Transfer (Transfer Data):
Setelah koneksi berhasil dibentuk, perangkat-perangkat yang terhubung dapat mulai mentransfer data. Protokol TCP memastikan bahwa data dikirimkan dalam urutan yang benar dan tiba dengan andal. Setiap segmen data yang dikirimkan akan diberi nomor urutan, dan penerima akan mengirimkan pengakuan (ACK) kepada pengirim setelah menerima data. Jika pengirim tidak menerima ACK dalam jangka waktu tertentu, pengirim akan mengirim data lagi.

### 3. Connection Termination (Pengakhiran Koneksi):
Setelah proses pertukaran data selesai, koneksi perlu diakhiri. Pengakhiran koneksi dalam TCP melibatkan empat langkah:

-  #### 3.1 Langkah 1 (FIN): 
   Perangkat pengirim ingin mengakhiri koneksi dan mengirimkan flag FIN (finish) ke perangkat penerima.

-  #### 3.2 Langkah 2 (ACK): 
   Perangkat penerima mengirimkan balasan ACK untuk mengkonfirmasi bahwa ia menerima flag FIN.

-  #### 3.3 Langkah 3 (FIN): 
   Setelah menerima ACK, perangkat penerima ingin mengakhiri koneksi juga. Penerima mengirimkan flag FIN ke perangkat pengirim.

-  #### 3.4 Langkah 4 (ACK): 
   Perangkat pengirim mengirimkan balasan ACK untuk mengkonfirmasi bahwa ia menerima flag FIN dari perangkat penerima.





