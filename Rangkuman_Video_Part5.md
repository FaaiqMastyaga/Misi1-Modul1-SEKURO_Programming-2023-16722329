# Git

## Git Command (local)
- $ git init
- $ git add [nama file]
- $ git status
- $ git commit
- $ git config
- $ git branch
- $ git help
- dll

## Area pada repo Git
- Working tree : Folder tempat kita bekerja -> folder yang diisi dengan file-file projek
- Staging area : Memberi tahu Git bahwa kita telah melakukan perubahan 
- History : Perubahan yang telah dilakukan commit akan masuk ke dalam history

Staging area dan history akan tersimpan dalam folder .git

Jadi, ketika folder kita sudah dinisialisasi sebagai repo, maka git secara otomatis akan membuat folder bernama .git

## Langkah-langkah bekerja dengan Git
1. Pindahkan directory ke folder yang ingin dijadikan sebagai repo
2. Membuat folder menjadi repo : ketik "git init"
3. Menambahkan file ke dalam staging area : ketik "git add [nama file]". Setelah file masuk ke staging area, file siap untuk di-commit
4. Mengecek apakah ada perubahan pada file dalam folder : ketik "git status"
5. Bila ingin mengeluarkan file dari staging area : ketik "git rm --cached [nama file]"
6. Sebelum melakukan commit, kita harus mendefinisikan terlebih dahulu data kita : ketik 'git config --global user.name "[nama]"' dan ketik 'git config --global user.email "[alamat email]"'
7. Untuk melakukan commit : ketik 'git commit -m "[isi pesan]"'. Jika langkah 6 tidak dilakukan, maka akan error
8. Untuk melihat history perubahan yang telah dilakukan : ketik "git log"
9. Untuk melihat history 3 perubahan terakhir yang telah dilakukan : ketik "git log -3"
10. Untuk melihat history perubahan pada suatu file secara spesifik : ketik "git log -- [nama file]"
11. Untuk mengembalikan file yang telah dihapus : ketik "git checkout [5 karakter pertama hash] -- [nama file]"
