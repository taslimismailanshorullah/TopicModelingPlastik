# Efek Domino Konflik Geopolitik Iran pada Diskursus Industri Plastik Indonesia

Repositori ini berisi data, kode, dan analisis mengenai dampak guncangan geopolitik terhadap industri plastik lokal, diukur dari narasi media online di Indonesia menggunakan pendekatan *Topic Modeling*.

## 📌 Latar Belakang & Objektif
Konflik geopolitik memicu guncangan pada rantai pasok komoditas global yang berdampak pada industri plastik di Indonesia. Proyek ini bertujuan untuk mengidentifikasi dan memetakan wacana serta pola *framing* media online nasional dalam merepresentasikan krisis ini menggunakan metode *Natural Language Processing* (NLP).

## 🛠️ Metodologi & Tools
- **Sumber Data:** 142 artikel berita (hasil *regex filtering* dari 1.541 artikel mentah) dari portal nasional (Kompas.com, CNN Indonesia, Bisnis.com, VIVA.co.id).
- **Pendekatan:** *Neural Topic Modeling* dengan **BERTopic**.
- **Pipeline:**
  - **Embedding:** IndoBERT (`indobenchmark/indobert-base-p1`)
  - **Dimensionality Reduction:** UMAP
  - **Clustering:** HDBSCAN
  - **Topic Representation:** c-TF-IDF

## 📊 Temuan Utama
Model berhasil mengidentifikasi 9 topik wacana utama tanpa *outlier* (0,0%). Tiga pola makro *framing* media yang ditemukan:
1. **Dominasi Ekonomi Mikro (>54%):** Pemberitaan sangat fokus pada viktimisasi UMKM dan pedagang kecil.
2. **Kesenjangan Geopolitik:** Media domestik kurang mengelaborasi koneksi kausal dari krisis global ke ranah lokal.
3. **Momentum Diskursus Alternatif (~41%):** Momentum krisis dimanfaatkan untuk mempromosikan narasi kesehatan, daur ulang industri, dan gaya hidup ramah lingkungan.

*(TIPS UNTUK TASLIM: Jika kamu sudah drag-and-drop gambar grafik ke GitHub, letakkan kode gambarnya di baris ini)*

## 📂 Struktur Repositori
- `berita_plastik (1).csv` : Dataset mentah hasil ekstraksi berita.
- `topic_modeling_plastik_compiled.ipynb` : *Source code* lengkap (Python/Jupyter Notebook) untuk pemrosesan teks, pemodelan BERTopic, dan visualisasi.
- `Efek Domino Konflik Geopolitik Iran pada Diskursus Industri Plastik Indonesia.pdf` : Laporan komprehensif penelitian.

---
*Dibuat untuk keperluan portofolio Data Science.*
