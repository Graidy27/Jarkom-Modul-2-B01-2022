# Jarkom-Modul-2-B01-2022

Anggota :
> Ichsanul Aulia - 05111840007001\
> Alfin Indrawan - 5025201199\
> Graidy Megananda - 5025201188

---
## Tabel Konten
- [Pembagian tugas](pembagian-tugas)
- [Soal 1](#nomor-1)
- [Soal 2](#nomor-2)
- [Soal 3](#nomor-3)
- [Soal 4](#nomor-4)
- [Soal 5](#nomor-5)
- [Soal 6](#nomor-6)
- [Soal 7](#nomor-7)
- [Soal 8](#nomor-8)
- [Soal 9](#nomor-9)
- [Soal 10](#nomor-10)
- [Soal 11](#nomor-11)
- [Soal 12](#nomor-12)
- [Soal 13](#nomor-13)
- [Soal 14](#nomor-14)
- [Soal 15](#nomor-15)
- [Soal 16](#nomor-16)
- [Soal 17](#nomor-17)
- [Kesulitan](#kesulitan)

## Pembagian Tugas
- Graidy = nomor 1 hingga nomor 7

## Nomor 1
### Soal
WISE akan dijadikan sebagai DNS Master, Berlint akan dijadikan DNS Slave, dan Eden akan digunakan sebagai Web Server. Terdapat 2 Client yaitu SSS, dan Garden. Semua node terhubung pada router Ostania, sehingga dapat mengakses internet (1).

### Penyelesaian
1. Klik ```servers``` di kiri atas.
2. Klik ```local```.
3. Klik ```Add blank project```.
4. Masukkan nama ```project``` yang diinginkan.
5. Klik ```Add project```.
6. Klik tombol `Add a node` di samping kiri.
7. Lalu tarik `ubuntu-1` ke area kosong di halaman.
8. Tunggu hingga proses loading selesai.
9. Jika berhasil, maka akan menampilkan tampilan seperti berikut : <br>
![image]

10. Klik kanan dan `change hostname` menjadi `Ostania` <br>
![image]

11. Klik kanan kembali dan `change symbol` menjadi symbol `router` <br>
![image]

12. Lakukanlah langkah 6 hingga 10 untuk node `SSS`, `Garden`, `WISE`, `Berlint`, dan `Eden` sehingga didapatkan tampilan sebagai berikut : <br>
![image]

13. Klik tombol `Add a node` di samping kiri.
14. Tarik `NAT` dan dua `Switch` ke area kosong di halaman. <br>
![image]

15. Klik `Add a Link` dan tambahkan link untuk menghubungkan setiap node dan switch sehingga didapatkan tampilan sebagai berikut: <br>
![image]

16. Kita perlu melakukan setting network pada masing-masing node dengan fitur `Edit network configuration`, untuk konfigurasi network pada masing - masing node diisi dengan setting sebagai berikut :
- Ostania
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
	address 192.173.1.1
	netmask 255.255.255.0

auto eth2
iface eth2 inet static
	address 192.173.2.1
	netmask 255.255.255.0

auto eth3
iface eth2 inet static
	address 192.173.3.1
	netmask 255.255.255.0
```
- SSS
```
auto eth0
iface eth0 inet static
	address 192.173.1.2
	netmask 255.255.255.0
	gateway 192.173.1.1
```
- Garden
```
auto eth0
iface eth0 inet static
	address 192.173.1.3
	netmask 255.255.255.0
	gateway 192.173.1.1
```
- WISE
```
auto eth0
iface eth0 inet static
	address 192.173.2.2
	netmask 255.255.255.0
	gateway 192.173.2.1
```
- Berlint
```
auto eth0
iface eth0 inet static
	address 192.173.3.2
	netmask 255.255.255.0
	gateway 192.173.3.1
```
- Eden
```
auto eth0
iface eth0 inet static
	address 192.173.3.3
	netmask 255.255.255.0
	gateway 192.173.3.1
```
17. Restart semua node.
18. Topologi sudah bisa berjalan secara lokal, namun untuk mengakses jaringan keluar maka perlu dilakukan beberapa konfigurasi sebagai berikut :
- Ketikkan command berikut pada console router `Ostania`:
```
cd
bash enable-internet.sh
```
- Pada node SSS, Garden, WISE, Berlint, dan Eden ketikkan command berikut:
```
cd
bash no1.sh
```
- Restart kembali semua node.
19. Semua node sekarang sudah bisa melakukan ping ke www.google.com (sudah terhubung ke internet).

### Penjelasan File .sh
1. enable-internet.sh
2. no1.sh

### Screenshot


## Nomor 2
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 3
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 4
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 5
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 6
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 7
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 8
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 9
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 10
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 11
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 12
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 13
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 14
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 15
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 16
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot

## Nomor 17
### Soal
### Penyelesaian
### Penjelasan File .sh
### Screenshot
