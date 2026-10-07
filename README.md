# Fundamentals of Data Science

Source code contoh dan latihan untuk mata kuliah **Fundamental of Data Science**, Program Studi Sarjana Informatika, Universitas Islam Indonesia.

Seluruh kode ditulis dalam bentuk notebook Jupyter (`.ipynb`) dan mengikuti modul **Fundamen Sains Data: Pengantar Python untuk Sains Data, Probabilitas, dan Statistika**. Setiap notebook sudah dijalankan dari awal sampai akhir tanpa galat, dan outputnya (termasuk grafik) tersimpan di dalam file, sehingga dapat dibaca langsung di GitHub maupun dijalankan ulang di Google Colab.

## Isi

| Berkas | Bagian modul | Pokok bahasan |
| --- | --- | --- |
| [`bab-a-python-dan-lingkungan-kerja-data-science.ipynb`](modul-01-fundamen-sains-data/bab-a-python-dan-lingkungan-kerja-data-science.ipynb) | A | Python dalam data science, notebook Jupyter/Colab/VS Code, antarmuka Colab, runtime, sumber dataset, urutan eksekusi cell, Gemini, VS Code |
| [`bab-b-library-python-untuk-data-science.ipynb`](modul-01-fundamen-sains-data/bab-b-library-python-untuk-data-science.ipynb) | B | Impor library, array NumPy, DataFrame pandas, grafik Matplotlib |
| [`bab-c-probabilitas-dan-statistika-dengan-python.ipynb`](modul-01-fundamen-sains-data/bab-c-probabilitas-dan-statistika-dengan-python.ipynb) | C | Statistik deskriptif, probabilitas lewat simulasi, variabel acak diskrit (Bernoulli, binomial, PMF, CDF), variabel acak kontinu (normal, PDF), studi kasus terpadu |
| [`latihan/latihan-akhir.ipynb`](modul-01-fundamen-sains-data/latihan/latihan-akhir.ipynb) | Latihan | Penyelesaian Latihan 1 sampai 4 beserta interpretasinya |

Setiap notebook memuat penjelasan teori, kode contoh, **hasil yang diharapkan**, dan interpretasi — mengikuti struktur modul. Notebook latihan memuat penyelesaian sebagai acuan; mahasiswa dianjurkan mengerjakan sendiri terlebih dahulu.

## Struktur folder

```
.
├── README.md
├── requirements.txt
└── modul-01-fundamen-sains-data/
    ├── bab-a-python-dan-lingkungan-kerja-data-science.ipynb
    ├── bab-b-library-python-untuk-data-science.ipynb
    ├── bab-c-probabilitas-dan-statistika-dengan-python.ipynb
    └── latihan/
        └── latihan-akhir.ipynb
```

Modul berikutnya cukup ditambah sebagai folder sejajar, misalnya `modul-02-.../`, dengan pola nama `bab-<huruf>-<judul-bab-dalam-huruf-kecil>.ipynb`.

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
