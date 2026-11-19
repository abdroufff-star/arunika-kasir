# ARUNIKA — Aplikasi Kasir & Order Percetakan (PWA + Firebase)

Paket ini berisi seluruh file yang siap langsung diunggah ke repositori GitHub dan di-deploy melalui Vercel.

## Daftar File
- `index.html` — Aplikasi utama ARUNIKA (responsif PC & HP, Firebase Auth Google + Cloud Firestore).
- `manifest.json` — Konfigurasi PWA agar bisa di-install sebagai aplikasi di PC (Edge/Chrome) dan HP.
- `sw.js` — Service Worker resmi untuk dukungan PWA penuh.
- `icon.svg` — Ikon aplikasi ARUNIKA resolusi tinggi.
- `vercel.json` — Pengaturan header optimal untuk Vercel.

## Langkah Upload & Aktivasi
1. Ekstrak seluruh isi file `.zip` ini.
2. (Opsional) Buka `index.html`, cari `DEFAULT_FIREBASE_CONFIG`, lalu ganti nilai `PASTE_..._ANDA` dengan `firebaseConfig` milik Anda. Anda juga bisa mengisinya nanti langsung dari tombol **"Atur Konfigurasi Firebase"** di layar login.
3. Buka repositori GitHub Anda → klik **Add file → Upload files** → seret semua file hasil ekstrak (`index.html`, `manifest.json`, `sw.js`, `icon.svg`, `vercel.json`, `README.md`) → klik **Commit changes**.
4. Tunggu Vercel selesai melakukan deploy otomatis (status **Ready**).
5. Di **Firebase Console**:
   - **Authentication → Sign-in method**: Aktifkan **Google**.
   - **Authentication → Settings → Authorized domains**: Tambahkan domain Vercel Anda (misal `arunika-kasir.vercel.app`).
   - **Firestore Database**: Pastikan database sudah aktif (lokasi `asia-southeast2` / Jakarta).
6. Buka link Vercel Anda, tekan `Ctrl + F5`, lalu klik **Masuk dengan Google**.
