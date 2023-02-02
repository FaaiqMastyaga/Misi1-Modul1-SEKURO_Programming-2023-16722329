# GitHub : Branch & Merge

## Branching
- Membuat snapshot tanpa mengganggu jalur utama (Master branch)
- Membuat fitur eksperimental (mau menambahkan fitur, tapi belum yakin)
- Dua orang mengerjakan repo yang sama, kemudian nantinya digabungkan menggunakan merge

## Cara Melakukan Branching
Untuk melakukan branching, ada dua cara:
1. Pada repository, klik main --> di sini kita bisa mencari branch yang sudah ada sebelumnya atau bahkan membuat branch baru
2. Pada repository, klik salah satu file, pada bagian commit changes, centang pilihan create a new branch.

## Merging
- Menggabungkan dua buah branch

## Cara Melakukan Merging
Klik Compare & pull request pada repo. Halaman akan berpindah ke halaman baru dengan judul "Open a pull request". Klik "Create pull request". Setelah itu, masuk ke tab pull request (di jajaran tab repo). Kita bisa melihat hasil modifikasi dari pull request yang telah kita lakukan. Kemudian, klik "merge pull request" dan "confirm merge".
Untuk menggabungkan beberapa branch, maka merging harus dilakukan satu per satu.
Jika saat ingin melakukan merging terjadi conflict, maka kita harus resolve conflict secara manual terlebih dahulu pada bagian pull request yang terjadi conflict. Jika ada bagian/baris yang berubah, maka kita bisa memilih apakah ingin menggunakan yang sebelumnya atau menggunakan hasil modifikasi di pull request tersebut. Setelahnya, barulah kita bisa melakukan merge.
Pull request juga dapat dilakukan pada repo milik orang lain. Misal, kita memodifikasi source code dari repo milik orang lain dan kita ingin hasil modifikasinya tersebut dimasukkan ke dalam repo orang tadi. Nah, kita tinggal melakukan pull request dan menunggu konfirmasi dari pemilik repo apakah ia mau menerima hasil modifikasi yang telah kita lakukan atau tidak.

## Recap
- Branch : jalur bebas dari sebuah commit
- Checkout : berpindah ke branch / commit yang lain
- Pull Request : meminta pemilik repo untuk mengambil perubahan yang telah dilakukan
- Merge : menggabungkan 2 buah branch
- Merge Conflict : baris yang sama diubah oleh 2 branch yang berbeda
