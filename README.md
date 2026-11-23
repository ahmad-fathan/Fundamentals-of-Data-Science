# Fundamentals of Data Science

Notebook Jupyter untuk mata kuliah **Fundamentals of Data Science**, Program Studi Sarjana Informatika, Universitas Islam Indonesia.

## Isi

| Folder | Notebook | Topik |
| --- | --- | --- |
| Introduction to Data Science | `bab-a-python-dan-lingkungan-kerja-data-science.ipynb` | Python, Jupyter/Colab, sumber dataset |
| Introduction to Data Science | `bab-b-library-python-untuk-data-science.ipynb` | NumPy, pandas, Matplotlib |
| Probability and Statistics | `bab-c-probabilitas-dan-statistika-dengan-python.ipynb` | Statistik deskriptif, probabilitas, distribusi |
| Probability and Statistics | `latihan-akhir.ipynb` | Penyelesaian Latihan 1–4 |
| Introduction to Machine Learning | `bab-d-regresi-linier-dengan-python.ipynb` | Regresi linier, metrik evaluasi, gradient descent |
| Introduction to Machine Learning | `latihan-akhir.ipynb` | Penyelesaian Latihan 1–5 (`diabetes`) |
| Classification | `bab-e1-naive-bayes-data-tabular.ipynb` | Naïve Bayes data tabular |
| Classification | `bab-e2-naive-bayes-data-teks.ipynb` | Naïve Bayes data teks (SMS spam) |

Semua notebook sudah dijalankan lengkap dengan output tersimpan.

## Menjalankan

**Colab:** unggah `.ipynb` ke <https://colab.research.google.com>, lalu *Runtime > Restart session and run all*.

**Lokal:**

```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Butuh Python 3.9+.
