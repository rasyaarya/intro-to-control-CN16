# Lab 1: PID dan anti-windup

Nama: Yudhistiro Harimurti Puspoyo
NRP: 5016261006

## Task 1: baseline (kp=5, ki=6, kd=0)

| Mode | Puncak (m/s) | Akhir (m/s) |
| --- | --- | --- |
| tanpa anti-windup | 2.39 | 1.05 |
| dengan anti-windup | 1.06 | 1.00 |

Tangkapan layar terminal:

## Task 2: suku integral dimatikan (ki=0)

Kecepatan akhir kedua baris:

| Mode | Puncak (m/s) | Akhir (m/s) |
| --- | --- | --- |
| tanpa anti-windup | 0.83 | 0.83 |
| dengan anti-windup | 0.83 | 0.83 |

Selisih dengan baris dengan anti-windup Task 1:
Selisih baris pada dengan anti-windup yang muncul adalah 0.17

Fungsi suku integral:
Fungsi suku integral adalah menyamakan puncak dan akhir dari mode tanpa anti wind-up maupun dengan anti wind-up. Selain itu,fungsi suku integral adalah mengoreksi gerak dengan mempertimbangkan akumulasi kesalaham 


## Task 3: suku integral diperbesar (ki=12)

Puncak tanpa anti-windup: 2.59
Puncak dengan anti-windup: 1.09
Selisih dengan Task 1: 1.5
Kesimpulan soal overshoot: 
Overshoot dapat mempengaruhi gerak sebuah robot, mulai dari gerak yang tidak smooth hingga terjadi error yang fatal (menabrak, tidak bisa dikendalikan, dll)


## Paragraf

Dari perolehan data di atas, suku integra berfungsi untuk mengoreksi sebuah kesalahan dari pergerakan robot dari waktu ke waktu. Jika suku integral terlalu rendah, robot akan mengalami keterlambatan dalam memproses kesalahan.
Juga, suku yang terlalu rendah ini juga dapat membuat robot tidak mencapai tujuannya (misal hanya sampai 80% pengerjaan/ proses, dan tidak mau bergerak lagi).
Apanbila suku integral terlalu besar, robot juga akan mengalami beberapa masalah seperti overshoot yang terlalu besar, sehingga robot dapat berfluktuasi atau berosilasi secara berlebihan di sekitar titik setel (setpoint) karena terlalu banyak akumulasi kesalahan.
