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


<img width="1041" height="894" alt="Screenshot 2026-09-03 101511" src="https://github.com/user-attachments/assets/67845ebe-b93b-4102-9225-0db67e58b3a2" />

<img width="886" height="900" alt="Screenshot 2026-09-03 101610" src="https://github.com/user-attachments/assets/08ea94fb-204c-44af-ac4e-c1e16ab86620" />

<img width="1598" height="601" alt="Screenshot 2026-09-03 102515" src="https://github.com/user-attachments/assets/8099ab1a-aab3-48d3-8dee-e75c6f514d8d" />

<img width="438" height="865" alt="Screenshot 2026-09-03 102620" src="https://github.com/user-attachments/assets/5cff73ee-baad-4f53-bad6-ccdf7c374579" />

<img width="657" height="905" alt="Screenshot 2026-09-03 102545" src="https://github.com/user-attachments/assets/d719b1f9-4130-4a30-a914-5768960d002f" />

<img width="597" height="798" alt="Screenshot 2026-09-03 101834" src="https://github.com/user-attachments/assets/5efca4aa-1246-402d-9f2a-1d71fad1bd1c" />

<img width="1889" height="900" alt="Screenshot 2026-09-03 101915" src="https://github.com/user-attachments/assets/9ea71fdd-6b36-40fd-ac62-967cdb0c5672" />

<img width="651" height="493" alt="Screenshot 2026-09-03 101948" src="https://github.com/user-attachments/assets/8ecc87b8-b096-4a44-8ef0-7c62e468914b" />

<img width="545" height="597" alt="Screenshot 2026-09-03 102016" src="https://github.com/user-attachments/assets/7ee0ccb9-b722-4245-b6ca-bff17cbe78ba" />

<img width="1670" height="899" alt="Screenshot 2026-09-03 102113" src="https://github.com/user-attachments/assets/ba8eb36a-a077-4630-8cc0-60400dc46232" />

<img width="1655" height="897" alt="Screenshot 2026-09-03 102149" src="https://github.com/user-attachments/assets/e750be58-1d80-4c13-8bca-77b596ce2be5" />

<img width="1671" height="904" alt="Screenshot 2026-09-03 102208" src="https://github.com/user-attachments/assets/2e4bdf3c-7c22-4403-808b-43577519c201" />

<img width="1669" height="898" alt="Screenshot 2026-09-03 102237" src="https://github.com/user-attachments/assets/d1bf74a5-16bf-43b8-b40a-3f87f9cd9652" />

<img width="1677" height="894" alt="Screenshot 2026-09-03 102257" src="https://github.com/user-attachments/assets/bd6989ef-2168-4815-9695-b2af6aec046a" />

<img width="1648" height="901" alt="Screenshot 2026-09-03 102319" src="https://github.com/user-attachments/assets/a7757dcf-3581-43cb-a86e-78311b035e4e" />

<img width="1143" height="806" alt="Screenshot 2026-09-03 102405" src="https://github.com/user-attachments/assets/fc9d2bb6-eafa-45ea-bdc3-6c3d07d56c60" />

<img width="1183" height="878" alt="Screenshot 2026-09-03 104213" src="https://github.com/user-attachments/assets/2b5b8f67-b5ee-4134-a699-9cb3bb4c92cc" />

<img width="911" height="760" alt="Screenshot 2026-09-03 104256" src="https://github.com/user-attachments/assets/560089ac-a8b5-4d46-a3e4-51f5d3c22fc2" />

<img width="893" height="622" alt="Screenshot 2026-09-03 104313" src="https://github.com/user-attachments/assets/d17d9efb-ab64-43b6-99ec-ad937ec942c2" />

<img width="724" height="820" alt="Screenshot 2026-09-03 104345" src="https://github.com/user-attachments/assets/0fb9bb16-480c-438f-8157-c1bf3a14f88b" />

<img width="790" height="843" alt="Screenshot 2026-09-03 104412" src="https://github.com/user-attachments/assets/2e5fea81-badc-4a2b-b3ef-d9b3a70c2b9d" />

<img width="1893" height="851" alt="Screenshot 2026-09-03 104443" src="https://github.com/user-attachments/assets/8d140e5a-6f73-4a15-9b0f-ed30ee125815" />

<img width="1106" height="830" alt="Screenshot 2026-09-03 104505" src="https://github.com/user-attachments/assets/0ce51281-1623-45f5-bd53-2092e8f705b0" />

<img width="1131" height="831" alt="Screenshot 2026-09-03 105055" src="https://github.com/user-attachments/assets/a190e4c1-7d83-452c-80c9-a10ca8640bdb" />

<img width="1097" height="591" alt="Screenshot 2026-09-03 105116" src="https://github.com/user-attachments/assets/24d57943-9602-408a-a460-58559d1fb9ae" />

<img width="565" height="694" alt="Screenshot 2026-09-03 105210" src="https://github.com/user-attachments/assets/a6c4506a-58df-4ace-b18e-b065b2cde20f" />


















