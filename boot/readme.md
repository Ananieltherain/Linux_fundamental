Folder /boot di linux adalah tempat penyimpanan semua file penting yang di butuhkan
komputer unttuk bisa menyala atau memulai sistem operasi linux. Anda bisa membayangkannya
seperti sebuah kotak peralatan khusus yang berisi semua instruksi dan komponen utama yang
diperlukan sebelum sistem linux berjalan sepenuhnya.

## Mengapa folder /boot penting?
- Proses booting:
  Saat anda menekan tombol daya, komputer akan membaca instruksi dari folder ini untuk
  memuat program yang disebut bootloader.
- Bootloader (misalnya, GRUB):
  Program ini bertugas menampilkan menu di mana anda bisa memilih sistem operasi atau
  kernel mana yang akan dimuat. Setelah anda memilih, bootloader akan mengambil file-
  file dari folder /boot untuk menjalankan sistem operasi yang anda pilih.
- Kernel linux:
  Kernel adalah inti dari sistem operasi yang mengelola sumber daya perangkat keras.
  File kernel utama disimpan di folder ini.
- Keamanan:
  Karena berisi file-file yang sangat penting, folder /boot biasanya di linugi dan tidak
  boleh diutak-atik secara sembarangan. Mengubah atau menghapus file di sini bisa membuat
  sistem anda tidak bisa menyala.

## Isi dalam folder /boot
Di dalam folder ini, anda akan menemukan beberapa file dan folder khusus:

- File kernel (misalnya, vmlinuz-5.15.0-xx-generic):
  Ini adalah file kernel linux yang sebenarnya. Namanya biasanya di awali dengan vmlinuz
  dan diikuti oleh nomor versi.
- File initrd.img:
  File ini adalah initial RAM disk. Ia berfungsi sebagai sistem file sementara yang
  digunakan selama proses booting untuk memuat modul-modul penting yang di butuhkan
  kernel.
- Folder grub:
  Folder ini berisi file konfigurasi dan skrip untuk bootloader GRUB. File utamanya
  biasanya ada di /etc/default/grub atau /boot/grub/grub/cfg.

  ## Perlu partsi terpisah?
  Secara standar, folder /boot berada di partisi yang sama dengan sistem file root (/).
  Namun, pada beberapa kasus, seperti sistem yang menggunakan skema partisi tertentu
  (misalnya UEFI) atau untuk alasan keamanan, folder /boot bisa dibuat di partisi
  terpisah. Jika partisi /boot terpisah, ruangnya perlu diperhatikan agar tidak penuh
  saat tidak penuh saat ada pembaruan kernel.
