# 📝 Vodič za dodavanje sadržaja

Ovaj vodič pokazuje gdje točno trebate dodati svoj sadržaj na svakoj stranici.

## 🎨 Dodavanje logotipa (opciono)

Trenutno stranica koristi placeholder logo (ljubičasti kvadrat sa slovom "F").

### Kako zamijeniti sa pravim logom:

**Opcija 1: PNG/SVG datoteka**

1. Dodajte vašu logo datoteku u `public/` folder (npr. `public/logo.png` ili `public/logo.svg`)

2. U datoteci `src/layouts/Layout.astro`, pronađite:

**Linija ~74-78** (navigacija):
```html
<!-- Zamijenite: -->
<div class="w-10 h-10 md:w-12 md:h-12 bg-gradient-to-br from-flexio to-purple-700 rounded-xl flex items-center justify-center shadow-md group-hover:shadow-lg transition-all">
  <span class="text-white font-bold text-lg md:text-xl">F</span>
</div>

<!-- Sa: -->
<img 
  src="/logo.png" 
  alt="Flexio Logo" 
  class="w-10 h-10 md:w-12 md:h-12 object-contain"
/>
```

**Linija ~278-282** (footer):
```html
<!-- Zamijenite: -->
<div class="w-10 h-10 bg-gradient-to-br from-flexio to-purple-700 rounded-xl flex items-center justify-center">
  <span class="text-white font-bold text-lg">F</span>
</div>

<!-- Sa: -->
<img 
  src="/logo.png" 
  alt="Flexio Logo" 
  class="w-10 h-10 object-contain"
/>
```

**Opcija 2: Inline SVG**

Ako imate SVG kod, možete ga direktno umetnuti umjesto placeholdera.

---

## 🔍 Kako pronaći mjesta za sadržaj

U svakoj datoteci potražite komentare:
```html
<!-- Ovdje će biti tvoj sadržaj -->
```

## 📄 Stranice za popuniti

### 1. **O nama** (`src/pages/o-nama.astro`)

**Linija ~60-70** - Glavni opis studija:
```html
<p class="text-lg leading-relaxed">
  <!-- Ovdje će biti tvoj sadržaj o studiju, historiji, filozofiji rada, itd. -->
</p>
```

**Što dodati:**
- Povijest studija
- Filozofija rada
- Misija i vizija
- Što vas razlikuje od drugih

---

**Linija ~170-180** - Opis Petre Habun:
```html
<p>
  <!-- Ovdje će biti tvoj sadržaj o Petri - biografija, iskustvo, obrazovanje -->
</p>
```

**Što dodati:**
- Biografija Petre
- Njeno obrazovanje i certifikati
- Godine iskustva
- Specijalizacije

---

### 2. **Program** (`src/pages/program.astro`)

**Linija ~60-70** - Dodatni opis Pilates mašina:
```html
<!-- Ovdje će biti dodatni opis satova -->
```

**Što dodati:**
- Detaljan opis satova na mašinama
- Trajanje satova
- Za koga je namijenjeno
- Što očekivati na satu

---

**Linija ~110-120** - Dodatni opis Yoga satova:
```html
<!-- Ovdje će biti dodatni opis satova -->
```

**Što dodati:**
- Detaljan opis Power Vinyasa Yoga
- Što uključuje sat
- Razine težine
- Benefiti

---

**Linija ~140-150** - Opis satova:
```html
<p class="text-lg">
  [Ovdje će biti detaljan opis satova koje želiš dodati]
</p>
```

**Što dodati:**
- Detaljni opis svih vrsta satova
- Struktura sata
- Što polaznici trebaju ponijeti
- Preporuke za početnike

---

**Linija ~170-180** - Cjenik:
```html
<p class="text-lg text-gray-700">
  [Ovdje će biti cjenik koji želiš dodati]
</p>
```

**Što dodati:**
- Cijene individualnih satova
- Cijene grupnih satova
- Paketi (npr. 5, 10, 20 satova)
- Mjesečne članarine
- Popusti (studenti, umirovljenici, itd.)

**Primjer strukture cjenika:**
```html
<div class="space-y-6">
  <div>
    <h4 class="text-xl font-semibold text-gray-900 mb-3">Individualni satovi</h4>
    <ul class="space-y-2 text-gray-700">
      <li class="flex justify-between">
        <span>1 sat (60 min)</span>
        <span class="font-semibold">XXX kn</span>
      </li>
      <li class="flex justify-between">
        <span>Paket 5 satova</span>
        <span class="font-semibold">XXX kn</span>
      </li>
    </ul>
  </div>
  
  <div>
    <h4 class="text-xl font-semibold text-gray-900 mb-3">Grupni satovi</h4>
    <ul class="space-y-2 text-gray-700">
      <li class="flex justify-between">
        <span>1 sat (60 min)</span>
        <span class="font-semibold">XXX kn</span>
      </li>
    </ul>
  </div>
</div>
```

---

### 3. **Događanja** (`src/pages/dogadanja.astro`)

**5 kartica događanja** (Linije ~50, ~80, ~110, ~140, ~170):

Svaka kartica ima:
```html
<p class="text-gray-700 mb-4">
  <!-- Ovdje će biti tvoj sadržaj o [NAZIV DOGAĐANJA] -->
</p>
```

**Što dodati za svako događanje:**
- Kratak opis događanja
- Kada se održava
- Trajanje
- Za koga je namijenjeno
- Cijena (ako ima)
- Kako se prijaviti

**Primjer:**
```html
<p class="text-gray-700 mb-4">
  Trodnevna Pilates radionica za sve razine. Fokus na pravilnoj tehnici 
  i izgradnji snage. Održava se svaki mjesec.
</p>
<div class="mt-4 space-y-2 text-sm text-gray-600">
  <p><strong>Kada:</strong> Svaki prvi vikend u mjesecu</p>
  <p><strong>Trajanje:</strong> 3 dana (petak-nedjelja)</p>
  <p><strong>Cijena:</strong> XXX kn</p>
</div>
```

---

### 4. **Galerija** (`src/pages/galerija.astro`)

**Linija ~80-90** - Dodavanje fotografija:

Trenutno ima placeholder grid. Zamijenite placeholder kartice s pravim slikama:

```html
<!-- Umjesto placeholdera: -->
<div class="aspect-square rounded-2xl bg-gradient-to-br from-purple-100 to-pink-100...">
  <!-- placeholder SVG -->
</div>

<!-- Dodajte: -->
<div class="aspect-square rounded-2xl overflow-hidden hover:shadow-xl transition-shadow">
  <img 
    src="/images/galerija/slika-1.jpg" 
    alt="Opis slike"
    class="w-full h-full object-cover hover:scale-105 transition-transform duration-300"
  />
</div>
```

**Koraci za dodavanje slika:**
1. Dodajte fotografije u `public/images/galerija/` folder
2. Zamijenite placeholder kartice s `<img>` tagovima
3. Dodajte dobre alt tekstove za pristupačnost

---

**Linija ~110-120** - Arhiva fotografija:
```html
<p class="text-gray-700">
  [Ovdje će biti arhiva starijih fotografija]
</p>
```

**Što dodati:**
- Linkove na albume po godinama
- Linkove na događanja
- Ili jednostavno još jedan grid fotografija

---

### 5. **Kontakt** (`src/pages/kontakt.astro`)

**Linija ~85-95** - Točna adresa (opciono):
```html
<p class="text-lg text-gray-900 font-semibold">
  Zagreb, Hrvatska
</p>
<!-- Ovdje možeš dodati točnu adresu -->
```

**Dodaj ako želiš:**
```html
<p class="text-sm text-gray-600 mt-1">
  Ulica i broj, 10000 Zagreb
</p>
```

---

## 💡 Savjeti

### 1. Formatiranje teksta
Koristite HTML tagove za formatiranje:
```html
<p>Običan tekst</p>
<strong>Podebljani tekst</strong>
<em>Kurziv</em>
<br /> <!-- novi red -->
```

### 2. Liste
```html
<ul class="space-y-2">
  <li>Stavka 1</li>
  <li>Stavka 2</li>
  <li>Stavka 3</li>
</ul>
```

### 3. Naglašeni blokovi
```html
<div class="bg-purple-50 rounded-xl p-4 mb-6">
  <p class="text-sm text-purple-900 leading-relaxed">
    Važna napomena ili posebna informacija
  </p>
</div>
```

### 4. Linkovi
```html
<a href="/program" class="text-flexio hover:underline">
  Link tekst
</a>
```

## 🎨 CSS klase koje možete koristiti

- **Boje teksta:** `text-gray-900`, `text-gray-600`, `text-flexio`
- **Veličine teksta:** `text-sm`, `text-base`, `text-lg`, `text-xl`, `text-2xl`
- **Boldanje:** `font-semibold`, `font-bold`
- **Razmak:** `mb-4` (margin-bottom), `mt-4` (margin-top), `space-y-4` (razmak između elemenata)
- **Pozadina:** `bg-purple-50`, `bg-white`, `bg-gray-50`

## 🚀 Testiranje izmjena

Nakon što dodate sadržaj:

```bash
# Dev server će automatski prikazati promjene
npm run dev

# Ili rebuildirajte
npm run build
```

Otvorite browser i pregledajte stranice na:
- http://localhost:4323/ (ili koji god port prikazuje terminal)

---

## ❓ Pomoć

Ako niste sigurni kako nešto dodati, pogledajte postojeći kod na drugim stranicama kao primjer, ili se javite!

Sretno s dodavanjem sadržaja! 🎉

