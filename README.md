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

## Design Program
Terdiri dari file:
1. Assets : aset dari game (background picture)
2. Synchronization:
    -  **_Controller.java :_** Alur logic game. File ini dimodified di bagian *when key is released from being pressed*, yang mana untuk mengubah score player (menjadi +1) jika bergerak saat menekan salah satu tombol __W, A, S, D__ atau __UP, LEFT, DOWN, RIGHT__, dan akan terus bertambah ketika user menekan tombol yang berbeda dari sebelumnya. Sehingga ketika user telah menekan salah satu tombol, misalnya UP, maka score akan bertambah 1, kemudian check apakah tombol selanjutnya yang ditekan user tidak sama dengan tombol sebelumnya. Jika tombol yang ditekan kedua kali tidak sama dengan tombol pertama, maka score bertambah 1 lagi, dst. 
    -  **_Display.java :_** Menyediakan container untuk JFrame.
    -  **_Game.java :_** Main program (main logic dari game).
    -  **_GameInterface.java :_**  Interface untuk menyimpan function utama yang ada di dalam struktur game
    -  **_GameObject.java :_** Class abstract untuk menampung object-obcject game
    -  **_Handler.java :_** Menampung object-object yang akan dirender di layar
    -  **_Player.java :_** Object dari game, inheritance dari class abstract GameObject
    -  **_Synchronization.java :_** Menjalankan game


## Alur Program
- User menekan salah satu tombol __W, A, S, D__ atau __UP, LEFT, DOWN, RIGHT__ sehingga score akan bertambah menjadi 1 dari yang awal mula nya 0, dan akan terus bertambah 1 ketika user menekan tombol lainnya hingga user tidak menekan tombol lagi. 
- Jika **user menekan tombol yang sama** (ex: user tekan W, kemudian tekan W kembali), maka score tidak akan mengalami perubahan (akan tetap pada score terakhir yang dicapai).


## Dokumentasi Program

https://user-images.githubusercontent.com/101309423/233794044-92b58619-9fdf-4c16-ad68-e00b9b5dec6a.mp4
