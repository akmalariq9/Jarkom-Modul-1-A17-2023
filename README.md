# **Praktikum 1 Jaringan Komputer**
<div align=justify>

Berikut adalah Repository dari Kelompok A17 untuk pengerjaan Praktikum Modul 1 Jaringan Komputer. Dalam Repository ini terdapat Anggota Kelompok, Dokumentasi serta Penjelasan tiap soal, Screenshot Output, dan Kendala yang dialami.

# **Anggota Kelompok**

| Nama                      | NRP        | Kelas                |
| ------------------------- | ---------- | ----------------     |
| Andrian                | 5025211079 | Jaringan Komputer A  |
| Akmal Ariq Romadhon       | 5025211188 | Jaringan Komputer A  |

# **Dokumentasi dan Penjelasan Soal**
<div align=justify>

Berikut adalah dokumentasi yang berisi source code dari tiap soal dan penjelasan terkait perintah yang digunakan. 

## **Soal Nomor 1**
User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.

- **Soal Nomor 1A :** <br>
    Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? 
- **Soal Nomor 1B :** <br>
    Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut? 
- **Soal Nomor 1C :** <br>
    Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
- **Soal Nomor 1D :** <br>
    Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?

## **Penyelesaian Soal Nomor 1**
Untuk mendapatkan sequence number pada packet user mengunggah suatu file dengan protokol FTP, kita perlu memfilter  Protocol menjadi FTP terlebih dahulu.![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/5157ee23-2611-4666-8db1-2cd1ce75d265)
Lalu, kita perlu mencari paket dengan info kata kunci STOR.
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/d3e166bf-7e6e-438d-900a-059142cd4c8b)
Pada bagian Transmission Protocol Control, kita dapat melihat nilai sequence
number (raw) dan juga acknowledge number (raw).
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/39ff48ce-ed3a-4b61-8e73-fddd03d26fd0)
Lalu, untuk melihat response dari packet, kita dapat right-click pada baris packet, lalu memilih bagian follow lalu TCP Stream.
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/173bbe17-b6a1-4411-8806-b814c67dcf8e)
Pada bagian TCP Stream, kita dapat menekan command yang terdapat setelah STOR.
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/88d03061-f6ac-4075-b4bd-843b688b7f22)
Dengan menekan itu, kita akan terforward ke response dari STOR tersebut. Disini kita dapat mencari sequence number (raw) dan acknowledge number (raw)-nya.
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/e38621fe-62b4-4837-b589-43a135e6f0e7)
Hasil:
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/e50af45b-af32-4897-a656-9821ff9fc48d)



## **Soal Nomor 2**
Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!

## **Penyelesaian Soal Nomor 2**
Coming Soon.

## **Soal Nomor 3**
Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:

- **Soal Nomor 3A :** <br>
    Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702? 

- **Soal Nomor 3B :** <br>
Protokol layer transport apa yang digunakan?

## **Penyelesaian Soal Nomor 3 :**
Coming Soon

## **Soal Nomor 4**
Berapa nilai checksum yang didapat dari header pada paket nomor 130?

## **Penyelesaian Soal Nomor 4**
Pertama-tama, kita perlu mencari paket bernomor 130 terlebih dahulu
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/798dc03c-caf5-4d5e-8ec2-b66c0b1da56c)
Lalu, untuk mencari checksum-nya kita perlu right-click baris paket tersebut.
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/69d87b3e-4b78-4129-8f8d-8ed1c9290da8)
Checksum terdapat pada bagian User Datagram Protocol
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/f460b5c0-0ab0-40ce-988e-438bcf51e709)
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/7e26b9cf-f70b-4cd2-84d1-d0b90eb4c858)




## **Soal Nomor 5**
Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.

- **Soal Nomor 5A :** <br>
Berapa banyak packet yang berhasil di capture dari file pcap tersebut? 

- **Soal Nomor 5B :** <br>
Port berapakah pada server yang digunakan untuk service SMTP?

- **Soal Nomor 5C :** <br>
Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?

## **Penyelesaian Soal Nomor 5**
Coming Soon

## **Soal Nomor 6**
Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.

## **Penyelesaian Soal Nomor 6** 
Pertama-tama, kita mencari source IP address pada packet bernomor 7812.
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/f67bf789-0141-455f-b013-07f3590b44ed)
IP address = 104.18.14.101
Selanjutnya, diberitahu bahwa ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. Hal ini merupakan a1z26 cipher encryption. Dengan itu, kita perlu mendecrypt IP yang kita terima dan pada hint ketiga, tertulis bahwa rentang huruf yang digunakan hanya Huruf A-R, 1-18. Maka dari itu, untuk angka diatas 18, kita perlu memisahnya menjadi 2 angka, sehingga IP menjadi = 10 4 18 14 10 1.
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/bb522dc5-3721-467a-8b7b-52f831ee9c88)
Hasil yang didapatkan adalah jdrnja, dan dikarenakan huruf yang digunakan semua merupakan huruf besar, maka hasilnya menjadi JDRNJA.
![image](https://github.com/akmalariq9/Jarkom-Modul-1-A17-2023/assets/91018876/de90671a-b1ec-4dfe-9327-61a9da383d07)



## **Soal Nomor 7**
Berapa jumlah packet yang menuju IP 184.87.193.88?

## **Penyelesaian Soal Nomor 7** 
Coming Soon.

## **Soal Nomor 8**
Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)

## **Penyelesaian Soal Nomor 8**
Coming Soon.
    
## **Soal Nomor 9**
Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!

## **Penyelesaian Soal Nomor 9** 
Coming Soon.
    
## **Soal Nomor 10**
Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet

## **Penyelesaian Soal Nomor 10**
Coming Soon.

# **_Screenshot_ Output**
Berikut adalah output dari tiap-tiap soal yang telah dikerjakan: <br>

Coming Soon

# **End of The Line**

```c
#include <stdio.h>

int main(){
    printf("Thank you!");
}
```
