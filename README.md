### CARA PENGGUNAAN GIT

**1. Download Aplikasi Git**

> Buka website resmi git [https://git-scm.com/](url), kemudian pilih git sesuai perangkat yang anda gunakan. Jika menggunakan windows maka klik pada tulisan windows, kemudian unduh Git sesuai dengan arsitektur komputer anda. Jika menggunakan 64bit, unduh yang 64bit. Begitu juga jika menggunakan 32bit. 
<img width="775" alt="Download git" src="https://user-images.githubusercontent.com/72985112/96274746-15b01000-0ffb-11eb-9716-04d6ca24a5fd.png">

**2. Instalasi Git**

> Instal Git pada perangkat komputer anda.
Jika sudah berhasil terinstal, untuk mencobanya, silahkan buka CMD atau PowerShell, kemudian ketik perintah
`git --version`
<img width="326" alt="cut git version" src="https://user-images.githubusercontent.com/72985112/96277156-18f8cb00-0ffe-11eb-9d25-69cc778c346d.png">

**3. Melakukan Konfigurasi Awal**

> Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email.
Apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah _git commit_.
Silahkan lakukan konfigurasi dengan perintah berikut ini:
`$ git config --global user.name "username anda"`
`$ git config --global user.email "email anda"`
<img width="361" alt="1  Cut Menambahkan global config" src="https://user-images.githubusercontent.com/72985112/96276947-d6cf8980-0ffd-11eb-9759-8b4d04f48604.png">

**4. Membuat Repositori Lokal**

> Buat folder aktif, misalnya Lab_pemrogramans1, kemudian klik kanan pada folder tersebut, lalu klik _git bash here_
<img width="621" alt="cut git bash here" src="https://user-images.githubusercontent.com/72985112/96277592-ab996a00-0ffe-11eb-8e7f-34956198bfc2.png">

> Kemudian buat folder project praktikum dengan nama Latihan1 dengan cara memasukan perintah berikut:
`$ mkdir Latihan1`
`$ cd Latihan1`
<img width="353" alt="2  Cut Membuat reposiory local" src="https://user-images.githubusercontent.com/72985112/96278465-bacce780-0fff-11eb-8afb-57af1dc51204.png">

> Jalankan perintah _git init_ untuk membuat repository lokal
`$ git init`
<img width="432" alt="git init" src="https://user-images.githubusercontent.com/72985112/96278930-4cd4f000-1000-11eb-9600-5c675df8ccb6.png">

> Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git
<img width="577" alt="cut git" src="https://user-images.githubusercontent.com/72985112/96279370-c836a180-1000-11eb-8856-e625cbf7fbce.png">

**5. Menambahkan File Baru Pada Repository**

> Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository). disini kita akan coba buat satu file bernama README.md (text file) dengan menggunakan perintah :
`$ echo "#Latihan 1" >> README.md`
<img width="329" alt="echo" src="https://user-images.githubusercontent.com/72985112/96279972-94a84700-1001-11eb-9c94-43f20256a2ca.png">

> Untuk menambah file yang baru saja dibuat tersebut gunakan perintah _git add_
`$ git add README.md`
<img width="452" alt="git add" src="https://user-images.githubusercontent.com/72985112/96280329-0bdddb00-1002-11eb-9b92-3b5cab5a10ba.png">
maka file README.md berhasil ditambahkan
<img width="497" alt="readme git" src="https://user-images.githubusercontent.com/72985112/96280574-4e9fb300-1002-11eb-9d3c-4f593d3bb524.png">

**6. Commit (Menyimpan perubahan ke database)**

> Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah berikut:
`$ git commit --m "komentar commit"`
<img width="432" alt="commit" src="https://user-images.githubusercontent.com/72985112/96280963-e0a7bb80-1002-11eb-8cf4-d137c69a2fdc.png">

**7. Membuat Repository Server**

> Server reopsitory yang digunakan adalah [http://github.com](url)
> Buatlah akun github, kemudian pada laman github klik tombol start a project
<img width="645" alt="start a new project" src="https://user-images.githubusercontent.com/72985112/96281761-fec1eb80-1003-11eb-8588-fa7cde79d2bf.png">

atau klik new repository dari menu icon +
<img width="182" alt="new repository" src="https://user-images.githubusercontent.com/72985112/96281939-3b8de280-1004-11eb-966a-870696a987c9.png">

> Isi nama repositorynya, misalnya: labpy1, kemudian klik tombol create repository.
<img width="669" alt="7  Membuat repistory server2" src="https://user-images.githubusercontent.com/72985112/96282817-6a588880-1005-11eb-8087-6dcf1d1b8cbb.png">

**8. Menambahkan Remote Repository**
Untuk menambahkan remote repository server, gunakan perintah:
`$ git remote origin [url]`
 
<img width="411" alt="8  Menambahkan remote repository" src="https://user-images.githubusercontent.com/72985112/96283122-ed79de80-1005-11eb-8338-fc1a95b151e5.png">

**9.PUSH (Mengirim Perubahan Ke Server)**

> Untuk mengirim perubahan pada local repository ke server gunakan perintah berikut:
`$git push -u origin master`
<img width="405" alt="9  Push (Mengirim perubahan ke server)" src="https://user-images.githubusercontent.com/72985112/96283476-76911580-1006-11eb-932a-7aaf9c6310a6.png">

> Perintah ini akan meminta memasukkan username dan password pada akun github.com
<img width="735" alt="login" src="https://user-images.githubusercontent.com/72985112/96283646-b3f5a300-1006-11eb-97c0-269e0bb843a3.png">

**10. Melihat Hasil Pada Server Repository**

> Buka laman github.com, arahkan pada repositorinya. Maka halaman tersebut akan berubah sesuai dengan apa yang telah anda buat tadi.
<img width="957" alt="hasil repository" src="https://user-images.githubusercontent.com/72985112/96283988-2ebebe00-1007-11eb-91c8-6ef26964af18.png">

**11. Clone Repository**

> Clone repository, pada dasarnya adalah mengcopy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory). 
untuk melakukan cloning, gunakan perintah berikut:
`$ git clone [url]`
<img width="421" alt="clonning" src="https://user-images.githubusercontent.com/72985112/96284517-e05def00-1007-11eb-9436-37e07da9e4cc.png">

