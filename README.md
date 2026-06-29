========================================================================
  WEBSITE KAHWIN — Farid & Amy
  Panduan pemasangan di XAMPP (localhost + phpMyAdmin)
========================================================================

ISI KANDUNGAN ZIP
------------------------------------------------------------------------
  wedding-website/
    index.html              <- laman web (buka melalui browser)
    api/
      config.php            <- tetapan sambungan pangkalan data
      save_rsvp.php         <- simpan RSVP
      get_rsvps.php         <- baca senarai RSVP (papan pemuka)
      clear_rsvps.php       <- padam semua RSVP
    database/
      wedding.sql           <- struktur pangkalan data (import ke phpMyAdmin)
    README.txt              <- fail ini


LANGKAH PEMASANGAN
------------------------------------------------------------------------
1) Pasang & buka XAMPP. Klik "Start" pada Apache DAN MySQL.

2) Salin folder "wedding-website" ke dalam folder htdocs XAMPP:
     Windows : C:\xampp\htdocs\wedding-website
     macOS   : /Applications/XAMPP/htdocs/wedding-website

3) Buka phpMyAdmin di browser:
     http://localhost/phpmyadmin

4) Cipta pangkalan data:
     - Klik tab "Import"
     - Pilih fail: wedding-website/database/wedding.sql
     - Klik "Go" / "Import"
   (Ini akan cipta pangkalan data 'wedding_rsvp' dan jadual 'rsvps'.)

5) Semak tetapan sambungan di:
     wedding-website/api/config.php
   Untuk XAMPP default, tidak perlu ubah apa-apa:
     host     = localhost
     user     = root
     password = (kosong)
     database = wedding_rsvp

6) Buka website:
     http://localhost/wedding-website/

   SIAP! RSVP yang dihantar tetamu akan tersimpan ke MySQL,
   dan papan pemuka admin akan membacanya dari pangkalan data.


CARA GUNA
------------------------------------------------------------------------
- Tetamu: tekan "Sahkan Kehadiran" -> pilih kategori -> pilih kerusi
  -> isi borang -> "Sahkan RSVP". Skrin kejayaan papar QR + butang WhatsApp.

- Admin: di bahagian footer laman utama, klik "Papan Pemuka" untuk
  melihat jumlah RSVP, senarai tetamu, kehadiran, telefon & ucapan.


NOTA
------------------------------------------------------------------------
- Jika dibuka terus (double-click index.html tanpa server), website
  tetap berfungsi tetapi data hanya disimpan dalam browser (localStorage).
  Untuk simpan ke pangkalan data MySQL, mesti dibuka melalui XAMPP
  (http://localhost/...).

- Nama "Farid & Amy", tarikh 14 November 2026, dan lokasi adalah
  contoh — boleh ditukar dalam fail reka bentuk asal.

- Foto galeri kini placeholder. Hantar foto sebenar untuk digantikan.
========================================================================
