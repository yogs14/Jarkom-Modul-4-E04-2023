# Jarkom-Modul-4-E04-2023

***Anggota kelompok:***
1. Yoga Firman Syahputra (5025221212)
2. Vidiawan Nabiel Arrasyid (5025221231)


## Pembagian Subnet

| Subnet | Rute | Jumlah IP | Netmask |
| ------ | ---- | --------- | ------- |
|   A1   | Aura - Cloud0 | 2 | /30 |
|   A2   | Frieren - Switch5- LakeKorridor | 26 | /27 |
|   A3   | Flamme - Switch8 - RohrRoad | 1002 | /22 |
|   A4   | Fern - Switch9 - AppetitRegion - LaubHills | 1024 | /21 |
|   A5   | Lugner - Switch1 - TurkRegion - Switch0 - GrobeForest | 1253 | /21 |
|   A6   | Heiter - Switch6 - Sein - RiegelCanyon | 513 | /22 |
|   A7   | Linie - Switch11 - GranzChannel | 256 | /23 |
|   A8   | Denken - Switch2 - RoyalCapital - WilleRegion | 128 | /24 |
|   A9   | Lawine - Switch7 - BredtRegion | 31 | /26 |
|   A10   | Himmel - Switch10 - SchwerMountains | 7 | /28 |
|   A11   | Eisen - Switch4 - Richter - Revolte | 4 | /29 |
|   A12   | Eisen - Switch3 - Stark | 3 | /29 |
|   A13   | Flamme - Fern | 2 | /30 |
|   A14   | Flamme - Himmel | 2 | /30 |
|   A15   | Flamme - Frieren | 2 | /30 |
|   A16   | Aura - Frieren | 2 | /30 |
|   A17   | Aura - Denken | 2 | /30 |
|   A18   | Lawine - Switch7 - BredtRegion | 2 | /30 |
|   A19   | Eisen - Linie | 2 | /30 |
|   A20   | Eisen - Lugner | 2 | /30 |
|   A21   | Aura - Eisenn | 2 | /30 |
| --- | --- | --- | --- |
| Total |  | #### | /19 |


## Penurunan VLSM Tree
![VLSM Tree Fix](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/1cbc2cf7-ff4f-4f77-9a7c-879080e59c9a)


## Hasil Pembagian IP per Node
![Screenshot 2023-12-04 140128](https://github.com/yogs14/Jarkom-Modul-4-E04-2023/assets/121499055/317a8ef5-74e2-4bcf-9993-5eb43e3a8925)

| Subnet | Node | IP | Subnet Mask | Length |
| ------ | ---- | -- | ----------- | ------ |
|   A1   | Aura | 192.208.27.129 | 255.255.255.252 | /30 |
|   A2   | Frieren | 192.208.27.65 | 255.255.255.224 | /27 |
|   A2   | LakeKorridor | 192.208.27.66 | 255.255.255.224 | /27 |
|   A3   | Flamme | 192.208.27.16 | 255.255.255.0 | /22 |
|   A3   | RohrRoad| 192.208.27.17 | 255.255.255.0 | /22 |
|   A4   | Fern | 192.208.8.1 | 255.255.248.0 | /21 |
|   A4   | AppetitRegion | 192.208.8.2 | 255.255.248.0 | /21 |
|   A4   | LaubHills | 192.208.8.3 | 255.255.248.0 | /21 |
|   A5   | Lugner | 192.208.0.1 | 255.255.248.0 | /21 |
|   A5   | TurkRegion | 192.208.0.2 | 255.255.248.0 | /21 |
|   A5   | GrobeForest | 192.208.0.3 | 255.255.248.0 | /21 |
|   A6   | Heiter | 192.208.20.1 | 255.255.252.0 | /22 |
|   A6   | Sein | 192.208.20.2 | 255.255.252.0 | /22 |
|   A6   | RiegelCanyon | 192.208.20.3 | 255.255.252.0 | /22 |
|   A7   | Linie | 192.208.24.1 | 255.255.254.0 | /23 |
|   A7   | GranzChannel | 192.208.24.2 | 255.255.254.0 | /23 |
|   A8   | Denken | 192.208.26.1 | 255.255.255.0 | /24 |
|   A8   | RoyalCapital | 192.208.26.2 | 255.255.255.0 | /24 |
|   A8   | WilleRegion | 192.208.26.3 | 255.255.255.0 | /24 |
|   A9   | Lawine | 192.208.27.1 | 255.255.255.192 | /26 |
|   A9   | BredtRegion | 192.208.27.2 | 255.255.255.192 | /26 |
|   A10   | Himmel | 192.208.27.97 | 255.255.255.240 | /28 |
|   A10   | SchwerMountains | 192.208.27.98 | 255.255.255.240 | /28 |
|   A11   | Eisen | 192.208.27.113 | 255.255.255.248 | /29 |
|   A11   | Richter | 192.208.27.114 | 255.255.255.248 | /29 |
|   A11   | Revolte | 192.208.27.115 | 255.255.255.248 | /29 |
|   A10   | Himmel | 192.208.27.97 | 255.255.255.240 | /28 |
