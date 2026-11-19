# Auto Transfer & Vend / Restock - Growlauncher (Boren Store)

Script otomatisasi transfer item, auto vend buy-drop, dan restock vending machine untuk Growlauncher Android & PC.

## Fitur Utama

1. **Mode 1: Transfer Murni (Move Items)**:
   - Mengambil floating item (block / seed) berdasarkan `Item ID` di **Input World**.
   - Otomatis berpindah dan meletakkan (drop) item di **Output World** secara teratur dan aman.

2. **Mode 2: Auto Vend (Beli & Drop)**:
   - Memindai vending machine di **Input World**.
   - **Anti-Scam Protection**: Verifikasi ID item dan harga sebelum membeli.
   - **Toggle Per Item**:
     - `Per Item` ON: Harga dihitung **X World Lock / 1 item** (contoh: 1 WL/item, 2 WL/item). Membeli jika harga <= `Item Buy Price`.
     - `Per Item` OFF: Rate dihitung **X item / 1 World Lock** (contoh: 200/WL, 100/WL). Membeli jika rate >= `Item Buy Price`.
   - Membawa item yang dibeli dan meletakkannya (drop) di **Output World**.

3. **Mode 3: Auto Restock Toko (Isi Vend Hingga 5k)**:
   - Mengambil persediaan block / seed dari storage di **Input World**.
   - Mengisi vending machine di **Output World** hingga kapasitas maksimal **5.000 (5k) item** per vend.
   - Otomatis menandai dan melewati vend yang sudah penuh (5k) agar langsung melanjutkan ke vend berikutnya.

4. **Toggle Alur Vertikal & Horizontal**:
   - `Vertical` ON: Memindai dan meletakkan drop/restock secara vertikal (kolom per kolom: atas ke bawah sumbu y, lalu pindah ke kolom x berikutnya).
   - `Vertical` OFF: Memindai dan meletakkan secara horizontal (baris per baris: kiri ke kanan sumbu x, lalu pindah ke baris y berikutnya).

5. **Dual Interface**:
   - Standalone Dear ImGui Window dengan kontrol presisi (`[-]` / `[+]` counter, text input, status log visual).
   - Native Growlauncher 5-Tab Menu (`/transfer`).

## Cara Menggunakan
Jalankan `loader_transfer.lua` di Growlauncher untuk selalu mendapatkan versi terbaru secara otomatis langsung dari GitHub.
