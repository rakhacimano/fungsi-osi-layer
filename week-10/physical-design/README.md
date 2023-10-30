    Nama		        : Rakha Putra Pratama
    NRP		        : 3122600005
    Kelas		        : 2 D4 IT A
    Mata Kuliah	        : Konsep Jaringan
    Dosen Pengampu	        : Dr. Ferry Astika Saputra S.T., M.Sc

# Physical Design

<div align="center">
<img src="./assets/design-physical.JPG">
<p><strong>Gambar :</strong> Physical Design</p>
</div>

Untuk configurasinya sebagai berikut :

### **1. Router 0**

    -Static
    Network     : 192.168.4.0
    Mask        : 255.255.255.0
    Next Hop    : 10.252.108.14
    -Fe 0/0
    IPv4 Address: 10.252.108.4
    Subnet Mask : 255.0.0.0

### **2. Router 1**

    -Fe 0/0
    IPv4 Address: 10.252.108.14
    Subnet Mask : 255.0.0.0
    -Fe 1/0
    IPv4 Address: 192.168.4.1
    Subnet Mask : 255.255.255.0

### **3. PC 0**

    IPv4 Address    : 192.168.4.2
    Subnet Mask     : 255.255.255.0
    Default Gateway : 192.168.4.1

### **4. PC 1**

    IPv4 Address    : 192.168.4.3
    Subnet Mask     : 255.255.255.0
    Default Gateway : 192.168.4.1

### **5. PC 2**

    IPv4 Address    : 192.168.4.4
    Subnet Mask     : 255.255.255.0
    Default Gateway : 192.168.4.1
