# Menghitung manual backpropagation

1. buatlah perhitungan manual jaringan syarat tiruan algoritma backpropagation dengan jumlah data 4 2 fitur 1 output 4 itrasi

| NO   | NAMA    | IPK  | JUMLAH SKS | Lulus Tepat  Waktu |
| ---- | ------- | ---- | ---------- | ------------------ |
| 1    | Aldi    | 3.8  | 120        | Ya                 |
| 2    | Camelia | 2.9  | 90         | Tidak              |
| 3    | Rana    | 3.9  | 144        | Ya                 |
| 4    | Dinda   | 1.5  | 70         | Tidak              |

| NORMALISASI  |      |
| ------------ | ---- |
| Nilai MIN    |      |
| IPK =        | 1.5  |
| Jumlah SKS = | 70   |
| Nilai MAX    |      |
| IPK =        | 3.9  |
| Jumlah SKS = | 144  |
|              |      |
| Tidak=       | 0.0  |
| Ya=          | 1.0  |

[gambar]

| NO   | IPK     | JUMLAH SKS  | Lulus Tepat  Waktu |
| ---- | ------- | ----------- | ------------------ |
| 1    | 0.95833 | 0.675675676 | 1                  |
| 2    | 0.58333 | 0.27027027  | 0                  |
| 3    | 1       | 1           | 1                  |
| 4    | 0       | 0           | 0                  |

condition = jika error telah mencapai 0,40 atau iterasinya telah mencapai 10

**ITERASI 0**

| Menentukan  bobot secara acak |       |
| ----------------------------- | ----- |
| V11 =                         | 0.375 |
| V21 =                         | 0.951 |
| V12 =                         | 0.732 |
| V22 =                         | 0.599 |
| W11 =                         | 0.156 |
| W21 =                         | 0.156 |
| Menentukan bias secara acak   |       |
| V01 =                         | 0.058 |
| V02 =                         | 0.866 |
| W01 =                         | 0.601 |

[gambar]

**ITERASI 1**

| Menghitung semua output/keluaran di unit  tersembunyi |             |
| ---------------------------------------- | ----------- |
| Z_in11 =                                 | 1.059942568 |
| Z_in12 =                                 | 0.533777027 |
| Z_in13 =                                 | 1.384       |
| Z_in14 =                                 | 0.058       |
| Z_in21 =                                 | 1.63010473  |
| Z_in22 =                                 | 1.246641892 |
| Z_in23 =                                 | 1.84        |
| Z_in24 =                                 | 0.866       |
|                                          |             |
| Z11 =                                    | 0.74267957  |
| Z12 =                                    | 0.630363612 |
| Z13 =                                    | 0.79963265  |
| Z14 =                                    | 0.514495937 |
| Z21 =                                    | 0.836183985 |
| Z22 =                                    | 0.776718015 |
| Z23 =                                    | 0.862948707 |
| Z24 =                                    | 0.7039127   |

[gambar]

[gambar]

**ITERASI 2**

| Menghitung semua output/keluaran jaringan di unit  Y |             |
| ---------------------------------------- | ----------- |
| y_in11 =                                 | 0.847302715 |
| y_in12 =                                 | 0.820504734 |
| y_in13 =                                 | 0.860362692 |
| y_in14 =                                 | 0.791071747 |
|                                          |             |
| y11 =                                    | 0.700001019 |
| y12 =                                    | 0.694343471 |
| y13 =                                    | 0.702736425 |
| y14 =                                    | 0.688061409 |

[gambar]

[gambar]

**ITERASI 3**

| Memeriksa stopping, jika telah memenuhi maka tidak perlu  melanjutkan ke step 4 (selesai) |            |
| ---------------------------------------- | ---------- |
| MSE =                                    | 0.56695319 |

[gambar]

**ITERASI 4**

| Menghitung kesalahan/error disetiap unit keluaran  Y |             |
| ---------------------------------------- | ----------- |
| delta_1 =                                | 0.062999664 |

[gambar]

| Menghitung suku perubahan bobot Wjk |             |
| ----------------------------------- | ----------- |
| delta_W01 =                         | 0.012599933 |
| delta_W11 =                         | 0.009357713 |
| delta_W21 =                         | 0.010535862 |

alpha = 0.2

[gambar]