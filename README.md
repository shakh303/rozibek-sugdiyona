# Ro'zibek & Sug'diyona — To'y taklifnomasi

Bir sahifali to'y taklifnomasi sayti. 19-sentabr, 2026-yil.

## Tuzilma

```
index.html                 # butun sayt (HTML + CSS + JS bitta faylda)
assets/audio/music.mp3     # fon musiqasi (tugma bosilganda boshlanadi)
assets/images/             # kelin-kuyov surati shu yerga qo'shiladi
.nojekyll                  # GitHub Pages uchun kerak
```

## Dizayn

O'zbek suzani gul naqshlariga asoslangan uslub — lola (tulpan) shoxchasi asosiy
bezak sifatida takrorlanadi (SVG, `#sprig-shape`). Rang: zaytun-yashil fon,
antik oltin chiziqlar, terrakota urg'u. Shriftlar: Cinzel (sarlavhalar),
Cormorant Garamond (matn), Pinyon Script (ismlar).

## Nimalarni o'zgartirish mumkin

Hammasi `index.html` ichida. Qidiring va almashtiring:

| Nima | Qayerda |
|---|---|
| Ismlar | `Ro'zibek<span class="amp">va</span>Sug'diyona` — 4 joyda (cover, hero, closing) |
| Sana matni | `19-sentabr, 2026-yil` va `19 · 09 · 2026` |
| Vaqt | **DIQQAT — hali tasdiqlanmagan taxminiy qiymat**: «Vaqt» kartasidagi `18:00` |
| Manzil | «Manzil» kartasidagi `Muratali qishlog'i` / `«Risolat ona» to'yxonasi` |
| Xarita havolasi | `<a href="...` — Google Maps havolasi allaqachon qo'yilgan |
| Orqaga hisoblagich | JS ichidagi `new Date('2026-09-19T18:00:00+05:00')` — vaqt aniqlangach shu yerni ham yangilang |
| Rang | CSS boshidagi `--gold:#C9A24B`, `--ground:#1F3A2E` |
| Kelin-kuyov surati | `assets/images/couple.jpg` — Hero bo'limidagi arka-ramkada ko'rinadi |
| Musiqa | `assets/audio/music.mp3` faylini almashtiring (nomi o'zgarmasin) |
| Musiqa balandligi | JS ichidagi `var VOL = .65` |

> Musiqa «Taklifnomani ochish» tugmasi bosilganda boshlanadi — brauzerlar sahifa
> ochilishi bilan avtomatik ovoz chiqarishga ruxsat bermaydi. O'ng pastdagi
> dumaloq tugma orqali mehmon ovozni o'chira oladi.

## GitHub Pages'ga joylash

1. GitHub'da yangi **public** repo yarating.
2. Shu papkadagi barcha fayllarni yuklang:

```bash
git init
git add .
git commit -m "To'y taklifnomasi"
git branch -M main
git remote add origin https://github.com/FOYDALANUVCHI/rozibek-sugdiyona.git
git push -u origin main
```

3. Repo → **Settings → Pages** → Source: `Deploy from a branch`, Branch: `main`, papka: `/ (root)` → Save.
4. Bir necha daqiqadan so'ng sayt `https://FOYDALANUVCHI.github.io/rozibek-sugdiyona/` manzilida ochiladi.
