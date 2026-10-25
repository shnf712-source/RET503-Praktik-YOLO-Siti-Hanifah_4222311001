# Praktik Terpadu RET503 — Minggu 4–7

**Nama:** Siti Hanifah  
**NIM:** 4222311001
**Model:** YOLOv8n  
**Dataset:** COCO subset — person, car, bottle

## Eksperimen

| Eksperimen | Konfigurasi | mAP50 | mAP50-95 |
|---|---|---:|---:|
| E1 — Pretrained | imgsz=416 | 0.305 | 0.167 |
| E2 — Scratch | imgsz=416 | 0.011 | 0.002 |
| E3 — Tuning | imgsz=640 | 0.429 | 0.246 |

## Evaluasi Test

Model terpilih: E3 — Tuning  
mAP50: 0.592  
mAP50-95: 0.394

## Kesimpulan

Pada eksperimen ini, E3 dengan ukuran gambar 640 menghasilkan mAP50-95 validasi tertinggi. E2 yang dilatih dari awal menghasilkan nilai lebih rendah dibanding model pretrained pada dataset dan pengaturan yang digunakan.

## File

- `00_ambil_subset_coco.py` — mengambil subset dataset.
- `01_cek_anotasi.py` — memeriksa anotasi.
- `02_yolo_ke_coco.py` — konversi anotasi YOLO ke COCO.
- `03_coco_ke_yolo.py` — konversi anotasi COCO ke YOLO.
- `05_split_dataset_yolo.py` — membagi dataset.
- `06_latih_bandingkan.py` — menjalankan eksperimen dan evaluasi.
- `hasil_praktik_4222311007.txt` — laporan eksperimen.
- `hasil_praktik_4222311007.csv` — tabel hasil eksperimen.

Catatan: file gambar dataset dan bobot model tidak disertakan dalam repositori ini.
