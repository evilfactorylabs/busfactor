# busfactor

tujuan dibuatnya repositori ini adalah untuk menghindari SPOF khususnya ketika salah satu 'angota inti'
dari evilfactorylabs meninggal spesifiknya adalah si faultable. jadi, evilfactorylabs masih bisa berjalan
sekalipun salah satu anggotanya—khususnya BDFL—meninggal.

alamat email utama yang digunakan oleh evilfactorylabs adalah `hello@evilfactory.id`.

## PIC

ada 3 anggota inti yang bertanggung jawab atas semua apa yang terjadi di evilfactorylabs:

- @faultable, fariz@evilfactory.id
- @ri7nz, ri7nz@evilfactory.id
- @kevanantha, kevanantha@evilfactory.id

segala informasi yang bersifat 'rahasia' ada di 3 orang diatas. PIC hanya boleh 3 orang, no matter what.

## Vault

penyimpanan rahasia utama untuk semua kredensial (email+password, gpg public/secret key, etc) evilfactorylabs
berada di *instance* Bitwarden @faultable yang bisa diakses di https://bw.evilfactory.id.

untuk alamat email, silahkan gunakan email utama yang kata sandi utama (shared) nya sudah
dikirim ke @ri7nz dan @kevanantha.

## PGP Public Key

alamat email inti yang digunakan oleh evilfactorylabs adalah `hello@evilfactory.id` dengan sidik jari
`7D1FCE5D2A1675283B4AD0BC9826691987479B5D`, silahkan ambil *backup* dari public dan secret key tersebut di vault.

## Email

semua alamat yang berada di `@evilfactory.id` menggunakan layanan dari Migadu. untuk akun administrator di Migadu,
seperti biasa menggunakan alamat email `hello@evilfactory.id`

## Server

ada 2 server saat ini yang dikelola oleh evilfactorylabs, dan semua berada di Linode. Untuk melakukan SSH, kunci
public nya (ECDSA) ada di vault dan memiliki nama pengguna `evil` dengan grup wheel/sudo.

yang masing-masing memiliki alamat IP:

- public: 192.46.229.118, private: 100.106.52.26 (dita)
- public: 192.46.225.58, private: 100.87.234.49 (resly)

yang mana hanya bisa diakses (SSH) melalui jaringan Tailscale yang kredensialnya sudah ada di vault. jika dalam suatu
kondisi tidak bisa membuat koneksi SSH, bisa akses via LISH yang kredensial terkait Linode sudah ada di vault juga.

## Domain

ada 3 alamat domain yang dikelola oleh evilfactorylabs:

- evilfactory.id, utama
- evilfactorylabs.org, untuk landing page
- evlfctry.pro, pemendek tautan
- edgy.network, payung untuk projek-projek terkait infra

yang mana didaftarkan melalui registry Namecheap. khusus untuk evilfactory.id, registry yang digunakan
adalah Cloudkilat. Untuk terkait DNS, bisa cek repository [faultable/dns](https://github.com/faultable/dns)

## Internet accounts

setiap akun yang ada di internet yang me-representasikan evilfactorylabs, selalu menggunakan alamat
email `social@evilfactory.id` yang tidak memiliki kunci publik dan pribadi PGP. Akun-akun tersebut antara lain (A-Z):

- Twitter
- Discord
- repl.it
- GitHub
- Netlify
- Revue
- Saweria
- Trakteer
- Xendit
- Zapier

Yang menggunakan nama pengguna `@evilfactorylabs`.

## Changelog

- 14 februari 2021, membuat rancangan dokumen pertama. mungkin ini bisa disimpan di Handbook
- 14 maret 2021, nambahin dns dan ganti IP privat
