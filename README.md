# Instalasi Flowgorithm di Elementary OS 6 Odin

<img src="https://github.com/Rizky1408/Quis-III/blob/main/assets/images%20(1).jpeg" width="650">

Untuk menginstal Flowgorithm pada linux khususnya distro Elementary OS,hal pertama yang harus kita lakukan yaitu menginstall <b>Wine</b>.
Wine berfungsi untuk menjalankan aplikasi windows di linux,dikarenakan Flowgorithm tidak support untuk operasi system berbasis linux,sehingga
Dibutuhkanlah sebuah media yang bisa menjembatani hal tersebut.<br><br>
Untuk menginstall wine pertama yang harus kita lakukan yaitu mengaktifkan support 32 bit dengan command <br>

Check instalasi architectures OS kita
```
$ dpkg --print-architecture
```

Jika architectures 32 bit kita sudah terinstall,ikuti command di bawah ini untuk melihat respon "i386"
```
$ dpkg --print-foreign-architectures
```
Jika architectures 32 bit tidak tampil,maka ikuti command dibawah ini
```
$ sudo dpkg --add-architecture i386
```
Cek lagi dengan perintah berikut ini
```
$ dpkg --print-foreign-architectures
```
Jika architectures 32 bit sudah tampil selanjutnya Install apt-add-repository<br><br>
Update Repository
```
$ sudo apt update
```
Tambahkan apt-add-repository
```
$ sudo apt install software-properties-common
```
Tambahkan repository ubuntu WineHQ 
```
$ wget -nc https://dl.winehq.org/wine-builds/winehq.key
$ sudo -H gpg -o /etc/apt/trusted.gpg.d/winehq.key.gpg --dearmor winehq.key
```

Tambahkan Repositorynya
```
$ sudo apt-add-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ focal main'
```
Update package
```
$ sudo apt update
```
Install Wine dengan command
```
$ sudo apt install --install-recommends winehq-stable
```
Setelah instalasi wine selesai,tinggal kita check dengan command
```
$ wine --version
```
saat tutorial ini dibuat versi wine sudah di wine-6.0.1<br><br>
Setelah menginstall wine langkah selanjutnya kita tinggal menginstall Flowgorithm,download filenya di situs resmi 
<a href="http://www.flowgorithm.org/download/index.html">Flowgorithm</a> download di bagian Macintosh & Linux <br><br>
<img src="https://github.com/Rizky1408/Quis-III/blob/main/assets/ss%203.png" width="650"> <br>
Setelah mendownload filenya kita tinggal mengklik 2 kali pada file instalasinya sama seperti kita menginstall aplikasi windows pada umumnya.
tampilan awalnya akan seperti dibawah ini<br>
<img src="https://github.com/Rizky1408/Quis-III/blob/main/assets/ss%204.png" width="650">

# Membuat Program Hello World Dengan Flowgorithm

Untuk membuat program Hello World pertama kita mengklik pada bagian anak panah dibawah "start" setelah itu tampilan akan seperti ini<br>
<img src="https://github.com/Rizky1408/Quis-III/blob/main/assets/ss%205.png" width="650">

Langkah selanjutnya kita tinggal mengklik pada bagan bertuliskan output dan langkah seterusnya tinggal kita mengklik 2 kali pada bagan output dibawah start dan menuliskan "Hello World" dengan tanda petik maka tampilannya akan seperti gambar di bawah ini<br>
<img src="https://github.com/Rizky1408/Quis-III/blob/main/assets/ss%206.png" width="650">

Jika sudah seperti gambar di atas tinggal kita mengklik ok dan jalankan programnya dengan menekan tombol run (Segitiga kesamping warna hijau) maka tampilannya akan seperti gambar dibawah<br>
<img src="https://github.com/Rizky1408/Quis-III/blob/main/assets/ss%207.png" width="650">

Itu adalah langkah-langkah menginstall Flowgorithm pada Elementary OS,Jika ada salah kata ataupun definisi, mohon di koreksi.
Terimakasih












