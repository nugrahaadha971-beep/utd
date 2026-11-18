# UTD Reagent Audit – Clinical Command Center

Aplikasi web satu file untuk audit stok reagen, tanggal expired (FEFO), dan sisa tes alat HISCL 800 di Unit Transfusi Darah. Tanpa server dan tanpa build; semua data tersimpan di `localStorage` browser masing-masing perangkat.

## Deploy ke GitHub Pages

1. Buat repository baru di GitHub (mis. `utd-reagent-audit`) dan unggah seluruh isi folder ini.
2. Buka **Settings → Pages → Build and deployment → Source**, pilih **GitHub Actions**.
3. Push ke branch `main`. Workflow `.github/workflows/pages.yml` akan men-deploy otomatis.
4. Situs aktif di `https://<username>.github.io/<nama-repo>/`.

Alternatif tanpa Actions: pada Settings → Pages pilih **Deploy from a branch** → `main` / `(root)`, lalu hapus folder `.github`.

## Catatan penting

- Data **tidak** tersinkron antar perangkat. Gunakan tombol **Salin JSON** dan **Impor** untuk memindahkan data.
- Situs GitHub Pages bersifat publik. Jangan memasukkan data pasien atau data rahasia ke dalam aplikasi ini.
- Hapus data browser akan menghapus stok yang tersimpan, jadi cadangkan JSON secara berkala.
