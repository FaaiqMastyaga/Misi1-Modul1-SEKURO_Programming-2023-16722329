# Version Control System (VCS)

## Definisi
“Version Control System, disebut juga Revision Control System atau Source Code Management merupakan sistem yang mengelola perubahan dari sebuah dokumen, program komputer, website, dan kumpulan informasi lain.”

## Alasan Menggunakan Version Control System
1. Mempermudah kita untuk merekam perubahan yang terjadi pada file yang kita miliki. Contoh kasus --> Kita membuat sebuah file untuk mengerjakan skripsi. Dalam pengerjaannya terjadi banyak revisi sehingga kita harus membuat file baru terus-menerus karena kita tidak ingin file lama kita hilang (merekam perubahan yang terjadi, tetapi secara manual). Nah, dengan menggunakan VCS kita bisa melakukan perekaman tersebut dengan lebih baik tanpa harus membuat banyak file dengan nama yang berbeda. Dan jika sewaktu-waktu kita ingin kembali ke file yang lama, kita hanya tinggal mengunjungi file lama itu berdasarkan rekaman yang sudah tersimpan.
2. Memungkinkan kita untuk bekerja secara tim dengan lebih efektif dan efisien. Contoh kasus --> Kita mengerjakan projek programming secara tim. Masing-masing orang dalam tim membuat source code yang berbeda-beda tergantung pada bagian yang dikerjakannya. Setelah masing-masing personal selesai dengan source code yang dikerjakannya, mereka menggabungkan semua file source code yang berbeda itu menjadi satu. Akan tetapi, hal ini cukup rumit dan tidak efisien. Dengan menggunakan VCS, pekerjaan kita bisa menjadi lebih mudah. Semua orang dalam tim dapat berkontribusi untuk mengerjakan tugasnya pada sebuah file source code yang sama. Kemudian, kita bisa melacak siapa yang telah melakukan perubahan pada file source code tersebut dan kapan terjadinya perubahan tersebut.

## Kegunaan Version Control System (VCS)
Berdasarkan dua contoh kasus sebelumnya, dapat kita simpulkan bahwa version control system berguna untuk hal-hal berikut.
1. Menyimpan rekaman / snapshot perubahan pada source code ataupun file lainnya
2. Memungkinkan kita supaya lebih efisien dalam berkolaborasi mengerjakan sebuah projek tim
3. Mengetahui siapa yang melakukan suatu perubahan terhadap file / source code dan kapan perubahan itu terjadi
4. Memungkinkan kita untuk kembali ke keadaan sebelum perubahan (checkout)

Contoh VCS : Git, subversion, mercurial, CVS

## Git
### Apa itu Git?
“Git merupakan sebuah software untuk mengelola perubahan file di dalam folder.”

### Istilah-istilah dalam Git
-	Repo : Folder project
-	Commit : Rekaman / snapshot dari repo
-	Hash : Penanda unik pada sebuah commit (berupa string)
-	Checkout : Berpindah ke sebuah commit
-	Branch : Cabang bebas dari sebuah commit
-	Merge : Menggabungkan branch
-	Remote : Sumber yang memiliki repo
-	Clone : Mengambil repo dari remote
-	Push : Mengirimkan commit ke repo
-	Pull : Mengambil commit dari repo
