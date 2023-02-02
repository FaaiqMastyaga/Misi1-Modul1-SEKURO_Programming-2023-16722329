# Git : Branch & Merge

## Branch
Branch adalah membuat cabang bebas dari commit. Pemanfaatannya untuk membuat / menambahkan suatu fitur baru pada projek tetapi kita masih belum yakin dengan fitur yang akan ditambahkan tersebut.

# Merge
Penggabungan cabang / branch

## Implementasi Branch di dalam Git
Misal, kita memiliki sebuah repo. Di dalam repo tersebut, kita membuat commit. Ingat bahwa commit memiliki hash, username, email, dan timestamp. Commit ini terhubung dengan sebuah branch. Secara default, branch-nya berupa branch master. Untuk mengetahui branch mana yang aktif pada sebuah commit, ada sesuatu yang disebut dengan head. Head ini berfungsi sebagai pointer yang mengarah pada branch yang aktif.

Saat kita melakukan perubahan pada repo kita, maka ada commit selanjutnya. Commit ini memiliki hash yang baru. Pointer head masih menunjuk ke arah branch master, sedangkan branch master menunjukkan commit yang paling baru ini. Dengan demikian, commit yang sedang aktif saat ini adalah commit yang paling baru. 

## Branch
### Membuat branch
Ketik : git branch [nama_branch]
Untuk membuat lebih dari satu branch, pembuatannya harus dilakukan satu per satu.

### Menampilkan branch
Untuk menampilkan nama-nama branch yang ada pada commit saat ini, maka ketik: git branch

### Mengubah tampilan commit
Untuk membuat tampilan commit yang lebih baik, ketik : git log --all --decorate --oneline --graph
Hal ini sering digunakan karena sangat berguna. Supaya tidak perlu repot mengulang perintah yang panjang, maka dibutuhkan alias / nama lain, misalnya graph.
Ketik : alias graph="git log --all --decorate --oneline --graph"
Selanjutnya, kita hanya perlu menuliskan graph untuk melihat tampilan commit berupa timeline.

### Berpindah branch
Untuk memindahkan branch yang sedang aktif, ketik : git checkout [nama_branch].
Pada commit yang sama, pointer head sebagai penunjuk branch aktif sebelumnya akan berpindah ke nama branch yang baru saja dimasukkan dalam perintah. Dengan demikian, nama branch yang baru saja dimasukkan menjadi branch yang aktif sekarang. Misal, dari branch yang baru ini kita menambahkan sebuah commit. Artinya, nama branch beserta pointer yang menunjuknya akan berpindah ke commit saat ini. Commit yang ada di branch ini tidak akan mengganggu branch master ataupun branch lainnya.

### Menghapus branch
Biasanya, setelah kita melakukan branching dan menggabungkannya (merging) ke branch utama / master, branch yang sebelumnya dipakai untuk di merge sudah tidak terpakai lagi. Jadi, kita ingin menghapus branch tersebut. Untuk menghapus branch tersebut, caranya ketik : git branch -d [nama_branch]. Akan tetapi, perintah ini hanya bisa dilakukan untuk branch yang sudah di-merge. Ada perintah lain untuk menghapus branch (tidak peduli apakah branch yang ingin dihapus sudah di-merge atau belum), yaitu ketik : git branch -D [nama_branch]

## Merge
### Jenis merge di dalam  Git
1. Fast Forward
2. Three-way Merge

Perintah untuk melakukan kedua jenis merge tersebut sama, akan tetapi cara kerja di belakang layarnya yang berbeda.
Untuk melakukan merge, ketik : merge [nama_branch]
Pastikan kita sudah berada di berada di branch yang benar saat kita melakukan merge. Misalnya, jika kita ingin memasukkan branch1 ke branch master, maka pindahkan pointer terlebih dahulu agar branch yang aktif sekarang adalah branch master. Kemudian, barulah kita mengetikkan 'merge branch1'.

### Penjelasan Mengenai Merge
1. Fast Forward Merge
Terjadi ketika branch yang ingin digabungkan berada pada jalur langsung (direct path)
2. Three-way (Merge Commit)
Terjadi ketika branch yang ingin digabungkan tidak terhubung secara langsung. Misalnya, kita punya 2 branch lain yang merupakan cabang dari branch master. Kemudian, kita ingin menggabungkan kedua branch tersebut. Maka, dilakukannya merge commit (three-way merge)

### Memastikan branch yang sudah di-merge
Untuk mengetahui branch mana yang sudah di-merge, maka ketik : git branch --merged
