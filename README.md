# bfs
Nama : Andika Anantyo

NIM : 5311421017

**TEKNIK PENCARIAN BLIND SEARCH**

1.  Tentukan bagaimana algoritma BFS di atas dapat menentukan node ke 8, 6, dan 7.
2.  Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.5 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 5.
3.  Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.6 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 9.
4.  Ubahlah kode program di atas sehingga bentuk tree seperti Gambar 4.7 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node C.

**Jawab**

1.  Node 8, 6, dan 7 ditemukan dalam urutan tertentu berdasarkan jarak (distance) dari node awal yang ditentukan, yaitu node 3. Algoritma BFS mengunjungi node-node dalam urutan lebar, yang berarti akan lebih dulu mengunjungi node yang lebih dekat dengan node awal dan kemudian bergerak ke node yang lebih jauh.
    1.  Pertama, BFS dimulai dari simpul awal n3 (dengan jarak 0) dan mengeksplorasi semua simpul yang dapat dijangkau dari n3.
    2.  Di level pertama pencarian, BFS akan mengeksplorasi simpul-simpul yang terhubung langsung ke n3, yaitu n4 dan n2.
    3.  Di level kedua, BFS akan mengeksplorasi simpul-simpul yang terhubung ke simpul level pertama, yaitu n5 dan n6 (dari n4) serta n1 (dari n2).
    4.  Di level ketiga, BFS akan mengeksplorasi simpul-simpul yang terhubung ke simpul level kedua, yaitu n7 (dari n5 dan n6) dan n8 (dari n6).
    5.  Setelah selesai menjelajahi semua simpul yang terjangkau, BFS akan mengakhiri eksekusi.

        Hasil output program:

        ![](media/b106c844ac464c3bcbd8448abd7e8612.png)

2.  Merubah method static void agar hasil tree seperti gambar 4.5. Algoritma BFS dapat menentukan node 5 dengan tahapan sebagai berikut.

    ![](media/73e547533160a40b2d044e306f159384.png)

    1.  Pertama, BFS dimulai dari simpul awal n0 (dengan jarak 0) dan mengeksplorasi semua simpul yang dapat dijangkau dari n0.
    2.  Di level pertama pencarian, BFS akan mengeksplorasi simpul-simpul yang terhubung langsung ke n0, yaitu n1 dan n2.
    3.  Di level kedua, BFS akan mengeksplorasi simpul-simpul yang terhubung ke simpul level pertama, yaitu n3 dan n4 (dari n1) serta n5 dan n6 (dari n2).
    4.  Setelah selesai menjelajahi semua simpul yang terjangkau, BFS akan mengakhiri eksekusi.

        Hasil output program:

        ![](media/2e7f13183f4137e6d4d523f04ba4eb22.png)

3.  Merubah method static void agar hasil tree seperti gambar 4.6. Algoritma BFS dapat menentukan node 9 dengan tahapan sebagai berikut.

    ![](media/5d88c5b75c4ec26e13c89c1d7e299603.png)

    1.  Pertama, BFS dimulai dari simpul awal n1 (dengan jarak 0) dan mengeksplorasi semua simpul yang dapat dijangkau dari n1.
    2.  Di level pertama pencarian, BFS akan mengeksplorasi simpul-simpul yang terhubung langsung ke n0, yaitu n2, n3,dan n4.
    3.  Di level kedua, BFS akan mengeksplorasi simpul-simpul yang terhubung ke simpul level pertama, yaitu n5 dan n6 (dari n2) serta n7 dan n8 (dari n4).
    4.  Di level ketiga, BFS akan mengeksplorasi simpul-simpul yang terhubung ke simpul level kedua, yaitu n9 dan n10 (dari n5) serta n11 dan n12 (dari n7).
    5.  Setelah selesai menjelajahi semua simpul yang terjangkau, BFS akan mengakhiri eksekusi.

        Hasil output program:

        ![](media/68818eb8dcd6abe60065620dbb73ab2c.png)

4.  Merubah method static void agar hasil tree seperti gambar 4.7. Pada program yang saya buat, saya menggunakan angka untuk mewakili abjad (A = 1, B =2, dst) karena saya belum dapat merubah kodingnya untuk menampilkan abjad. Algoritma BFS dapat menentukan node C (node 3) dengan tahapan sebagai berikut.

    ![](media/215299715042400733cf71b46da6b67c.png)

    1.  Pertama, BFS dimulai dari simpul awal n6 (nF) (dengan jarak 0) dan mengeksplorasi semua simpul yang dapat dijangkau dari n6 (nF).
    2.  Di level pertama pencarian, BFS akan mengeksplorasi simpul-simpul yang terhubung langsung ke n6 (nF), yaitu n2 (nB) dan n7 (nG).
    3.  Di level kedua, BFS akan mengeksplorasi simpul-simpul yang terhubung ke simpul level pertama, yaitu n1 (nA) dan n4 (nD) (dari nB) serta n9 (nI) (dari nG).
    4.  Di level ketiga, BFS akan mengeksplorasi simpul-simpul yang terhubung ke simpul level kedua, yaitu n3 (nC) dan n5 (nE) (dari nD) serta n8 (nH) (dari nI).
    5.  Setelah selesai menjelajahi semua simpul yang terjangkau, BFS akan mengakhiri eksekusi.

        Hasil output program

        ![](media/5d5ed5067673ef35b5835376cf705ebe.png)

**TEKNIK HEURISTIC SEARCH**

1.  Pelajari class EightPuzzleSearch, EightPuzzleSpace, dan Node.
2.  Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.8. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1.
3.  Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.9. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1 dan 2.
4.  Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.10. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1, 2, dan 3.
5.  Ubahlah initial dan goal state dari program dan class-class di atas sehingga bentuk initial dan goal statenya Gambar 5.11. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state.

**Jawab**

1.  Penjelasan class sebagai berikut:
    1.  Class EightPuzzleSearch
        -   Kelas ini merupakan inti dari algoritma pencarian untuk menyelesaikan masalah puzzle delapan ubin.
        -   Kelas ini memiliki fungsi untuk mengatur dan menjalankan pencarian serta menentukan parameter penting seperti heuristik yang digunakan.
        -   Melakukan inisialisasi node awal (root) dan node tujuan (goal), serta mengatur ruang terbuka (open) dan ruang tertutup (closed) yang digunakan selama pencarian.
        -   Menyediakan metode untuk menghitung biaya heuristik (h1 dan h2), memilih heuristik, memilih node terbaik untuk dieksplorasi, dan mengelola informasi pencarian.
    2.  Class EightPuzzleSpace
        -   Program berisi metode untuk menghitung biaya heuristik (h1 dan h2), memilih heuristik, memilih node terbaik untuk dieksplorasi, dan mengelola informasi pencarian.
        -   Program berisi metode untuk menghitung biaya heuristik (h1 dan h2), memilih heuristik, memilih node terbaik untuk dieksplorasi, dan mengelola informasi pencarian.
        -   Program juga berisi metode untuk mendapatkan daftar node suksesor yang dapat dicapai dari suatu node tertentu, sehingga memungkinkan pencarian bergerak dari satu keadaan ke keadaan lain dalam ruang pencarian.
    3.  Class Node
        -   Kelas ini merepresentasikan node dalam konteks pencarian puzzle delapan ubin.
        -   Setiap node memiliki properti berupa konfigurasi ubin dalam bentuk array 1 dimensi, biaya pencarian (cost), referensi ke node parent, dan daftar node suksesor yang dapat dicapai dari node ini.
        -   Node ini memiliki metode untuk mencetak dirinya dalam bentuk string, membandingkan dua node untuk menentukan kesamaan konfigurasi ubin, serta untuk mengembalikan jalur dari root hingga node ini.
        -   Digunakan dalam penyimpanan informasi tentang keadaan di ruang pencarian dan mengelola pergerakan antar-keadaan selama pencarian.
2.  Initial dan goal state yang diinginkan seperti gambar 5.8. Hal yang perlu dilakukan adalah merubah urutan angka pada initial dan goal state sesuai dengan urutan gambar 5.8 dari kiri atas ke kanan turun dari kiri ke kanan lagi dan seterusnya. Hasil yang didapatkan dengan menunggu waktu running 200 menit hanya menunjukkan keadaan awal saja, tidak menunjukkan goal statenya. Berbeda dengan koding awal program yang menunjukkan initial state, kemudian riwayat pencarian, dan goal state nya juga dengan waktu 0 detik. Saya menggunakan goal state yang tidak rumit dengan mayoritas angka urut dari awal ke akhir, dan hasil yang muncul sesuai yang diinginkan dengan waktu yang singkat.

    ![](media/a4d18b431d9e55dbcf200e706c01b800.png)

    Hasil program awal (defaultnya):

    ![](media/82abef6b4154c65cb9ec38344ac33092.png)

    Hasil program setelah dirubah:

    ![](media/f20aeff5e587d4f4d60d8be9bac14a7e.png)

    Hasil program dengan membuat goalnya tidak rumit:

    ![](media/f2aad360ae50129ab16b604e6f637a40.png)

3.  Initial dan goal state yang diinginkan seperti gambar 5.9. Hal yang perlu dilakukan adalah merubah urutan angka pada initial dan goal state sesuai dengan urutan gambar 5.9 dari kiri atas ke kanan turun dari kiri ke kanan lagi dan seterusnya. Hasil yang didapat dari running program selama 87 menit hanya menunjukkan initial state saja, tidak ada goal statenya. Hal ini sama seperti soal nomor 2 dengan hasil hanya initial state. Saya menggunakan goal state yang tidak rumit dengan mayoritas angka urut dari awal ke akhir, dan hasil yang muncul sesuai yang diinginkan dengan waktu yang singkat

    ![](media/fb5dcd751d5b51633e22b6d56ef381e9.png)

    Hasil program:

    ![](media/399004d6b4152943a9f18dbb9d2179dc.png)

    Hasil program dengan goal yang tidak rumit:

    ![](media/5a87a9304a302c20dde322665169fb14.png)

4.  Initial dan goal state yang diinginkan seperti gambar 5.10. Hal yang perlu dilakukan adalah merubah urutan angka pada initial dan goal state sesuai dengan urutan gambar 5.10 dari kiri atas ke kanan turun dari kiri ke kanan lagi dan seterusnya. Setelah running program dalam 0 detik, didapatkan hasil seperti yang diinginkan yaitu initial state, riwayat pencarian, dan goal state yang sesuai dengan gambar 5.10. Berbeda dengan nomor-nomor sebelumnya yang hanya menunjukkan initial state saja dan waktu yang relatif lama.

    ![](media/38b76551441b2badb047f029af230c33.png)

    Hasil program:

    ![](media/ffd4596be9d64de65b2a4fb0cb1b26b9.png)

5.  Initial dan goal state yang diinginkan seperti gambar 5.11. Hal yang perlu dilakukan adalah merubah urutan angka pada initial dan goal state sesuai dengan urutan gambar 5.11 dari kiri atas ke kanan turun dari kiri ke kanan lagi dan seterusnya. Kemudian pada koding lain dirubah karena untuk memunculkan abjad berbeda dengan memunculkan angka. Pada nomor ini saya belum paham cara untuk merubah angka menjadi abjadnya.

    ![](media/9fe74cf553df12405fb76ea4636b1c99.png)

    Hasil program: belum berhasil masih error

    **CATATAN**

    Pada percobaan **Teknik Heuristic Search** yang sudah dilakukan, terdapat beberapa hal yang saya temukan:

-   Initial state dengan urutan acak maupun tidak, tidak mempengaruhi waktu untuk mencapai goal state.
-   Goal state sangat berpengaruh terhadap waktu pencarian. Pada percobaan yang sudah saya lakukan pada nomer 2 dan 3 dengan goal state yang acak, waktu pencariannya lama hingga 200 menit dan hasilnya hanya initial state saja. Sedangkan pada nomer 4 dengan goal state yang mayoritas urut hanya angka 0 yang diubah, waktu algoritma mencapai goal state sangat cepat dan hasilnya seperti yang diinginkan.
-   Saya melakukan percobaan dengan memakai goal state dengan urutan angka yang urut, hanya dirubah letak 0 nya saja. Pada nomer 2 dan 3 dapat dilihat, algoritma membutuhkan waktu yang cepat dan hasil yang sesuai. Berbeda dengan goal state yang sesuai dengan soal yang urutannya acak.
-   Saya juga sudah mencoba dengan bahasa Python di Google Collabs, dan hasilnya juga masih sama saja dengan waktu yang lama juga.

    ![](media/a5ed4fc81a863f386f8d7a81ae66d675.png)
