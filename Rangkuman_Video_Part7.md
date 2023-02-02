# Git : Merge Conflict

Merge conflict dapat terjadi karena dua buah branch mengerjakan baris yang sama dari suatu file dalam repository. Nantinya, hal ini dapat di-solve secara manual.

Misalnya, kita memiliki sebuah file dalam repo kita. Kemudian, kita memiliki 2 buah branch, branch master dengan branch cabang1. 

Kita memiliki sebuah file yang sama dalam masing-masing branch. Kemudian, kita ingin mengedit file pada salah satu branch, misal cabang1. Misalnya, kita menghapus beberapa baris yang tidak diperlukan dari file itu, kemudian mengubah isi dari beberapa baris dalam file tersebut.

Setelah itu, kita ingin melakukan merge dari file dari cabang1 ke branch master. Dalam hal ini, akan terjadi merge conflict karena sudah ada beberapa baris yang kita ubah pada file dari branch1. Dengan demikian, sebelum bisa melakukan merge, harus dilakukan resolve secara manual terlebih dahulu. Kita bisa memilih bagian baris mana saja yang akan diambil dari file dari kedua branch tersebut. Setelahnya, hapus bagian Git marker dan barulah proses resolve selesai. Dalam hal ini, proses merging belum selesai. Kita harus menyimpan file yang telah dimodifikasi tadi ke dalam staging area terlebih dahulu. Kemudian, kita lakukan commit dan proses merge sekarang sudah selesai.

## Checkout ke Sebuah Commit
Untuk melihat commit yang telah kita lakukan beserta hash-nya, maka ketik : git log
Jika kita ingin kembali ke suatu commit, maka ketik : git checkout [7 karakter pertama hash]

Setelah kita melakukan checkout ke sebuah commit, maka kita berada dalam keadaan 'detached HEAD' yang artinya pointer HEAD lepas dari branch (dimana seharusnya pointer HEAD ini menempel pada branch). Selain itu, kondisi repo kita akan berada di commit yang telah kita tuju barusan. Dalam hal ini, kita bisa melanjutkan pekerjaan kita pada commit yang sekarang. Misalnya, kita ingin membuat branch baru. Maka, pada commit ini akan terbentuk 2 buah branch. Kita bisa melanjutkan membuat commit-commit pada branch ini.

Jika kita ingin kembali ke branch, maka ketik : git branch [nama_branch]

## Screenshot Percobaan Menggunakan Git
https://github.com/FaaiqMastyaga/Misi1-Modul1-SEKURO_Programming-2023-16722329/blob/78104f728d67683ad6811b229d2432abda2d2e07/Screenshot/Git%20-%20merge%20conflict.pdf
