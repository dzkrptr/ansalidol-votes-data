# ansalidol-votes-data

Data hasil voting **ANSAL IDOL 2026** (RSUD dr. H. Moch. Ansari Saleh).

- `votes.json` — hasil hitung suara per finalis, **diupdate otomatis tiap menit** oleh Google Apps Script (`publishVotes()`).
- Halaman hasil voting membaca berkas ini lewat `raw.githubusercontent.com` (CORS `*`, gratis, tahan ribuan pembaca).

Format `votes.json`:
```json
{
  "total": 0,
  "votes": { "nama depan lowercased": jumlah },
  "finalis": [ "Nama Finalis (Unit)" ],
  "updatedAt": "ISO timestamp"
}
```

> File ini publik agar bisa dibaca browser pengguna. Token/rahasia **tidak** disimpan di sini.