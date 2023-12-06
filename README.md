# Jarkom-Modul-4-F13-2023

| **No** | **Nama**                         | **NRP**    |
| ------ | -------------------------------- | ---------- |
| 1      | Helmi Abiyu Mahendra             | 5025211061 |
| 2      | Muhammad Naufal Fawwaz Ramadhan  | 5025211223 |


--------------------------------
# Laporan Resmi

Penggunaan metode subnetting ``VLSM``  pada ``Cisco Packet Tracer`` dan ``CIDR`` pada  ``GNS3``

## VLSM

Pembagian IP dengan VLSM (Variable Length Subnet Mask) adalah teknik yang memungkinkan pembagian subnet dengan ukuran yang bervariasi, sesuai dengan kebutuhan jaringan. Dalam VLSM, subnet yang lebih besar dibagi menjadi subnet yang lebih kecil untuk memanfaatkan alamat IP secara efisien. Hal ini memungkinkan penggunaan subnet mask yang berbeda untuk setiap subnet, sehingga memaksimalkan jumlah alamat IP yang tersedia dan mengurangi pemborosan.

Untuk langkah awalnya, jumlah host yang ada pada jaringan akan dihitung, dan kemudian ditentukan ``/`` terkecil yg mampu menampung semua host tersebut. 

untuk kasus kali ini digunakan subnet /19 sebagai dasarnya.
untuk tabel kapasitas subnet adalah sebagai berikut

![subnet](Images/rentang.png)

## Topologi VLSM CPT

Berikut topologi jaringan yang kami gunakan dalam Cisco packcet tracer

![topologi](Images/CPT.png)

## Pembagian IP

Prefix IP kelompok F13 adalah ``10.58``
Untuk melakukan efisiensi pembagian IP, prosesnya dapat digambarkan dalam tree sebagai berikut

![tree](Images/CPTTree.png)

Dan hasil lebih jelasnya tersaji pada tabel

![tabel](Images/CPTTable.png)

## Konfigurasi Jaringan

### Router

#### Aura
Click node >> ```Config``` >> ``Interface``
```
FE 0/1
IP Address  : 10.58.0.25
Netmask     : 255.255.255.252
```
Masih di dalam ``Config``>>``Routing``>>``Static``
```
NetID    :
Netmask  :
Next Hop :
```
