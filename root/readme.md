# Folder /root Linux

Folder /root adalah direktori home khusus untuk pengguna root (administrator sistem di
Linux). Anda dapat menganggapnya sebagai folder "Dokumen Saya" atau "Pengguna" di 
windows, tetapi untuk pengguna dengan hak akses tertinggi.

### Perbedaan penting: /root & /

Karena namanya mirip, banyak pemula dalam linux yang sering salah membedakan antara
direktori /root dan /

Apa itu direktori / (Direktori Akar):

- Paling atas dalam hierarki sistem berkas linux. Semua direktori dan berkas lain
  berada di bawah direktori ini.
- Berisi direktor - direktori penting untuk seluruh sistem, seperti /etc, /home, /bin,
  /usr, /var dsb.
- Semua pengguna memiliki akses ke direktori ini dan subdirektorinya, meskipun dengan
  batasan yang ketat.

Apa itu direktori /root:

- Direktori home untuk pengguna superuser (Root).
- Direktori home untuk pengguna superuser (Root).
- Berisi berkas pribadi dan konfigurasi yang hanya bisa diakses oleh pengguna root.
- Hanya pengguna root yang dapat mengaksesnya secara langsung. Pengguna lain tidak
  dizinkan masuk karena alasan keamanan.

### Mengapa folder /root itu penting?

1. Keamanan dan isolasi:
   Dengan memisahkan home direktori root dari home direktori pengguna biasa (/home/
   nama_pengguna), tindakan yang dilakukan sebagai root akan tidak secara sengaja
   mempenngaruhi berkas pribadi pengguna lain.
2. Tugas Administratif:
   Pengguna root menggunakan direktori ini untuk menyimpan skrip, berkas log, atau
   berkas konfigurasi penting yang hanya relavan untuk administrasi sistem.
3. Mencegah kesalahan:
   Dengan tidak menggunakan akun root untuk tugas sehari - hari, pengguna mengurangi
   risiko kerusakan sistem yang tidak disengaja. Jika ada malware yang terunduh,
   dampaknya akan terbatas pada direktori home pengguna, bukan seluruh sistem.
