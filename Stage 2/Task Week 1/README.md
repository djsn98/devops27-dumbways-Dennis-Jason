# TASK WEEK 1

## Deploy Mysql
> STEP 1 : Menyalakan server Appserver-1
>
> ![image5](images/image5.png)
>
> STEP 2 : Buat user baru untuk server
>
> ![image4](images/image4.png)
>
> STEP 3 : Setup agar dapat melakukan ssh tanpa pasword dengan ssh key
>
> ![image18](images/image18.png)
>
> ![image38](images/image38.png)
>
> ![image1](images/image1.png)
>
> STEP 4 : Ssh tanpa password
>
> ![image41](images/image41.png)
>
> STEP 5 : Lakukan sudo apt update  
> ![image6](images/image6.png)
>
> STEP 6 : Menginstall mysql server
>
> ![image2](images/image2.png)
>
> STEP 7 : Cek apakah Mysql sudah berjalan

![image11](images/image11.png)

STEP 8 : Masuk ke MySql

![image35](images/image35.png)

STEP 9 : Setup mysql_secure_installation

![image47](images/image47.png)

STEP 10 : Menambahkan password ke user root

![image24](images/image24.png)

STEP 11 : Menambah user baru ke MySql

![image28](images/image28.png)

STEP 12 : Menambahkan hak akses (previleges) ke user mysql baru

![image36](images/image36.png)

STEP 13 : Masuk ke Mysql dengan user baru

![image9](images/image9.png)

STEP 14 : Membuat database

![image17](images/image17.png)

STEP 15 : Mengubah bind address pada file
/etc/mysql/mysql.conf.d/mysqld.cnf

![image7](images/image7.png)

## Role Based
> STEP 1 : Membuat database “demo” dan tabel “transaction”
>
> ![image20](images/image20.png)
>
> STEP 2 : Membuat role dan hak akses
>
> ![image22](images/image22.png)
>
> STEP 3 : Membuat user dengan nama Dennis dan role admin
>
> ![image23](images/image23.png)
>
> STEP 4 : Membuat user dengan nama guest dan role guest
>
> ![image21](images/image21.png)

STEP 5 : Tes semua user dengan melakukan login

![image3](images/image3.png)

![image48](images/image48.png)

## Remote User
> STEP 1 : Jalankan server dan pastikan mysql berjalan
>
> ![image40](images/image40.png)
>
> STEP 2 : Lakukan remote ke database mysql dengan perintah “mysqlsh
> –sql
>
> anonym@192.168.0.7:3306”
>
> ![image19](images/image19.png)

## Deploy Wayshub Backend
> STEP 1 : Menjalankan server Gateway-server
>
> ![image16](images/image16.png)
>
> STEP 2 : SSH ke server Gateway-server
>
> ![image30](images/image30.png)
>
> STEP 3 : Install NodeJS 14
>
> ![image12](images/image12.png)
>
> STEP 4 : Clone repo wayshub-backend di github dumwaysdev
> ![image26](images/image26.png)
>
> STEP 5 : Edit file config/config.json pada folder project
> wayshub-backand
> ![image52](images/image52.png)
>
> ![image27](images/image27.png)
>
> STEP 6 : Jalankan server DB dan pastikan DB MySql berjalan
>
> ![image50](images/image50.png)
>
> STEP 7 : Buat database dengan nama wayshub
>
> ![image44](images/image44.png)
>
> STEP 8 : Mengubah NodeJS yang digunakan menjadi versi 14
>
> ![image15](images/image15.png)
>
> STEP 9 : Install semua library pada project wayshub-backend
>
> ![image29](images/image29.png)
>
> STEP 10 : Migrasikan database dengan sequelize agar semua tabel
> terbuat
>
> ![image51](images/image51.png)
>
> STEP 11 : Install library pm2 untuk menjalankan aplikasi NodeJS di
> background
>
> ![image46](images/image46.png)
>
> STEP 12 : Jalankan aplikasi wayshub-backend dengan pm2
>
> ![image45](images/image45.png)
>
> STEP 13 : Cek di browser apakah aplikasi backend sudah berjalan
>
> ![image49](images/image49.png)

## Clone Wayshub Frontend Application
> STEP 1 : Clone repo wayshub-frontend di github dumbwaysdev
>
> ![image43](images/image43.png)
>
> STEP 2 : Mengubah menggunakan NodeJS versi 14
>
> ![image37](images/image37.png)
>
> STEP 3 : Mengedit file src/config/[<u>api.js</u>](http://api.js) di
> folder project wayshub-frontend pada
>
> bagian baseURL dengan domain backend
>
> ![image32](images/image32.png)
>
> ![image53](images/image53.png)
>
> STEP 4 : Menambahkan di file h C:\Windows\System32\drivers\etc\hosts
> agar me
>
> -routing domain [<u>wayshub.dennis.xyz</u>](http://wayshub.dennis.xyz)
> ke ip 192.168.0.8
>
> ![image33](images/image33.png)
>
> STEP 5 : Pastikan nginx running
>
> ![image13](images/image13.png)
>
> STEP 6 : Buka file /etc/nginx/sites-enabled/wayshub.conf dan tambahkan
> konfigurasi
>
> nginx untuk melakukan routing dari domain ke ip
>
> ![image31](images/image31.png)
>
> ![image34](images/image34.png)
>
> STEP 7 : Cek syntax dan test file konfigurasi nginx yang telah
> ditambahkan dengan
>
> perintah “sudo nginx -t”

![image14](images/image14.png)

STEP 8 : Reload file konfigurasi nginx

![image25](images/image25.png)

> STEP 9 : Pada folder project wayshub-frontend tambahkan file
> ecosystem.config.js
>
> ![image10](images/image10.png)
>
> STEP 10 : Install semua library pada project wayshub-frontend
>
> ![image39](images/image39.png)
>
> STEP 11 : Jalankan aplikasi wayshub-frontend dengan pm2
>
> ![image8](images/image8.png)
>
> STEP 12 : Cek apakah aplikasi wayshub-frontend sudah jalan dengan
> browser
>
> ![image42](images/image42.png)
