# ANALISIS STATISTIK DESKRIPTIF TERHADAP IPK, JAM BELAJAR, DAN KARAKTERISTIK PADA MAHASISWA ITERA

## Deskripsi
Repositori ini berisi analisis statistik deskriptif mahasiswa ITERA terkait:  
- IPK terakhir  
- Jam belajar per minggu  
- Karakteristik demografis dan fisik (berat badan, tinggi badan, jumlah anggota keluarga)  

Analisis mencakup:  
- Ukuran pemusatan: mean, median, modus  
- Ukuran penyebaran: range, variance, standar deviasi, IQR  
- Deteksi outlier (metode IQR)  
- Visualisasi data: dot plot, histogram, boxplot, stem-and-leaf plot  
- Analisis skewness pada data fisik  

## Prasyarat
- R versi 4.0 atau lebih baru  
- RStudio (direkomendasikan)  

## Struktur Direktori
```text
code/
├─ Dataset/
│ └─ dataset.csv
├─ codeR_1_RB.Rmd
data/
├─ dataset.csv
output/
├─ 1output_semua.pdf
├─ visualisasi/
│ ├─ bar_plot.png
│ ├─ box_plot.png
│ ├─ dot_plot.png
│ ├─ histogram.png
│ ├─ skewness.png
│ ├─ stem_leaf.png
│ └─ summary_data.png
├─ perhitungan/
│ └─ perhitungan_iqr.png
poster/
├─ Poster_1_RB.pdf
README.md
```


## Dataset
Dataset berasal dari survei mahasiswa ITERA tahun 2025, berisi 458 responden dengan variabel:  
- **IPK.Terakhir..** : IPK terakhir mahasiswa  
- **BelajarJam** : Jam belajar per minggu  
- **Jumlah.Anggota.Keluarga..** : Jumlah anggota keluarga  
- **Berat.Badan..** : Berat badan (kg)  
- **Tinggi.Badan..** : Tinggi badan (cm)  

## Paket R yang Digunakan
| Paket | Fungsi Utama |
|-------|--------------|
| `ggplot2` | Visualisasi data (dot plot, histogram, boxplot) |
| `dplyr` | Manipulasi dan transformasi data |
| `readr` | Membaca file CSV |

Instalasi paket (jika belum ada):

```r
install.packages(c("ggplot2", "dplyr", "readr"))
```


Cara Menjalankan Analisis
1. Clone repositori
```bash
git clone https://github.com/sains-data/ADS_1_RB.git
cd ADS_1_RB
```

2. Buka RStudio dan set working directory
```r
setwd("path/to/ADS_1_RB")
```

3. Install paket yang diperlukan (jika belum ada)
```r
install.packages(c("ggplot2", "dplyr", "readr"))
```

4. Jalankan script utama
Buka dan jalankan file R Markdown:
```r
file.edit("code/codeR_1_RB.Rmd")
```


Lalu klik “Run All” di RStudio.
