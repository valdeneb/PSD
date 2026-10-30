# Analisis Pendapatan Transaksi POS 2024–2025

Notebook Python untuk menghitung total pendapatan per tahun dari data transaksi POS.

## File
- `analisis_pendapatan_pos.ipynb` – notebook utama (sudah berisi output)
- `paket_a_transaksi_pos_2024_2025.csv` – dataset
- `hasil_pendapatan_per_tahun.csv` – hasil akhir
- `grafik_pendapatan_per_tahun.png` – grafik hasil

## Metode singkat
1. Hapus 30 baris duplikat persis.
2. Isi `kode_kasir` kosong dengan `TIDAK_DIKETAHUI` (tidak memengaruhi pendapatan).
3. Seragamkan format tanggal (3 format) dan harga (`13.500`, `7500,00`).
4. Buang `jumlah` negatif atau > 12 (salah input).
5. Hanya status `SELESAI` yang dihitung (`BATAL` dan `RETUR` tidak).
6. Pendapatan = jumlah × harga × (1 − diskon/100).

## Hasil (pendapatan bersih)
| Tahun | Pendapatan |
|-------|-----------|
| 2024 | Rp 127.406.475 |
| 2025 | Rp 135.001.100 |

## Menjalankan
```bash
pip install pandas matplotlib jupyter
jupyter notebook analisis_pendapatan_pos.ipynb
```
