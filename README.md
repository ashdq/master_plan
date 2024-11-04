Nama    : Fatriya Ibnu Ash shidiqqi

Kelas   : TI - 3B

NIM     : 2241720138

## 10| Dasar State Management

##  Tugas Praktikum 1: Dasar State dengan Model-View
1. Selesaikan langkah-langkah praktikum tersebut, lalu dokumentasikan berupa GIF hasil akhir praktikum beserta penjelasannya di file README.md! Jika Anda menemukan ada yang error atau tidak berjalan dengan baik, silakan diperbaiki. <br>
2. Jelaskan maksud dari langkah 4 pada praktikum tersebut! Mengapa dilakukan demikian? <br>
Untuk mengekspor model dari file plan.dart dan task.dart sehingga akan mempersingkat porses impor dari kedua file tersebut
3. Mengapa perlu variabel plan di langkah 6 pada praktikum tersebut? Mengapa dibuat konstanta ? <br>
Pentingnya Variabel plan: <br>
Variabel plan tampaknya mewakili data yang akan digunakan dalam tampilan PlanScreen ini. Kelas Plan mungkin menyimpan informasi atau tugas-tugas yang perlu ditampilkan pada layar (seperti data dalam master plan), sehingga keberadaan variabel ini penting untuk akses data di seluruh tampilan. <br>
Mengapa Dibuat Konstanta (const): <br>
Kata kunci const pada Plan digunakan untuk membuat objek ini menjadi immutable atau tidak bisa diubah setelah inisialisasi. Ini sering dilakukan jika data yang diinisialisasi bersifat statis atau tidak perlu diubah selama runtime.

4. Lakukan capture hasil dari Langkah 9 berupa GIF, kemudian jelaskan apa yang telah Anda buat!<br>
![alt text](assets/prak1.gif)
5. Apa kegunaan method pada Langkah 11 dan 13 dalam lifecyle state ?<br>
initState(): <br>
initState() adalah metode yang dipanggil sekali, saat state widget pertama kali diinisialisasi. Pada kode ini, initState() digunakan untuk membuat dan menginisialisasi objek scrollController dengan sebuah ScrollController(). scrollController memungkinkan kontrol dan pengaturan properti tampilan yang bisa di-scroll. <br>
dispose(): <br>
dispose() adalah metode yang dipanggil saat state widget dihapus secara permanen dari widget tree. Fungsi ini digunakan untuk membersihkan atau membuang sumber daya yang dipakai oleh widget agar tidak terjadi memory leak. Pada kode ini, scrollController.dispose() dipanggil untuk menghapus scrollController dan membebaskan sumber daya yang digunakannya. Ini penting karena ScrollController mengelola elemen-elemen yang bisa menghabiskan memori jika tidak di-dispose dengan benar.

6. Kumpulkan laporan praktikum Anda berupa link commit atau repository GitHub ke spreadsheet yang telah disediakan!<br>