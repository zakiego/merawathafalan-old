# merawathafalan

Melatih hafalan Al-Qur'an agar semakin kuat. Disertai dengan profil dan riwayat yang bisa dibagikan ke publik.

## Prinsip

Project ini dibangun dengan mengedepankan prinsip _mobile-first_.

## Fitur

- [x] Tebak sambung ayat
- [ ] Tebak ayat sebelumnya
- [ ] Tebak surah
- [ ] Tebak juz
- [ ] Grafik history total per ayat

## API

### Base

```http
https://zakiego.vercel.app/api/quran/v2
```

### Endpoint path

```http
GET /sambung-ayat?amount=10&mode=juz&encrypt=false&start=1&end=5
```

| Parameter | Type       | Default | Description                           | ‎            |
| :-------- | :--------- | :------ | :------------------------------------ | :----------- |
| `amount`  | `integer`  | 1       | jumlah soal                           | **optional** |
| `mode`    | `boolean ` | surah   | surah/juz                             | **optional** |
| `encrypt` | `boolean`  | false   | enkripsi                              | **optional** |
| `start`   | `integer`  | 1       | **dari** surah (1-114) / juz (1-30)   | **optional** |
| `end`     | `integer`  | 1       | **sampai** surah (1-114) / juz (1-30) | **optional** |

```http
GET /sambung-ayat:custom?amount=10&mode=juz&encrypt=false&select=1,2,3
```

| Parameter | Type       | Default | Description            | ‎            |
| :-------- | :--------- | :------ | :--------------------- | :----------- |
| `amount`  | `integer`  | 1       | jumlah soal            | **optional** |
| `mode`    | `boolean ` | surah   | surah/juz              | **optional** |
| `encrypt` | `boolean`  | false   | enkripsi               | **optional** |
| `select`  | `integer`  | 1       | surah/juz yang dipilih | **optional** |

## Made with

- [NextJS](https://nextjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Supabase](https://supabase.io/)
- [Vercel](https://vercel.com/)
