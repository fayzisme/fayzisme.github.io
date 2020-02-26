# Bootcamp Refactory

##### Materi - materi yang dipelajari.
  - Git flow
 
### 1. Git Flow
> Git adalah version control system yang digunakan para developer untuk mengembangkan software secara bersama-bersama. Fungsi utama git yaitu mengatur versi dari source code program anda dengan mengasih tanda baris dan code mana yang ditambah atau diganti.[ sumber](https://idcloudhost.com/pengertian-dan-manfaat-git-bagi-developer/)


### Installation

Install Git pada OS Linux
```sh
$ sudo apt install git-all
```
Untuk cek apakah sudah terinstall 
```sh
$ git --version
```

### Contoh Penerapan Git

Membuat repository baru pada akun Github,
Nama repository misal : [fayzisme.github.io](https://github.com/fayzisme/fayzisme.github.io)

Initialize Git pada folder project kita.
```sh
$ git init
```
Add project kita.
```sh
$ git add .
```
Dalam hal ini dalam project saya terdapat file berisi.
[index.html]() dan [README.md]() 

Kemudian lakukan commit.
```sh
$ git commit -m "pesan commit"
```
Masukkan link atau alamat remote yang akan kita gunakan.
Misal dalam hal ini:
```sh
$ git remote add origin https://github.com/fayzisme/fayzisme.github.io.git
```
Kemudian lakukan push dengan cara.
```sh
$ git push -u origin master
```
Maka repository saya hasilnya seperti ini :
![Image]()

### Mencoba mengerjakan project orang lain.

Clone project orang lain.
Misal dalam hal ini dengan project [Mas Fadhel](https://github.com/fdhlmhd)
```sh
$ git clone https://github.com/fdhlmhd/fdhlmhd.github.io.git
```

Masuk ke dalam folder project hasil clone tsb.
```sh
$ cd fdhlmhd.github.io/
```
Membuat branch baru untuk manambahkan code kita pada project tsb.
```sh
$ git checkout -b new_branch
```
Mulai otak atik code dalam project tsb.

Setelah dirasa cukup kemudian lakukan add.
```sh
$ git add .
```
Lalu commit.
Misal :
```sh
$ git commit -m "update code"
```
Kemudian Push hasil code kita dalam branch yang kita buat.
```sh
$ git push origin new-branch
```
Setelah itu lakukan Pull Request kepada pemilik repository tersebut.

### Contoh Menerima Pull Request.

Lakukan penambahan kontributor untuk project kita.

Setelah menerima pull request maka lakukan ini pada folder project kita.
```sh
$ git fetch origin nama_branch:nama_branch
```
Kemudian cek isi kodingan pada branch baru tsb.
```sh
$ git checkout nama_branch
```
 Apabila diterima kodingan dari branch baru tsb.
 Maka lakukan : 
 ```sh
$ git checkout master
$ git rebase nama_branch
```
