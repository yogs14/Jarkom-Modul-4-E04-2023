# Jarkom-Modul-4-E04-2023

***Anggota kelompok:***
1. Yoga Firman Syahputra (5025221212)
2. Vidiawan Nabiel Arrasyid (5025221231)

## VLSM (Variable Length Subnet Masking)
### Pembagian Subnet
![topologi fix](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/2df20c47-caec-4f27-809f-df5d2eb4dff9)

Kalkulasi jumlah alamat IP yang dibutuhkan oleh tiap subnet dan tentukan netmask berdasarkan jumlah IP yang dibutuhkan.

| Subnet | Rute | Jumlah IP | Netmask |
| ------ | ---- | --------- | ------- |
|   A1   | Aura - Cloud0 | 2 | /30 |
|   A2   | Frieren - Switch5- LakeKorridor | 26 | /27 |
|   A3   | Flamme - Switch8 - RohrRoad | 1002 | /22 |
|   A4   | Fern - Switch9 - AppetitRegion - Switch9 - LaubHills | 1024 | /21 |
|   A5   | Lugner - Switch1 - TurkRegion | 1002 | /22 |
|   A6   | Lugner - Switch0 - GrobeForest | 252 | /24 |
|   A7   | Heiter - Switch6 - Sein - Switch6 - RiegelCanyon | 513 | /22 |
|   A8   | Linie - Switch11 - GranzChannel | 256 | /23 |
|   A9   | Denken - Switch2 - RoyalCapital - Switch2 - WilleRegion | 128 | /24 |
|   A10   | Lawine - Switch7 - BredtRegion | 31 | /26 |
|   A11   | Himmel - Switch10 - SchwerMountains | 7 | /28 |
|   A12   | Eisen - Switch4 - Richter - Switch4 - Revolte | 4 | /29 |
|   A13   | Eisen - Switch3 - Stark | 3 | /29 |
|   A14   | Flamme - Fern | 2 | /30 |
|   A15   | Flamme - Himmel | 2 | /30 |
|   A16   | Flamme - Frieren | 2 | /30 |
|   A17   | Aura - Frieren | 2 | /30 |
|   A18   | Aura - Denken | 2 | /30 |
|   A19   | Lawine - Linie | 2 | /30 |
|   A20   | Eisen - Linie | 2 | /30 |
|   A21   | Eisen - Lugner | 2 | /30 |
|   A22   | Aura - Eisen | 2 | /30 |
| Total |  | 4268 | /19 |


## Penurunan VLSM Tree

Subnet terbesar yang terbentuk memiliki NID 192.208.0.0 dengan netmask /19 sehingga pembagian IP berdasarkan NID dan netmask dihitung sesuai dengan pohon berikut.

![VLSM Tree Fix lo ya](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/9208d015-6240-48ea-a3b0-0f78ea1a55e2)

Pada VLSM ini diturunkan sesuai dengan length atasnya sehingga ketika /19 akan diturunkan menjadi /20, dan pembagian IP-nya mengikuti tabel di atas. Kemudian jika ada subnet yang bisa di_assign_, maka kita langsung meng_assign_. Hal ini dilakukan berulang-ulang sampai semua subnet selesai di _assign_.

## Hasil Pembagian IP per Node
![PEMETAAN FIX LO YA](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/3fa2862f-b76e-44ba-8f90-a4da2c8fb02d)

Klasifikan masing-masing host menurut tabel diatas dan bisa diketahui bahwa subnet dari tiap-tiap IP adalah IP awal dari subnet -1 (dikurangi satu):
| Subnet | Node | IP | Subnet Mask | Length |
| ------ | ---- | -- | ----------- | ------ |
|   A1   | Aura | 192.208.24.129 | 255.255.255.252 | /30 |
|   A2   | Frieren | 192.208.24.65 | 255.255.255.224 | /27 |
|   A2   | LakeKorridor | 192.208.24.66 | 255.255.255.224 | /27 |
|   A3   | Flamme | 192.208.8.1 | 255.255.252.0 | /22 |
|   A3   | RohrRoad| 192.208.8.2 | 255.255.252.0 | /22 |
|   A4   | Fern | 192.208.0.1 | 255.255.248.0 | /21 |
|   A4   | AppetitRegion | 192.208.0.2 | 255.255.248.0 | /21 |
|   A4   | LaubHills | 192.208.0.3 | 255.255.248.0 | /21 |
|   A5   | Lugner | 192.208.12.1 | 255.255.252.0 | /22 |
|   A5   | TurkRegion | 192.208.12.2 | 255.255.252.0 | /22 |
|   A6   | Lugner | 192.208.22.1 | 255.255.255.0 | /24 |
|   A6   | GrobeForest | 192.208.22.2 | 255.255.255.0 | /24 |
|   A7   | Heiter | 192.208.16.1 | 255.255.252.0 | /22 |
|   A7   | RiegelCanyon | 192.208.16.2 | 255.255.252.0 | /22 |
|   A7   | Sein | 192.208.16.3 | 255.255.252.0 | /22 |
|   A8   | Linie | 192.208.20.1 | 255.255.254.0 | /23 |
|   A8   | GranzChannel | 192.208.20.2 | 255.255.254.0 | /23 |
|   A9   | Denken | 192.208.23.1 | 255.255.255.0 | /24 |
|   A9   | RoyalCapital | 192.208.23.2 | 255.255.255.0 | /24 |
|   A9   | WilleRegion | 192.208.23.3 | 255.255.255.0 | /24 |
|   A10   | Lawine | 192.208.24.1 | 255.255.255.192 | /26 |
|   A10   | BredtRegion | 192.208.24.2 | 255.255.255.192 | /26 |
|   A10   | Heiter | 192.208.24.3 | 255.255.255.192 | /26 |
|   A11   | Himmel | 192.208.24.97 | 255.255.255.240 | /28 |
|   A11   | SchwerMountains | 192.208.24.98 | 255.255.255.240 | /28 |
|   A12   | Eisen | 192.208.24.113 | 255.255.255.248 | /29 |
|   A12   | Revolte | 192.208.24.114 | 255.255.255.248 | /29 |
|   A12   | Richter | 192.208.24.115 | 255.255.255.248 | /29 |
|   A13   | Eisen | 192.208.24.121 | 255.255.255.248 | /29 |
|   A13   | Stark | 192.208.24.122 | 255.255.255.248 | /29 |
|   A14   | Flamme | 192.208.24.133 | 255.255.255.252 | /30 |
|   A14   | Fern | 192.208.24.134 | 255.255.255.252 | /30 |
|   A15   | Flamme | 192.208.24.137 | 255.255.255.252 | /30 |
|   A15   | Himmel | 192.208.24.138 | 255.255.255.252 | /30 |
|   A16   | Flamme | 192.208.24.141 | 255.255.255.252 | /30 |
|   A16   | Frieren | 192.208.24.142 | 255.255.255.252 | /30 |
|   A17   | Aura | 192.208.24.145 | 255.255.255.252 | /30 |
|   A17   | Frieren | 192.208.24.146 | 255.255.255.252 | /30 |
|   A18   | Aura | 192.208.24.149 | 255.255.255.252 | /30 |
|   A18   | Denken | 192.208.24.150 | 255.255.255.252 | /30 |
|   A19   | Lawine | 192.208.24.153 | 255.255.255.252 | /30 |
|   A19   | Linie | 192.208.24.154 | 255.255.255.252 | /30 |
|   A20   | Eisen | 192.208.24.157 | 255.255.255.252 | /30 |
|   A20   | Linie | 192.208.24.158 | 255.255.255.252 | /30 |
|   A21   | Eisen | 192.208.24.161 | 255.255.255.252 | /30 |
|   A21   | Lugner | 192.208.24.162 | 255.255.255.252 | /30 |
|   A22   | Aura | 192.208.24.165 | 255.255.255.252 | /30 |
|   A22   | Eisen | 192.208.24.166 | 255.255.255.252 | /30 |

## Assigment pada CPT
### Setelan IP
Kita masukkan masing-masing IP pada tiap host seperti yang ada pada AppetitRegion di bawah ini:
![appetitIP](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/71a6db26-3121-44f8-bf94-94d7d92e504d)

Selanjutnya, kita lakukan _assign_ gateway yang akan menjadi jalur keluar host sesuai router yang berada tepat pada host. Misalkan pada Appetitregion maka gateway nya adalah Router Fern
![appetitgateway](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/ce650dd9-48ae-4cf0-b278-3765e74776eb)
Lakukan langkah yang sama pada tiap host atau end-system lainnya seperti, Sein, TurkRegion, dst.

### Setelan Routing
Perutean bisa dimulai dari router yang langsung mengenai host atau end-system, misal pada Router Fern:
![routingFern](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/54f21fab-5b4d-4b77-b38d-324e19711bcf)

karena Fern berada dekat host maka dia di setel untuk mengambil semua pesan dan diarahkan menuju next hop

Selanjutnya, pada Flamme:
![RoutingFlamme](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/d016c65e-e673-45cd-94b8-de093ddaddbe)

karena pada Flamme pada hierarkinya menaungi 3 subnet maka arahkan ketiga subnet tersebut menuju nexthop.

Lakukan langkah yang sama pada router selanjutnya yakni Frieren, klasifikasikan setiap subnet yang menaungi host dan arahkan ke next hop:
![RoutingFrieren](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/df5d533d-f3f2-4fd3-935e-1bf01fb4b995)

karena pada Frieren harus mengarahkan 3 subnet sebelumnya dan 1 subnet baru yang berada di dekatnya maka arahkan subnet yang lama sama seperti langkah sebelumnya dan subnet yang baru ambil semua dan arahkan ke next hop yang ada di depan Frieren sendiri.

Terakhir, pada Aura yang mana merupakan router yang langsung terhubung ke internet, maka klasifikasikan semua subnet dari semua jalur dan arahkan masing-masing sesuai arah masuk port dari Aura sendiri:
![RoutingAura](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/9c138f8e-80bd-45c6-aac3-e71ec0318ee5)

Lakukan routing pada sisa router lainnya sama seperti logika pada langkah diatas!
Karena kita sudah melakukan routing banyak di Frieren, Aura akan bertugas untuk mensortir request yang masuk dan mengarahkan antara ke Frieren atau router lainnya yang berada di dekatnya.


## VLSM Routing Check
https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/9d4b3708-390c-47aa-9a24-7ac7c5fe49af

#### Kendala:
1. Cisco Packet Tracker yang kurang stabil menyebabkan pengecekan _routing_ menjadi sedikit sulit
2. Isi dari Modul 4 yang kurang menggambarkan mekanisme _routing_ secara komprehensif sampai pada tahap akhir membuat kebingungan yang memakan waktu
3. Asisten yang kurang jelas dalam memaparkan mekanisme _routing_ saat sesi lab karena memakai topologi yang sudah jadi membuat isi dari modul tidak memiliki penjabaran yang lebih luas
