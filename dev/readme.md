# Folder /dev pada Linux

  Untuk pemula, bayangkan folder /dev sebagai penghubung atau jembatan antara program
dan perangkat keras di komputer anda. Di linux, semuanya diperlakukan sebagai berkas
perangkat keras. Folder /dev berisi "berkas khusus" yang mewakili perangkat fisik 
(seperti harddisk, keyboard, dan USB) dan perangkat virtual (seperti memori dan
generator angka acak).

### Konsep "Semuanya adalah berkas"

  Dalam linux, ketika sebuah program ingin berinteraksi dengan sebuah perangat ia
tidak langsung "berbicara" dengan perangkat keras tersebut. Sebaliknya, ia akan 
membaca atau menulis ke berkas khusus yang ada di /dev, seolah-olah itu adalah
berkas biasa. Sistem operasi (kernel) yang akan menerjemahkan aksi adalah berkas biasa.
Sistem operasi (kernel) yang akan menerjemahkan aksi tersebut menjadi instruksi yang
bisa di pahami oleh perangkat keras.

### Contoh penggunaan

-  Akses ke harddisk:
Setiap harddisk atau partisi diwakili oleh sebuah berkas di /dev. Contohnya, /dev/sda
mungkin adalah harddisk pertama anda, dan /dev/sda1 adalah partisi pertama di disk 
tersebut.

- Membuang output:
Berkas /dev/null adalah pernagkat virtual yang sangat berguna. Semua data yang anda
kirim ke berkas ini akan dibuang dan diabaikan. Ini sering di gunakan saat menjalankan
perintah di terminal dan anda tidak ingin melihat keluarannya.

- Mengakses input|output acak:
Berkas /dev/random dan dev/urandom berfungsi sebagai generator angka acak yang bisa
digunakan oleh program untuk tujuan keamanan, seperti membuat kunci enkripsi.

### Jenis - jenis berkas di /dev

  Anda da[at melihat jenis berkas di /dev dengan menggunakan perintah "ls -l/dev"
di terminal. Perhatikan karakter pertama pada setiap baris:

- b (Block devices):
Perangkat yang membaca dan menulis data dalam blok-blok dengan ukuran tetap. Contohnya,
harddisk, solid state drive, dan CD-ROM.

- c (Character devices):
Perangkat yang membaca dan menulis data satu karakter pada satu waktu. Contohnya,
terminal, keyboard, dan mouse.

-l (Link simbolik):
Beberapa berkas di /dev adalah link ke berkas pernagkat yang sebenarnya. Contohnya,
/dev/cdrom sering kali merupakan link simbolik ke perangkat CD-ROM anda yang 
sesungguhnya, seperti /dev/sr0

### Mengapa ini penting bagi pemula?

  Memahami /dev membantu anda memahami cara linux mengelola perangkat keras. Meskipun
anda jarang berinteraksi langsung dengan berkas di /dev, pengetahuan ini akan berguna
saat:

- Melakukan partisi disk: Anda akan bekerja dengan nama perangkat seperti /dev/sda1
saat menggunakan utilitas partisi.

- Mencari informasi perangkat: Anda dapat mencari informasi tentang perangkat keras
sistem anda dengan menjelajahi subdirektori di /dev.

- Melakukan tindakan spesifik: Sesekali, anda mungkin perlu melakukan tindakan tingkat
tendah pada suatu perangkat, seperti melakukan klong disk menggunakan perintah dd dengan
menunjuk langsung ke berkas perangkat di /dev.
