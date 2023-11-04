    Nama		        : Rakha Putra Pratama
    NRP		        : 3122600005
    Kelas		        : 2 D4 IT A
    Mata Kuliah	        : Konsep Jaringan
    Dosen Pengampu	        : Dr. Ferry Astika Saputra S.T., M.Sc

# Routing Table

Untuk penugasan sebagai berikut :

### **1. Ping antar PC**

<div align="center">
<img src="./assets/pingPcKePc.png">
<p><strong>Gambar :</strong> Command Prompt Kelompok 4</p>
</div>
    
Untuk penugasan yang pertama yaitu menentukan IP sesuai dengan Router yang ada di Server Rack. Dapat dilakukan dengan cara yang pertama yaitu melihat apakah PC 1 terhubung dengan slot Router yang ada di Server, jika sudah mendapat informasi tentang dimana letak slot PC terhubung maka dilanjut konfigurasi IP di layer 3 yang akan mewakili letak dari PC, misal PC 1 terhubung dengan slot 7 di Router, maka di layer ke 3 slot 7, IP akan di konfigurasi menjadi 192.168.4.1 

### **2. Physical Route**

<div align="center">
<img src="./assets/physical.jpeg">
<p><strong>Gambar :</strong> Physical Route</p>
</div>
    
Gambar di atas merupakan contoh simulasi Physical dari percobaan yang telah dilakukan. Dimana PC akan pertama kali dihubungkan dengan Switch lalu berpindah ke Router yang ada di Server dan akan siap untuk dikonfigurasikan.

### **3a. Logical Route (Semua Kelompok)**
<div align="center">
<img src="./assets/logicalRouterKeRouter.jpeg">
<p><strong>Gambar :</strong> Logical Route</p>
</div>

Gambar di atas merupakan contoh simulasi Logical Route dari percobaan yang telah dilakukan. Main Router yang terdapat di Server akan menghubungkan Router 1 - 9 sehingga dapat berkomunikasi 1 dengan yang lain.

### **3b. Logical Route (Antar PC 1 Kelompok)**
<div align="center">
<img src="./assets/logicalRouterKePc.jpeg">
<p><strong>Gambar :</strong> Logical Route</p>
</div>

Gambar di atas merupakan contoh simulasi Logical Route dari percobaan yang telah dilakukan. Router akan menghubungkan Switch yang dilanjut ke PC sehingga ketika telah dilakukan konfigurasi, PC akan dapat terhubung satu sama lain dan dapat berkomunikasi.

### **4. Routing Table**
<div align="center">
<img src="./assets/ipRoutePrint.png">
<p><strong>Gambar :</strong> Routing Table</p>
</div>

Secara sederhana, Routing Table adalah panduan yang digunakan dalam jaringan untuk menentukan jalur terbaik yang harus diambil oleh data untuk mencapai tujuannya. Ini adalah komponen penting dalam manajemen dan pengiriman data dalam jaringan komputer.