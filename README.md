# BEM FST UNAIR Link Hub

Website statis sederhana yang berfungsi sebagai pusat tautan penting untuk **BEM FST Universitas Airlangga**. Halaman ini dirancang agar pengunjung bisa mengakses berbagai platform dan formulir dengan cepat melalui tampilan yang ringkas, responsif, dan modern.

## Fitur

- Tampilan link hub yang sederhana dan mudah dipahami
- Desain modern dengan nuansa gelap dan aksen emas
- Responsif untuk desktop maupun mobile
- Animasi ringan pada elemen halaman
- Struktur proyek sangat ringan karena hanya menggunakan HTML dan CSS

## Struktur Proyek

```text
.
|-- index.html
|-- style.css
`-- README.md
```

## Teknologi yang Digunakan

- HTML5
- CSS3
- Google Fonts (`Space Grotesk` dan `DM Sans`)

## Cara Menjalankan

Karena proyek ini adalah website statis, kamu tidak memerlukan proses build atau instalasi dependency.

1. Clone atau download repository ini.
2. Buka file `index.html` langsung di browser.

Alternatif lain, jika ingin menjalankan lewat local server, kamu bisa memakai ekstensi seperti **Live Server** di VS Code.

## Cara Kustomisasi

### Mengubah Judul dan Deskripsi

Edit bagian berikut di file `index.html`:

- Judul halaman pada tag `<title>`
- Judul utama pada elemen dengan class `.hub__title`
- Subjudul pada elemen dengan class `.hub__subtitle`

### Mengubah Daftar Link

Setiap kartu tautan berada di dalam elemen:

```html
<li class="hub__link-item">
  <a class="hub__link" href="https://example.com" target="_blank" rel="noopener noreferrer">
    <span class="hub__link-content">
      <span class="hub__link-title">Judul Link</span>
      <span class="hub__link-desc">Deskripsi singkat link</span>
    </span>
    <span class="hub__link-arrow" aria-hidden="true">&rarr;</span>
  </a>
</li>
```

Untuk menambah link baru, cukup duplikasi blok di atas lalu sesuaikan:

- `href` untuk alamat tujuan
- `.hub__link-title` untuk nama link
- `.hub__link-desc` untuk deskripsi singkat

### Mengubah Warna dan Gaya

Warna utama proyek berada di bagian `:root` dalam file `style.css`, contohnya:

- `--c-bg`
- `--c-surface`
- `--c-text`
- `--c-accent`

Kamu bisa mengganti variabel tersebut untuk menyesuaikan identitas visual organisasi atau acara.

## Kelebihan Proyek Ini

- Mudah diedit bahkan untuk pemula
- Cocok dipakai sebagai bio link organisasi, event, atau komunitas
- Tidak bergantung pada framework sehingga ringan dan cepat dibuka

## Pengembangan Selanjutnya

Beberapa ide pengembangan jika ingin proyek ini ditingkatkan:

- Menambahkan ikon untuk setiap tautan
- Menambahkan tombol copy link atau share
- Menyimpan data link dalam file JSON agar lebih mudah dikelola
- Menambahkan mode tema terang/gelap
- Menyediakan section kontak atau sosial media tambahan

## Lisensi

Proyek ini dapat digunakan dan dimodifikasi sesuai kebutuhan internal organisasi atau pengembangan pribadi.
