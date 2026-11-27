# Klasifikasi Ganjil-Genap Kendaraan dari Plat Nomor

Final project mata kuliah Pengolahan Citra Digital, Kelompok 7.

Anggota: 
Naura Alifa Damayanti
Andi Nabil Safaraz 
Muhammad Iqbal Hilmi 
Dania Hafiza  
Jundan Saiful Haq

Sistem ini mencari semua plat nomor pada foto jalan raya, lalu menentukan label ganjil atau genap dari digit terakhir setiap plat. Semua tahap menggunakan pengolahan citra konvensional, tanpa deep learning: enhancement, lokalisasi ROI (Sobel, Canny, morfologi), segmentasi karakter (Otsu, CCL), fitur HOG/LBP, dan classifier KNN/SVM/XGBoost.

## Dataset

Dataset **tidak disimpan di repo ini**. Unduh dari Kaggle: [juanthomaswijaya/indonesian-license-plate-dataset](https://www.kaggle.com/datasets/juanthomaswijaya/indonesian-license-plate-dataset). Dataset ini berisi dua folder:

- `Indonesian License Plate Dataset`: foto jalan raya dengan label bbox dan teks per plat.
- `Indonesian License Plate Recognition Dataset`: crop plat dengan bbox per karakter.

## Cara menjalankan

1. Buka `notebooks/pcd-kelompok7-ganjil-genap.ipynb` di Kaggle (*File → Import Notebook*).
2. *Add Input* → cari dataset di atas.
3. *Run All*. Path dataset dicari otomatis, dan hasil CSV tersimpan di `/kaggle/working`.

## Struktur repo

```
notebooks/   notebook utama (tanpa output)
results/     notebook hasil run dan file CSV
laporan/     naskah laporan format IEEE
proposal/    proposal
```
