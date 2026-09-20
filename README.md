# Pinterest hosting — salin folder ini APA ADANYA ke root repo GitHub publik

Struktur wajib (dibaca `make-pin-csv.py --media`):
    <repo>/001/PIN-01.png … PIN-12.png, PIN-V1.mp4, PIN-V2.mp4   (14 file/produk)
    <repo>/002/…  <repo>/003/…  <repo>/004/…  <repo>/005/… (menyusul)

URL media = https://raw.githubusercontent.com/<user>/<repo>/main/<id>/PIN-NN.png
Setelah push: `curl -sI <url> | head -1` harus HTTP 200 → jalankan
    python3 Listing/_build/make-pin-csv.py 001 --start YYYY-MM-DD --link <Share & Save listing> --media https://raw.githubusercontent.com/<user>/<repo>/main/001
Jangan mengganti nama file; jangan pakai branch selain main (atau sebutkan branch-nya).

Facebook (20 Sep 2026): folder `fb/<id>/` (C1–C5.png, Q1–Q3.png, REEL-A/B.mp4) = media URL untuk Bulk upload Meta Business Suite
(`Produk-Plans/05-JADWAL-FACEBOOK.csv` kolom media_url). Push setiap kali listing baru tayang.
