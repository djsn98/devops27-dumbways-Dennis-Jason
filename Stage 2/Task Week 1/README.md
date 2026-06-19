**TASK WEEK 1**

1.  **Deploy Mysql**

> STEP 1 : Menyalakan server Appserver-1
>
> ![](images/image3.png)
>
> STEP 2 : Buat user baru untuk server
>
> ![](images/image1.png)
>
> STEP 3 : Setup agar dapat melakukan ssh tanpa pasword dengan ssh key
>
> ![](images/image2.png)
>
> ![](images/image24.png)
>
> ![](images/image14.png)
>
> STEP 4 : Ssh tanpa password
>
> ![](images/image13.png)
>
> STEP 5 : Lakukan sudo apt update\
> ![](images/image5.png)
>
> STEP 6 : Menginstall mysql server
>
> ![](images/image15.png)
>
> STEP 7 : Cek apakah Mysql sudah berjalan

![](images/image23.png)

STEP 8 : Masuk ke MySql

![](images/image4.png)

STEP 9 : Setup mysql_secure_installation

![](images/image22.png)

STEP 10 : Menambahkan password ke user root

![](images/image6.png)

STEP 11 : Menambah user baru ke MySql

![](images/image20.png)

STEP 12 : Menambahkan hak akses (previleges) ke user mysql baru

![](images/image16.png)

STEP 13 : Masuk ke Mysql dengan user baru

![](images/image18.png)

STEP 14 : Membuat database

![](images/image7.png)

STEP 15 : Mengubah bind address pada file
`/etc/mysql/mysql.conf.d/mysqld.cnf`

![](images/image19.png)

2.  **Role Based**

> STEP 1 : Membuat database "demo" dan tabel "transaction"
>
> ![](images/image17.png)
>
> STEP 2 : Membuat role dan hak akses
>
> ![](images/image8.png)
>
> STEP 3 : Membuat user dengan nama Dennis dan role admin
>
> ![](images/image9.png)
>
> STEP 4 : Membuat user dengan nama guest dan role guest
>
> ![](images/image10.png)

STEP 5 : Tes semua user dengan melakukan login

![](images/image12.png)

![](images/image21.png)

3.  **Remote User**

> STEP 1 : Jalankan server dan pastikan mysql berjalan
>
> ![](images/image25.png)
>
> STEP 2 : Lakukan remote ke database mysql dengan perintah "mysqlsh
> --sql
>
> anonym@192.168.0.7:3306"
>
> ![](images/image11.png)
