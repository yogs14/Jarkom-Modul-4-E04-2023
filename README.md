# Jarkom-Modul-4-E04-2023

***Anggota kelompok:***
1. Yoga Firman Syahputra (5025221212)
2. Vidiawan Nabiel Arrasyid (5025221231)


## Pembagian Subnet
*ADA GAMBAR DISINI

| Subnet | Rute | Jumlah IP | Netmask |
| ------ | ---- | --------- | ------- |
|   A1   | Aura - Cloud0 | 2 | /30 |
|   A2   | Frieren - Switch5- LakeKorridor | 26 | /27 |
|   A3   | Flamme - Switch8 - RohrRoad | 1002 | /22 |
|   A4   | Fern - Switch9 - AppetitRegion - LaubHills | 1024 | /21 |
|   A5   | Lugner - Switch1 - TurkRegion | 1002 | /22 |
|   A6   | Lugner - Switch0 - GrobeForest | 252 | /24 |
|   A7   | Heiter - Switch6 - Sein - RiegelCanyon | 513 | /22 |
|   A8   | Linie - Switch11 - GranzChannel | 256 | /23 |
|   A9   | Denken - Switch2 - RoyalCapital - WilleRegion | 128 | /24 |
|   A10   | Lawine - Switch7 - BredtRegion | 31 | /26 |
|   A11   | Himmel - Switch10 - SchwerMountains | 7 | /28 |
|   A12   | Eisen - Switch4 - Richter - Revolte | 4 | /29 |
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
![VLSM Tree Fix lo ya](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/9208d015-6240-48ea-a3b0-0f78ea1a55e2)


## Hasil Pembagian IP per Node
![PEMETAAN FIX LO YA](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/3fa2862f-b76e-44ba-8f90-a4da2c8fb02d)


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
|   A7   | Linie | 192.208.16.3 | 255.255.252.0 | /22 |
|   A8   | Linie | 192.208.20.1 | 255.255.254.0 | /23 |
|   A8   | GranzChannel | 192.208.20.2 | 255.255.254.0 | /23 |
|   A9   | Denken | 192.208.23.1 | 255.255.255.0 | /24 |
|   A9   | RoyalCapital | 192.208.23.2 | 255.255.255.0 | /24 |
|   A9   | WilleRegion | 192.208.23.3 | 255.255.255.0 | /24 |
|   A10   | Lawine | 192.208.24.1 | 255.255.255.192 | /26 |
|   A10   | BredtRegion | 192.208.24.2 | 255.255.255.192 | /26 |
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
