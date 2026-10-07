# Website Latihan Webdev Abinara-1

Repo ini dipakai untuk latihan Git dan GitHub divisi Webdev. Setiap Pull Request yang di-merge langsung tampil di website latihan.

## Aturan

1. Jangan push langsung ke `main`. Semua perubahan lewat Pull Request.
2. Satu orang, satu branch. Nama branch: `anggota/nama-kamu`.
3. Hanya ubah slot milikmu sendiri di `index.html`.
4. Push ditolak? Jalankan `git pull origin main` dulu. Jangan pakai `--force`.

## Latihan 1: isi slot kamu

```bash
git clone git@github.com:DocHudson45/website-latihan.git
cd website-latihan
git switch -c anggota/nama-kamu
```

Buka `index.html`, cari slot dengan nomor milikmu, lalu ganti isinya:

```html
<article class="card">
  <h3>Nama Kamu</h3>
  <p>Satu fakta tentang dirimu.</p>
</article>
```

Simpan, cek di browser, lalu:

```bash
git add index.html
git commit -m "Isi slot 3 dengan profil Nama Kamu"
git push -u origin anggota/nama-kamu
```

Buka repo ini di GitHub, klik **Compare & pull request**, lalu **Create pull request**.

## Latihan 2: konflik

Latihan ini dikerjakan berpasangan dan sengaja dibuat bentrok.

1. Masing-masing buat branch baru dari `main` terbaru: `git switch main`, `git pull`, lalu `git switch -c konflik/nama-kamu`.
2. Ubah kalimat di **ZONA KONFLIK** (`<p class="tagline">`) dengan versi kalian sendiri.
3. Commit, push, dan buka PR.
4. PR pertama di-merge. PR kedua akan ditandai konflik.
5. Pemilik PR kedua menjalankan `git pull origin main`, memilih atau menggabungkan kedua versi, lalu commit dan push lagi.
