# KENAPA 1 PORT FTP BISA PAKAI UDP / TCP?

Protokol FTP (File Transfer Protocol) sebagian besar menggunakan protokol TCP (Transmission Control Protocol) untuk pengiriman data. Namun, beberapa implementasi khusus FTP juga dapat menggunakan protokol UDP (User Datagram Protocol) dalam beberapa situasi tertentu.

Alasan mengapa FTP menggunakan TCP adalah karena TCP menyediakan koneksi berorientasi byte yang andal dan terjamin, yang sangat sesuai untuk transfer data seperti file. Dalam lingkungan jaringan yang dapat mengalami kehilangan paket data atau masalah lainnya, protokol TCP memastikan bahwa data yang dikirimkan akan tiba dengan benar dan dalam urutan yang tepat.

Namun, ada beberapa kasus di mana FTP dapat menggunakan UDP:

## TFTP (Trivial File Transfer Protocol):
TFTP adalah protokol transfer file yang sederhana dan biasanya menggunakan UDP. Ini sering digunakan untuk mengunduh atau mengunggah file ke atau dari perangkat jaringan seperti router atau switch selama booting atau konfigurasi.

## Mode Aktif FTP: 
Mode aktif FTP dapat menggunakan koneksi UDP untuk mengirimkan data dari server ke klien. Dalam mode ini, server FTP menginisiasi koneksi data dengan klien. Namun, karena UDP adalah protokol tanpa koneksi dan tidak menjamin pengiriman data yang handal seperti TCP, implementasi ini jarang digunakan dan seringkali disesuaikan dengan kebutuhan khusus.

Penting untuk dicatat bahwa penggunaan UDP dengan FTP tidak umum dan mungkin memerlukan konfigurasi atau pengaturan khusus. Dalam sebagian besar kasus, FTP menggunakan TCP untuk memastikan kehandalan transfer data. Jika Anda berencana menggunakan FTP atau protokol lain dalam jaringan, pastikan Anda memahami konfigurasi dan implikasi yang terkait dengan penggunaan protokol tersebut.
