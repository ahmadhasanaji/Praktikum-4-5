# Artificial Intelligence Praktikum 4 dan Praktikum 5

## Praktikum 4
**TUGAS**
1. Tentukan bagaimana algoritma BFS di atas dapat menentukan node ke 8, 6, dan 7. 2. 
2.	Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.5 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 5. 
3.	Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.6 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 9. 
4.	Ubahlah kode program di atas sehingga bentuk tree seperti Gambar 4.7 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node C.

**PENYELESAIAN**
1. Algoritma BFS dimulai dengan memasukkan node awal (node 3) ke dalam antrian. Kemudian node 3 akan memeriksa node 2 dan node 4 karena terhubung langsung atau memiliki jarak 1 dengan node 3. Node 4 akan memeriksa node 1, node 6 dan node 5. Kemudian node 5 akan memeriksa node 8 dan node 7. Proses berlanjut hingga semua node yang terhubung dengan node awal telah diperiksa. Dengan demikian, pada akhir proses BFS, node 8, 6, dan 7 akan ditemukan dan diproses sesuai dengan aturan algoritma BFS.

2. Untuk membuat tree seperti pada gambar 4.5 method static void main diubah seperti berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%202A.png?raw=true)\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%202B.png?raw=true)\
Run program dan didapatkan hasil sebagai berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%202C.png?raw=true)\
Hasil tersebut sudah menunjukkan bahwa hasil tree yg diperoleh dari program sudah sesuai dengan gambar 4.5. Untuk menemukan node 5 algoritma BFS pertama-tama dimulai dengan memasukkan node 1 ke dalam antrian. Kemudian dilanjutkan node 1 akan memeriksa node 2 dan node 3 yang terhubung langsung dengan node 1 atau node yang memiliki tingkat kedalaman 1. Dilanjutkan node 3 akan memeriksa node yang memiliki tingkat kedalaman 2 dimulai dari memeriksa node 4, node 5, node 6, dan node 7. Setelah menemukan node 5 proses akan terus berlanjut sampai semua node yang terhubung dengan node awal telah diperiksa. Dengan demikian, pada akhir proses BFS, node 5 akan ditemukan dan diproses sesuai dengan aturan algoritma BFS.

3. Untuk membuat tree seperti pada gambar 4.6 method static void main diubah seperti berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%203A.png?raw=true)\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%203B.png?raw=true)\
Run program dan didapatkan hasil sebagai berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%203C.png?raw=true)\
Hasil tersebut sudah menunjukkan bahwa hasil tree yg diperoleh dari program sudah sesuai dengan gambar 4.6. Untuk menemukan node 9 algoritma BFS pertama-tama dimulai dengan memasukkan node 1 ke dalam antrian. Kemudian dilanjutkan node 1 akan memeriksa node 2, node 3, dan node 4 yang terhubung langsung dengan node 1 atau node yang memiliki tingkat kedalaman 1. Dilanjutkan node 4 akan memeriksa node yang memiliki tingkat kedalaman 2 dimulai dari memeriksa node 5, node 6, node 7, dan node 8. Kemudian node 8 akan memeriksa node 9, setelah menemukan node 9 proses akan terus berlanjut untuk memeriksa node 10, node 11, dan node 12 sampai semua node yang terhubung dengan node awal telah diperiksa. Dengan demikian, pada akhir proses BFS, node 9 akan ditemukan dan diproses sesuai dengan aturan algoritma BFS.

4. Untuk membuat tree seperti pada gambar 4.7 perlu dilakukan beberapa perubahan pada program.\
    - Kelas Node : Ganti tipe data variabel ’data’ dari yang awalnya ’int’ menjadi ’String’ untuk dapat menerima data huruf.\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%204A.png?raw=true)\
    - Metode main: Masukkan nilai node dengan tipe data string sebagai berikut.\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%204B.png?raw=true)\
    - Metode ’addEdge’ dan ’bfs’: Masukkan logika pemrosesan data untuk tipe data String sebagai berikut.\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%204C.png?raw=true)\

    Run program dan didapatkan hasil sebagai berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20No%204D.png?raw=true)\
Hasil tersebut sudah menunjukkan bahwa hasil tree yg diperoleh dari program sudah sesuai dengan gambar 4.7. Untuk menemukan node 3 (C) algoritma BFS pertama-tama dimulai dengan memasukkan node 6 (F) ke dalam antrian. Kemudian dilanjutkan node 6 akan memeriksa node 2 (B), dan node 7 (G) yang terhubung langsung dengan node 6 atau node yang memiliki tingkat kedalaman 1. Dilanjutkan node 7 akan memeriksa node yang memiliki tingkat kedalaman 2 dimulai dari memeriksa node 1 (A), node 4 (D), dan node 9 (I). Kemudian node 9 akan memeriksa node 3, setelah menemukan node 3 (C) proses akan terus berlanjut untuk memeriksa node 5 (E), dan node 8 (H) sampai semua node yang terhubung dengan node awal telah diperiksa. Dengan demikian, pada akhir proses BFS, node 3 (C) akan ditemukan dan diproses sesuai dengan aturan algoritma BFS.

**LAMPIRAN**
1. Lampiran 1: Gambar 4.5 Tree 1\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20Lampiran%201.png?raw=true)
2. Lampiran 2: Gambar 4.6 Tree 2\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20Lampiran%202.png?raw=true)
3. Lampiran 3: Gambar 4.7 Tree 3\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%204%20Lampiran%203.png?raw=true)

## Praktikum 5
**TUGAS**
1. Pelajari class EightPuzzleSearch, EightPuzzleSpace, dan Node. 
2.	Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 8. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1. 
3.	Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.9. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1 dan 2. 
4.	Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.10. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1, 2, dan 3. 
5.	Ubahlah initial dan goal state dari program dan class-class di atas sehingga bentuk initial dan goal statenya Gambar 5.11. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state.

**PENYELESAIAN**
1. Pada program yang diberikan terdapat 3 kelas, antara lain:\
    - EightPuzzleSearch\
Kelas ini bertanggung jawab untuk melakukan pencarian solusi untuk masalah puzzle 8 angka. Kelas ini menggunakan kelas EightPuzzleSpace untuk mendapatkan informasi tentang ruang pencarian dan kelas Node untuk mewakili simpul dalam pencarian. Kelas ini juga mengelola daftar terbuka (open) dan daftar tertutup (closed) serta menyediakan metode untuk mendapatkan simpul terbaik dari daftar terbuka (getBestNode), mendapatkan biaya sebelumnya dari simpul (getPreviousCost), mencetak jalur solusi (printPath), dan menjalankan algoritma pencarian (run).
    - EightPuzzleSpace\
Kelas ini berfungsi sebagai ruang yang menangani operasi terkait ruang pencarian untuk masalah puzzle 8 angka. Ini menyediakan metode untuk mendapatkan simpul awal (getRoot), mendapatkan tujuan (getGoal), dan mendapatkan daftar suksesor dari simpul tertentu (getSuccessors). Kelas ini bertanggung jawab atas menghasilkan konfigurasi awal dan tujuan dari puzzle 8 angka, serta menghasilkan daftar kemungkinan langkah yang dapat diambil dari suatu keadaan puzzle.
    - Node\
Kelas ini merepresentasikan simpul (node) dalam struktur data graf. Setiap simpul memiliki atribut state yang merupakan array integer berukuran 9, yang merepresentasikan keadaan dari puzzle 8 angka. Atribut lainnya termasuk biaya (cost) yang terkait dengan simpul tersebut, induk (parent) yang merupakan simpul yang merupakan pendahulu dari simpul saat ini, dan daftar suksesor (successors) yang merupakan daftar simpul anak dari simpul saat ini. Kelas ini juga memiliki metode untuk mengonversi ke string, memeriksa kesetaraan, dan mendapatkan jalur dari simpul ke akar.

    Setelah program di run maka didapatkan hasil berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%201.png?raw=true)

2. Ubah initial dan goal pada program seperti dengan gambar 5.8 sebagai berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%202A.png?raw=true)\
Run program dan didapatkan hasil sebagai berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%202B.png?raw=true)\
Dari hasil yang diperoleh diatas dapat diketahui bahwa langkah-langkah untuk mencapai goal state adalah.\
    - Langkah pertama dimulai dari root state terlebih dahulu:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%202C.png?raw=true)
    - Algoritma melakukan pencarian langkah demi langkah, menggeser angka yang berdekatan dengan posisi 0 atau "tile kosong" ke arah yang tepat.
    - Setiap iterasi memperlihatkan keadaan papan setelah satu langkah dilakukan.
    - Proses berlanjut hingga algoritma mencapai goal state:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%202D.png?raw=true)

    Setiap langkah mewakili langkah perpindahan ubin yang dilakukan untuk mencapai goal state. Algoritma mencoba berbagai kombinasi perpindahan ubin untuk menemukan jalur yang paling efisien menuju goal state. Dari hasil yang didapat terlihat bahwa dari posisi root state menuju ke posisi goal state memerlukan 13 langkah.
   
   Pada percobaan kedua, diperlukan 13 langkah untuk mencapai keadaan tujuan yang diinginkan, sedangkan pada percobaan pertama hanya memerlukan 6 langkah. Perbedaan ini disebabkan oleh perbedaan jarak yang lebih jauh dari keadaan awal ke keadaan tujuan pada puzzle di percobaan kedua, dibandingkan dengan percobaan pertama, atau karena kekacauan posisi yang lebih rumit pada percobaan kedua daripada percobaan pertama. Oleh karena itu, untuk mencapai keadaan tujuan yang diinginkan pada percobaan kedua, memerlukan langkah yang lebih banyak.

3. Ubah initial dan goal pada program seperti dengan gambar 5.9 sebagai berikut:\
 ![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%203A.png?raw=true)\
Run program dan didapatkan hasil sebagai berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%203B.png?raw=true)\
Dari hasil yang diperoleh diatas dapat diketahui bahwa langkah-langkah untuk mencapai goal state adalah.
    - Langkah pertama dimulai dari root state terlebih dahulu:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%203C.png?raw=true)
    - Algoritma melakukan pencarian langkah demi langkah, menggeser angka yang berdekatan dengan posisi 0 atau "tile kosong" ke arah yang tepat.
    - Setiap iterasi memperlihatkan keadaan papan setelah satu langkah dilakukan.
    - Proses berlanjut hingga algoritma mencapai goal state:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%203D.png?raw=true)

    Setiap langkah mewakili langkah perpindahan ubin yang dilakukan untuk mencapai goal state. Algoritma mencoba berbagai kombinasi perpindahan ubin untuk menemukan jalur yang paling efisien menuju goal state. Dari hasil yang didapat terlihat bahwa dari posisi root state menuju ke posisi goal state memerlukan 20 langkah.

   Pada eksperimen poin 3, diperlukan 20 langkah untuk mencapai keadaan tujuan yang diinginkan, sementara pada eksperimen poin 1 hanya memerlukan 6 langkah, dan pada eksperimen poin 2 memerlukan 13 langkah untuk mencapai keadaan tujuan yang diinginkan. Perbedaan ini disebabkan oleh fakta bahwa teka-teki pada poin 3 memiliki jarak yang lebih jauh dari keadaan awal hingga keadaan tujuan dibandingkan dengan poin 1 dan poin 2, atau karena memiliki posisi yang lebih acak dibandingkan dengan poin 1 dan poin 2. Sehingga, pada poin 3 membutuhkan lebih banyak langkah untuk mencapai keadaan tujuan yang diinginkan.

4. Ubah initial dan goal pada program seperti dengan gambar 5.10 sebagai berikut:\
 ![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%204A.png?raw=true)\
Run program dan didapatkan hasil sebagai berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%204B.png?raw=true)\
Dari hasil yang diperoleh diatas dapat diketahui bahwa langkah-langkah untuk mencapai goal state adalah.
    - Langkah pertama dimulai dari root state terlebih dahulu:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%204C.png?raw=true)
    - Algoritma melakukan pencarian langkah demi langkah, menggeser angka yang berdekatan dengan posisi 0 atau "tile kosong" ke arah yang tepat.
    - Setiap iterasi memperlihatkan keadaan papan setelah satu langkah dilakukan.
    - Proses berlanjut hingga algoritma mencapai goal state:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%204D.png?raw=true)

    Setiap langkah mewakili langkah perpindahan ubin yang dilakukan untuk mencapai goal state. Algoritma mencoba berbagai kombinasi perpindahan ubin untuk menemukan jalur yang paling efisien menuju goal state. Dari hasil yang didapat terlihat bahwa dari posisi root state menuju ke posisi goal state memerlukan 16 langkah.

   Dalam eksperimen ini, dapat diperhatikan bahwa pada awalnya, root dari keempat percobaan menunjukkan perbedaan yang signifikan. Root di percobaan ketiga memiliki urutan angka yang lebih kompleks bila dibandingkan dengan root pada percobaan lainnya. Selain itu, solusi dari setiap percobaan juga menunjukkan perbedaan. Dalam percobaan pertama, solusinya adalah 1 6 5 8 0 4 2 7 3, sementara dalam percobaan kedua, solusinya adalah 1 2 3 4 5 6 7 8 0. Di sisi lain, dalam percobaan ketiga, solusinya adalah 7 6 5 8 0 4 1 2 3. Secara keseluruhan, walaupun keempat percobaan berhasil mencapai solusi, perbedaan pada root dan solusi menandakan bahwa program dimulai dari kondisi awal yang berbeda dan mencapai tujuan yang berbeda.

5. Untuk menyelesaikan puzzle seperti pada gambar 5.11 perlu dilakukan perubahan tipe data pada program yang awalnya ’int’ menjadi tipe data ’String’.\
Ubah initial dan goal pada program seperti dengan gambar 5.10 sebagai berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%205A.png?raw=true)\
Run program dan didapatkan hasil sebagai berikut:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%205B.png?raw=true)\
Dari hasil yang diperoleh diatas dapat diketahui bahwa langkah-langkah untuk mencapai goal state adalah.
    - Langkah pertama dimulai dari root state terlebih dahulu:\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20No%205C.png?raw=true)
    - Algoritma melakukan pencarian langkah demi langkah, menggeser angka yang berdekatan dengan posisi 0 atau "tile kosong" ke arah yang tepat.
    - Setiap iterasi memperlihatkan keadaan papan setelah satu langkah dilakukan.

    Setiap langkah mewakili langkah perpindahan ubin yang dilakukan untuk mencapai goal state. Algoritma mencoba berbagai kombinasi perpindahan ubin untuk menemukan jalur yang paling efisien menuju goal state. Pada percobaan ini untuk mencapai nilai goal state diperluhkan langkah yang sangat panjang, dikarenakan posisi pada root state dan goal state sangat jauh, hal ini juga disebabkan karena posisi node yang sangat teracak.

**LAMPIRAN**
1. Lampiran 1: Gambar 5.8\
 ![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20Lampiran%201.png?raw=true)
2.	Lampiran 2: Gambar 5.9\
 ![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20Lampiran%202.png?raw=true)
3.	Lampiran 3: Gambar 5.10\
 ![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20Lampiran%203.png?raw=true)
4.	Lampiran 4: Gambar 5.11\
![alt text](https://github.com/ahmadhasanaji/Praktikum-4-5/blob/main/Screenshot/Praktikum%205%20Lampiran%204.png?raw=true)
