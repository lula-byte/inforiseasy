# Pusat Nilai Informatika - SMP IT Insan Mulia

Aplikasi database nilai Informatika untuk guru (halaman admin saja). Satu file `index.html`, tanpa server dan tanpa instalasi.

## Fitur
- Dashboard: grafik perkembangan nilai per tingkat (7, 8, 9) atau per kelas, grafik batang 3D rata-rata kelas, siswa nilai tertinggi, siswa perlu bimbingan khusus, siswa perlu dipantau, rata-rata per komponen.
- Data Nilai: CP1-CP4, TP1-TP4, Rata-rata, ASTS, ASAT, Nilai Akhir, Keterangan. Nilai di bawah KKM (75) ditandai merah dan ▼. Ada pencarian, filter kelas, urutan, dan Edit cepat langsung di tabel.
- Profil siswa: klik nama siswa untuk melihat seluruh nilai, peringkat kelas, dan grafik dibanding rata-rata kelas.
- Input Data: satu siswa lengkap dengan nilai, atau tempel daftar nama satu kelas sekaligus.
- Pengaturan: ubah KKM, backup JSON, ekspor CSV (Excel), pulihkan backup.

## Rumus
- Rata-rata = rata-rata CP1-CP4 dan TP1-TP4 (kolom kosong tidak dihitung)
- Nilai akhir = rata-rata dari (Rata-rata, ASTS, ASAT)
- ✔ Tuntas, ◐ Tuntas tetapi 2 komponen atau lebih di bawah KKM, ▼ Remedial (nilai akhir di bawah KKM)

## Memasang di GitHub Pages
1. Buat repository baru, misalnya `nilai-informatika`.
2. Unggah `index.html` dan `README.md`.
3. Buka Settings > Pages, pilih Branch `main` dan folder `/ (root)`, lalu Save.
4. Aplikasi bisa dibuka di `https://USERNAME.github.io/nilai-informatika/`.

## Catatan penting
Data disimpan di localStorage peramban guru. Artinya data hanya ada di perangkat dan peramban yang dipakai. Lakukan backup JSON secara berkala di menu Pengaturan. Jika repository dibuat publik, jangan mengunggah file backup berisi data siswa.
