# Task Day 1 — Dumbways
**Nama:** Dennis Jason

---

## 1. Secara konsep, jelaskan apa itu DevOps dengan bahasa kalian!

DevOps adalah role yang menghubungkan antara developer dengan tim operation. DevOps memiliki peran untuk mempercepat proses release aplikasi tapi tetap menjaga kualitas aplikasi tetap baik yaitu minim bug dan error dengan cara mengotomatisasi proses build, testing dan deployment.

---

## 2. Install Ubuntu Server 22.04.x LTS menggunakan Virtualbox/VMware/Virtualization Tool pilihan kalian dan buat step-by-step langkah instalasinya!

**STEP 1:** Buka VirtualBox dan klik new, lalu akan tampil sebuah form (gambar kiri)

![Step 1 - VirtualBox New VM](images/image15.png)
![Step 1 - VirtualBox New VM (2)](images/image33.png)

---

**STEP 2:** Pada bagian "Virtual machine name and operating system" isi nama VM, lokasi folder untuk menyimpan data VM dan pilih iso image instalasi os linux ubuntu server yang sudah disiapkan. Kemudian pastikan kolom OS, OS Distribution dan OS Version sudah sesuai dengan iso image yang dipilih. Lalu biarkan bagian "Proceed with Unattended Installation" tidak tercentang.

![Step 2 - VM Name and OS](images/image32.png)

---

**STEP 3:** Pada bagian "Specify virtual hardware" tentukan jumlah RAM dan CPU yang dibutuhkan.

![Step 3 - Specify Virtual Hardware](images/image11.png)

---

**STEP 4:** Pada bagian "Specify virtual hard disk" pilih *Create a New Virtual Hardrive*. Kemudian tentukan jumlah storage yang dibutuhkan untuk virtual machine. Lalu klik finish.

![Step 4 - Virtual Hard Disk](images/image34.png)

---

**STEP 5:** Pilih virtual machine yang telah dibuat, lalu klik start dan virtual machine akan berjalan seperti gambar di kiri.

![Step 5 - Start VM](images/image12.png)
![Step 5 - VM Running](images/image10.png)

---

**STEP 6:** Pilih bahasa untuk instalasi. Direkomendasikan menggunakan bahasa inggris agar mudah di solve ketika ada issue.

![Step 6 - Language Selection](images/image17.png)

---

**STEP 7:** Pilih *continue without updating* karena kita ingin menginstal linux yang sudah kita pilih versinya bukan yang terbaru.

![Step 7 - Continue Without Updating](images/image9.png)

---

**STEP 8:** Pilih layout keyboard, disarankan tidak perlu diubah langsung klik *done*.

![Step 8 - Keyboard Layout](images/image24.png)

---

**STEP 9:** Pilih tipe Ubuntu server yang akan diinstal, yang biasa atau *minimized* (ukuran kecil) dengan fitur secukupnya. Lalu pilih apakah ingin menginstall third party driver. Kemudian klik *done*.

![Step 9 - Ubuntu Server Type](images/image3.png)

---

**STEP 10:** Cek IPv4 Address untuk keperluan setting network di virtual machine.

![Step 10 - Check IPv4](images/image16.png)

---

**STEP 11:** Edit IPv4 pada network configuration interface "enp0s3".

![Step 11 - Edit IPv4](images/image5.png)
![Step 11 - Network Interface](images/image18.png)

---

**STEP 12:** Pilih pengkonfigurasian manual untuk IPv4.

![Step 12 - Manual IPv4](images/image19.png)

---

**STEP 13:** Isi konfigurasi IPv4 mengikuti di bawah ini. Setelah itu save.

![Step 13 - IPv4 Configuration](images/image31.png)

---

**STEP 14:** Klik done untuk proses berikutnya.

![Step 14 - Done](images/image22.png)

---

**STEP 15:** Untuk proxy configuration bisa kita skip dengan klik *Done*.

![Step 15 - Proxy Configuration](images/image26.png)

---

**STEP 16:** Ubuntu archive mirror configuration kita bisa skip juga dengan langsung klik *Done* dan kemudian muncul box pilih *Continue*.

![Step 16 - Mirror Configuration](images/image14.png)
![Step 16 - Continue](images/image29.png)

---

**STEP 17:** Pada bagian Guided storage configuration pilih Custom storage layout lalu klik *Done*.

![Step 17 - Storage Configuration](images/image28.png)

---

**STEP 18:** Pada *free space* pilih *Add GPT Partition*.

![Step 18 - Add GPT Partition](images/image35.png)

---

**STEP 19:** Set partisi dengan ukuran 7 giga byte dengan format ext4. Lalu klik *Create*.

![Step 19 - Partition 7GB ext4](images/image4.png)

---

**STEP 20:** *Add GPT Partition* pada *free space* lagi.

![Step 20 - Add GPT Partition Again](images/image27.png)

---

**STEP 21:** Set partisi dengan ukuran 2.8 giga byte dengan format swap. Untuk penampungan sementara seperti RAM tambahan. Lalu klik *Create*.

![Step 21 - Partition 2.8GB Swap](images/image21.png)

---

**STEP 22:** Pilih *Continue* untuk melakukan *destructive action* atau tindakan yang akan menghapus semua data dan mengisinya dengan instalasi dan data baru.

![Step 22 - Destructive Action](images/image2.png)

---

**STEP 23:** Pada *Profile Configuration* isi nama kita, nama server, username untuk login dan password untuk login juga.

![Step 23 - Profile Configuration](images/image7.png)

---

**STEP 24:** Kita skip untuk upgrade ubuntu pro lalu *Continue*.

![Step 24 - Skip Ubuntu Pro](images/image8.png)

---

**STEP 25:** Langsung *Done* karena kita hanya akan menginstal Ubuntu tanpa install OpenSSH server.

![Step 25 - Skip OpenSSH](images/image25.png)

---

**STEP 26:** Lalu ada pemilihan tambahan aplikasi yang ingin sekali kita install (tidak sempat ter-capture), lalu klik *Done* untuk langsung menginstal.

![Step 26 - Additional Apps](images/image20.png)

---

**STEP 27:** Setelah selesai instalasi lakukan re-boot.

![Step 27 - Reboot](images/image13.png)

---

**STEP 28:** Lakukan login pertama kali.

![Step 28 - First Login](images/image23.png)

---

## 3. Gunakan IP Address xxx.xxx.xxx.208 untuk server VM kalian!

![IP Address Configuration](images/image1.png)

---

## 4. Pastikan Ubuntu Server kalian ada jaringan dengan test menggunakan command `ping 8.8.8.8` / `ping google.com`

![Ping Test](images/image6.png)
![Ping google.com](images/image30.png)
