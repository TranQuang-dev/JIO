# Jio Farm Action

Automasi farm link aktivasi Jio Gemini via GitHub Actions.

## Quick Start

1. Fork repo ini ke akun tumbal Anda
2. Edit workflow di `.github/workflows/farm.yml`
3. Tekan "Run workflow" → isi `target_links: 1`
4. Hasil ada di Artifacts
5. Refresh sampai mendapat link

## Hasil

- `fresh_links.txt` - link aktivasi valid
- `farm_results.csv` - log detail per percobaan
- `farm.log` - log eksekusi lengkap

## Konfigurasi

| Parameter | Deskripsi | Default |
|-----------|-----------|---------|
| target_links | Jumlah link baru | 1 |
| max_runtime_minutes | Batas waktu eksekusi | 30 |

## Catatan

Script ini menggunakan panel Firebase publik untuk intercept OTP. Hasil tidak guaranteed karena tergantung availability panel dan device yang aktif.