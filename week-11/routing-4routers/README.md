    Nama		        : Rakha Putra Pratama
    NRP		        : 3122600005
    Kelas		        : 2 D4 IT A
    Mata Kuliah	        : Konsep Jaringan
    Dosen Pengampu	        : Dr. Ferry Astika Saputra S.T., M.Sc

# Physical Design

<div align="center">
<img src="./assets/topologi jaringan.JPG">
<p><strong>Gambar :</strong> Topologi Jaringan</p>
</div>

Untuk configurasinya sebagai berikut :

### **1. Router 0**

    -Static 1
    Network     : 192.168.11.0
    Mask        : 255.255.255.252
    Next Hop    : 192.168.20.9
    -Static 2
    Network     : 192.168.13.0
    Mask        : 255.255.255.252
    Next Hop    : 192.168.20.9
    -Fe 0/0
    IPv4 Address: 192.168.13.0
    Subnet Mask : 255.255.255.252
    -Fe 1/0
    IPv4 Address: 192.168.20.10
    Subnet Mask : 255.255.255.252
    -Fe 6/0
    IPv4 Address: 192.168.14.1
    Subnet Mask : 255.255.255.192

### **2. Router 1**

    -Static 1
    Network     : 192.168.14.0
    Mask        : 255.255.255.192
    Next Hop    : 192.168.20.10
    -Static 2
    Network     : 192.168.11.0
    Mask        : 255.255.255.252
    Next Hop    : 192.168.20.5
    -Fe 0/0
    IPv4 Address: 192.168.9.0
    Subnet Mask : 255.255.255.252
    -Fe 1/0
    IPv4 Address: 192.168.20.6
    Subnet Mask : 255.255.255.252
    -Fe 6/0
    IPv4 Address: 192.168.13.1
    Subnet Mask : 255.255.255.192

### **3. Router 2**

    -Static 1
    Network     : 192.168.14.0
    Mask        : 255.255.255.192
    Next Hop    : 192.168.20.13
    -Static 2
    Network     : 192.168.13.0
    Mask        : 255.255.255.192
    Next Hop    : 192.168.20.6
    -Static 3
    Network     : 192.168.12.0
    Mask        : 255.255.255.240
    Next Hop    : 192.168.20.1
    -Fe 0/0
    IPv4 Address: 192.168.20.14
    Subnet Mask : 255.255.255.252
    -Fe 1/0
    IPv4 Address: 192.168.20.5
    Subnet Mask : 255.255.255.252
    -Fe 6/0
    IPv4 Address: 192.168.20.2
    Subnet Mask : 255.255.255.252
    -Fe 7/0
    IPv4 Address: 192.168.11.1
    Subnet Mask : 255.255.255.240

### **4. Router 3**

    -Static 1
    Network     : 192.168.11.0
    Mask        : 255.255.255.252
    Next Hop    : 192.168.20.2
    -Fe 0/0
    IPv4 Address: 192.168.20.1
    Subnet Mask : 255.255.255.252
    -Fe 1/0
    IPv4 Address: 192.168.12.1
    Subnet Mask : 255.255.255.224
