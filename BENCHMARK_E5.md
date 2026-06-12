# Benchmark: Multilingual E5 Base

> Model: intfloat/multilingual-e5-base
> Dimensi Vektor: 768
> Bahasa: Multi-bahasa
> Framework: sentence-transformers
> Vector Database: Qdrant

---

## Konfigurasi Eksperimen

| Parameter | Nilai |
|:---|:---|
| Model Embedding | intfloat/multilingual-e5-base |
| Dimensi Vektor | 768 |
| Ukuran Chunk | 1000 |
| Overlap Chunk | 200 |
| Metode Chunking | Hybrid |
| Vector Database | Qdrant |
| Collection | scientific_articles |

---

## Hasil Ingestion

| Jurnal | DOI | Chunks Disimpan |
|:---|:---|:---:|
| Digital learning outcomes and sustainable learning in higher education | 10.1016/j.actpsy.2026.107152 | 71 |

---

## Kelebihan

- Mendukung banyak bahasa
- Cocok untuk retrieval lintas bahasa
- Dimensi lebih ringan dibanding BGE-M3
- Cocok untuk RAG dan Qdrant

## Kekurangan

- Dimensi lebih kecil dibanding BGE-M3
- Performa bergantung pada kualitas chunking

## Kesimpulan

Model intfloat/multilingual-e5-base berhasil digunakan untuk proses ingestion jurnal ke Qdrant. Model menghasilkan embedding berdimensi 768 dan mendukung retrieval multi-bahasa sehingga cocok digunakan pada sistem RAG yang menerima query Bahasa Indonesia maupun Bahasa Inggris.