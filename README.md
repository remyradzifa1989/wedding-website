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


<img width="625" height="700" alt="Screenshot 2026-08-10 124240" src="https://github.com/user-attachments/assets/a34a0c83-3987-4e0e-af5e-33f45a94075a" />

<img width="628" height="654" alt="Screenshot 2026-08-10 124306" src="https://github.com/user-attachments/assets/b8be58fa-ce1b-47b4-987f-6a5fe0314997" />

<img width="627" height="641" alt="Screenshot 2026-08-10 124323" src="https://github.com/user-attachments/assets/ded93fa6-14d1-4732-9db8-5fd89c6cb55f" />

<img width="625" height="719" alt="Screenshot 2026-08-10 124343" src="https://github.com/user-attachments/assets/3bd75172-682c-4d7a-9497-ae1f712bc6d5" />

<img width="626" height="721" alt="Screenshot 2026-08-10 124402" src="https://github.com/user-attachments/assets/5c4baff0-d76a-455f-8b2f-ab43b9b201fc" />

<img width="541" height="538" alt="Screenshot 2026-08-10 124418" src="https://github.com/user-attachments/assets/173e13ea-9672-4bb9-8837-53179352a3e5" />

<img width="390" height="212" alt="Screenshot 2026-08-10 124436" src="https://github.com/user-attachments/assets/48f8231a-81ab-48ae-953a-92ff44735c6e" />


<img width="463" height="697" alt="Screenshot 2026-08-10 123832" src="https://github.com/user-attachments/assets/e0e31c09-9ee5-4cef-9b6e-d269214c558a" />

<img width="456" height="698" alt="Screenshot 2026-08-10 123852" src="https://github.com/user-attachments/assets/fc9268bd-0a92-4325-86c6-c4447dcdcc52" />

<img width="463" height="686" alt="Screenshot 2026-08-10 123911" src="https://github.com/user-attachments/assets/a3b7a8d7-9c37-4d39-8144-e72bb1aef058" />

<img width="464" height="678" alt="Screenshot 2026-08-10 123929" src="https://github.com/user-attachments/assets/7276a0ab-73db-4dc0-a2b1-cf8590b2986f" />

<img width="466" height="683" alt="Screenshot 2026-08-10 123952" src="https://github.com/user-attachments/assets/ff97d822-7a93-4bc0-b2b4-032bf4db1ec6" />

<img width="465" height="655" alt="Screenshot 2026-08-10 124009" src="https://github.com/user-attachments/assets/738edb78-19c4-4bb0-b488-0754f33ed6b8" />








