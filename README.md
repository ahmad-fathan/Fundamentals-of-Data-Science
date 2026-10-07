# Fundamentals of Data Science

Source code contoh dan latihan untuk mata kuliah **Fundamental of Data Science**, Program Studi Sarjana Informatika, Universitas Islam Indonesia.

Seluruh kode ditulis dalam bentuk notebook Jupyter (`.ipynb`) dan mengikuti modul **Fundamen Sains Data: Pengantar Python untuk Sains Data, Probabilitas, dan Statistika**. Setiap notebook sudah dijalankan dari awal sampai akhir tanpa galat, dan outputnya (termasuk grafik) tersimpan di dalam file, sehingga dapat dibaca langsung di GitHub maupun dijalankan ulang di Google Colab.

## Isi

| Folder | Berkas | Bagian modul | Pokok bahasan |
| --- | --- | --- | --- |
| **Introduction to Data Science** | [`bab-a-python-dan-lingkungan-kerja-data-science.ipynb`](Introduction%20to%20Data%20Science/bab-a-python-dan-lingkungan-kerja-data-science.ipynb) | A | Python dalam data science, notebook Jupyter/Colab/VS Code, antarmuka Colab, runtime, sumber dataset, urutan eksekusi cell, Gemini, VS Code |
| **Introduction to Data Science** | [`bab-b-library-python-untuk-data-science.ipynb`](Introduction%20to%20Data%20Science/bab-b-library-python-untuk-data-science.ipynb) | B | Impor library, array NumPy, DataFrame pandas, grafik Matplotlib |
| **Probability and Statistics** | [`bab-c-probabilitas-dan-statistika-dengan-python.ipynb`](Probability%20and%20Statistics/bab-c-probabilitas-dan-statistika-dengan-python.ipynb) | C | Statistik deskriptif, probabilitas lewat simulasi, variabel acak diskrit (Bernoulli, binomial, PMF, CDF), variabel acak kontinu (normal, PDF), studi kasus terpadu |
| **Probability and Statistics** | [`latihan-akhir.ipynb`](Probability%20and%20Statistics/latihan-akhir.ipynb) | Latihan | Penyelesaian Latihan 1 sampai 4 beserta interpretasinya |

Setiap notebook memuat penjelasan teori, kode contoh, **hasil yang diharapkan**, dan interpretasi — mengikuti struktur modul. Notebook latihan memuat penyelesaian sebagai acuan; mahasiswa dianjurkan mengerjakan sendiri terlebih dahulu.

## Struktur folder

```
.
├── README.md
├── requirements.txt
├── Introduction to Data Science/
│   ├── bab-a-python-dan-lingkungan-kerja-data-science.ipynb
│   └── bab-b-library-python-untuk-data-science.ipynb
└── Probability and Statistics/
    ├── bab-c-probabilitas-dan-statistika-dengan-python.ipynb
    └── latihan-akhir.ipynb
```

Setiap notebook diberi nama dengan pola `bab-<huruf>-<judul-bab-dalam-huruf-kecil>.ipynb` dan ditempatkan pada folder sesuai topiknya. Bab baru cukup ditambahkan ke folder yang sesuai, atau dibuat folder topik baru sejajar dengan yang sudah ada.

## Menjalankan

### Google Colab

Buka <https://colab.research.google.com>, pilih **File > Upload notebook**, lalu unggah file `.ipynb`. Library NumPy, pandas, Matplotlib, dan SciPy sudah tersedia. Jalankan **Runtime > Restart session and run all** untuk memastikan seluruh cell berjalan tanpa galat.

### Lokal (Jupyter / VS Code)

```bash
python3 -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook                # atau buka folder ini di VS Code
```

Butuh Python 3.9 atau lebih baru.

## Catatan

- Cell yang hanya berjalan di Google Colab (`google.colab`, `kagglehub`) dibungkus `try/except`, sehingga notebook tetap berjalan tanpa galat di Jupyter maupun VS Code.
- Hasil simulasi memakai `np.random.default_rng(42)` agar dapat diulang. Angka hasil simulasi dan digit terakhir hasil pembulatan dapat berbeda antar versi NumPy/SciPy; interpretasi tidak berubah.
- Sumber dataset contoh: [seaborn-data](https://github.com/mwaskom/seaborn-data).

## Penggunaan

Disediakan untuk keperluan pembelajaran. Mahasiswa dipersilahkan membaca, menjalankan, dan mengubahnya untuk keperluan belajar.

---

**Ahmad Fathan Hidayatullah** — Program Studi Sarjana Informatika, Universitas Islam Indonesia
