# Tugas-6---Best-Time-to-Post
Workflow n8n untuk menemukan 5 jam terbaik untuk posting berdasarkan data historis postingan, lalu mengirim hasilnya sebagai laporan harian ke Telegram.

Nama: [Isi nama kamu] NIM / Kelas: [Isi NIM dan kelas]

Alur Workflow
Baca Data Posting - Google Sheets membaca jam tayang, Likes, Comments, dan Shares.
Hitung Engagement Score - Node Code (JavaScript) dengan rumus: Likes x1 + Comments x2 + Shares x3.
Agregasi Rata-rata per Jam - Node Code menghitung rata-rata per jam, mengurutkan, dan mengambil Top 5.
Clear Hasil Analisis Lama - Google Sheets (operasi Clear) menghapus data lama sebelum data baru ditulis.
Tulis Hasil Analisis Baru - Google Sheets (Append) menyimpan Top 5 ke tab Hasil Analisis.
Format dan Kirim ke Telegram - Pesan dengan emoji dan teks tebal dikirim sebagai laporan harian.
Hasil (Top 5 Jam Terbaik)
Peringkat	Jam	Rata-rata Engagement
1	15:00	464
2	12:00	386
3	18:00	290
4	09:00	205
5	20:00	175
Isi Repository
Tugas6_Best_Time_to_Post.json - file workflow n8n
Laporan_Tugas6.pdf - laporan berisi screenshot tiap langkah
Cara Pakai
Import file JSON di n8n (Create workflow, menu titik tiga, Import from File).
Pilih credential Google Sheets dan arahkan ke spreadsheet kamu.
Isi credential Telegram dan ganti ISI_CHAT_ID_KAMU dengan Chat ID kamu.
Klik Execute workflow.

Catatan: token bot dan Chat ID tidak disertakan di repository ini.
