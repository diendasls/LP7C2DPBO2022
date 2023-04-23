# LATIHAN 7 DPBO

*Saya Adinda Salsabilla 2005319 mengerjakan Latihan 7 dalam mata kuliah Desain dan Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin*


## Deskripsi Latihan 7
Modifikasi kode yang sudah diberikan, dengan ketentuan sebagai berikut:
1. Pemain mengendalikan bola. Setiap kali bola bergerak, skor pemain bertambah +1.
2. Skor hanya bertambah jika pemain berbelok, bukan bergerak berurutan. Detail: 
    - Saat pertama kali membuka program, pemain bergerak ke arah manapun, skor +1.
    - Setelah pemain bergerak, dia harus bergerak ke arah lain agar skornya +1. Jika menekan tombol yang sama, skor tetap (+0).
    - Contoh, pemain membuka program, lalu bergerak ke kanan dan berhenti, maka skor bertambah +1. Jika pemain bergerak ke arah atas, bawah, atau kiri, maka skor bertambah +1. Namun, jika pemain bergerak ke kanan lagi, maka skor +0.
    - Bagaimana jika urutannya, kanan - atas - kiri - kanan? Kanan yang kedua tetap +1, karena pergerakan pemain sebelumnya adalah kiri, sehingga tidak dianggap berurutan.
3. [BONUS] Buatlah sistem game yang menambahkan satu kotak atau objek apapun secara acak. Jika pemain menyentuh objek tersebut, skor bertambah +5 atau +10, lalu objek akan berpindah lagi ke posisi lain secara acak.
4. Belajar untuk meng-compile secara manual, bukan di-run via IDE. Hal ini bertujuan untuk membantu saat presentasi TMD nanti.


## Alur Program
- User menekan salah satu tombol __W, A, S, D__ atau __UP, LEFT, DOWN, RIGHT__ sehingga score akan bertambah menjadi 1 dari yang awal mula nya 0, dan akan terus bertambah 1 ketika user menekan tombol lainnya hingga user tidak menekan tombol lagi. 
- Jika **user menekan tombol yang sama** (ex: user tekan W, kemudian tekan W kembali), maka score tidak akan mengalami perubahan (akan tetap pada score terakhir yang dicapai).


## Dokumentasi Program

https://user-images.githubusercontent.com/101309423/233794044-92b58619-9fdf-4c16-ad68-e00b9b5dec6a.mp4
