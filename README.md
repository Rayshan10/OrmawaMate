# OrmawaMate

**Your Guide to Student Programs**

OrmawaMate adalah prototipe chatbot berbasis AI yang dirancang untuk membantu mahasiswa memperoleh informasi mengenai program kemahasiswaan, khususnya program yang berkaitan dengan organisasi mahasiswa (Ormawa).

Proyek ini dikembangkan sebagai bagian dari pembelajaran pada bootcamp Hacktiv8 bersama IBM SkillsBuild dan menjadi fondasi awal untuk pengembangan aplikasi OrmawaMate di masa mendatang.

## Latar Belakang

Informasi mengenai program kemahasiswaan dapat tersebar di berbagai dokumen dan sumber. OrmawaMate dikembangkan sebagai asisten informasi yang membantu mahasiswa mencari dan memahami informasi tersebut melalui percakapan dengan chatbot.

## Tujuan

- Mempermudah mahasiswa dalam mencari informasi program kemahasiswaan.
- Membantu mahasiswa memahami informasi yang tersedia dalam dokumen referensi.
- Mengeksplorasi penerapan AI, embeddings, dan pencarian berbasis vektor untuk sistem tanya jawab.
- Menjadi fondasi pengembangan aplikasi OrmawaMate berikutnya.

## Fitur Utama

- **Conversational Q&A** — menerima pertanyaan pengguna melalui antarmuka chatbot.
- **Document Processing** — memproses dokumen menjadi potongan teks untuk pencarian informasi.
- **Semantic Search** — mencari konteks yang relevan menggunakan embeddings dan basis data vektor.
- **Context-Aware Responses** — menggunakan konteks hasil pencarian untuk membantu model menghasilkan jawaban.

## Teknologi

- **Langflow** — membangun dan menghubungkan alur chatbot secara visual.
- **Google Generative AI Embeddings** — mengubah teks menjadi representasi vektor.
- **Astra DB** — menyimpan dan mencari data berbasis vektor.
- **Google Gemini** — model bahasa untuk menghasilkan respons chatbot.

## Arsitektur Alur

Secara garis besar, alur chatbot terdiri dari dua bagian:

1. **Pemrosesan dokumen:** dokumen dibaca, teks dipecah menjadi beberapa bagian, kemudian dibuat embeddings dan disimpan di Astra DB.
2. **Proses tanya jawab:** pertanyaan pengguna digunakan untuk mencari konteks yang relevan. Konteks dan pertanyaan diteruskan ke prompt, kemudian diproses oleh model bahasa untuk menghasilkan jawaban.

## Struktur Repository

```text
OrmawaMate/
├── README.md
└── ormawamate-langflow.json
```

File JSON berisi konfigurasi alur Langflow yang dapat digunakan sebagai dasar untuk mengimpor dan mengembangkan kembali prototipe chatbot.

## Cara Menggunakan

1. Clone repository ini.
2. Pastikan Langflow sudah tersedia di lingkungan pengembangan.
3. Impor file `ormawamate-langflow.json` melalui fitur impor flow Langflow yang tersedia pada versi yang digunakan.
4. Periksa konfigurasi setiap komponen dan lengkapi kredensial layanan yang diperlukan.
5. Siapkan dokumen referensi yang akan digunakan sebagai sumber informasi chatbot.
6. Jalankan flow dan uji chatbot melalui antarmuka yang tersedia.

Nama menu impor dan detail konfigurasi dapat berbeda tergantung versi Langflow.

## Catatan Konfigurasi dan Keamanan

- Gunakan API key dan kredensial milik sendiri.
- Jangan memasukkan API key, token, atau rahasia layanan ke dalam repository publik.
- Periksa konfigurasi koneksi Astra DB dan model AI sebelum menjalankan flow.
- Jawaban chatbot bergantung pada dokumen referensi dan konfigurasi yang digunakan.

## Roadmap

- [x] Membuat prototipe chatbot menggunakan Langflow.
- [x] Menyimpan konfigurasi flow ke dalam repository GitHub.
- [ ] Melengkapi dokumentasi dan menambahkan screenshot prototipe.
- [ ] Mengevaluasi kualitas jawaban chatbot.
- [ ] Mengembangkan backend untuk integrasi aplikasi.
- [ ] Mengembangkan antarmuka web OrmawaMate.
- [ ] Mengevaluasi kemungkinan pengembangan aplikasi mobile.

## Konteks Pengembangan

Proyek ini merupakan bagian dari proses pembelajaran dan eksplorasi pengembangan solusi AI untuk mendukung akses informasi kemahasiswaan.

---

**OrmawaMate — Your Guide to Student Programs**
