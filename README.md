# Flexio Pilates & Yoga Studio - Web stranica

Moderna i responzivna web stranica za Flexio Pilates & Yoga Studio u Zagrebu.

## 🎯 Karakteristike

- ✨ Moderan, minimalistički dizajn
- 📱 Potpuno responzivna (mobilna verzija prilagođena)
- 🚀 Brzo učitavanje (Astro SSG)
- 🎨 Tailwind CSS za styling
- ♿ Pristupačna (accessibility standardi)
- 🔍 SEO optimizirana

## 🛠️ Tehnologije

- **[Astro](https://astro.build/)** - Static Site Generator
- **[Tailwind CSS](https://tailwindcss.com/)** - CSS framework
- **[TypeScript](https://www.typescriptlang.org/)** - Type safety
- **React** - Interaktivne komponente (ako potrebno)

## 📦 Instalacija

1. Klonirajte repozitorij ili preuzmite datoteke
2. Instalirajte dependencies:

```bash
npm install
```

## 🚀 Pokretanje

### Development server

```bash
npm run dev
```

Stranica će biti dostupna na `http://localhost:4321`

### Build za produkciju

```bash
npm run build
```

### Preview produkcijskog build-a

```bash
npm run preview
```

## 📁 Struktura projekta

```
/
├── public/          # Statički fajlovi (favicon, slike)
├── src/
│   ├── layouts/    # Layout komponente
│   │   └── Layout.astro    # Glavni layout (header, footer, navigacija)
│   ├── pages/      # Stranice (.astro)
│   │   ├── index.astro     # Naslovnica
│   │   ├── o-nama.astro    # O nama / Učitelji
│   │   ├── program.astro   # Program / Opis satova / Cjenik
│   │   ├── dogadanja.astro # Događanja / Radionice / Workshopovi
│   │   ├── galerija.astro  # Galerija fotografija
│   │   ├── kontakt.astro   # Kontakt forma i info
│   │   └── index-old.astro # Backup stare one-page verzije
│   └── styles/     # Globalni stilovi
│       └── global.css
├── astro.config.mjs
├── tailwind.config.mjs
└── package.json
```

## 🎨 Customizacija

### Boje

Glavna boja brenda je definirana u `tailwind.config.mjs`:

```js
colors: {
  flexio: '#662d91', // Ljubičasta boja
}
```

### Fontovi

Projekt koristi:

- **Inter** - za body tekst
- **Playfair Display** - za naslove

Fontovi se učitavaju iz Google Fonts u `index.astro`.

### Sadržaj

#### Gdje dodati sadržaj:

**Layout (zajednički elementi):**
- `src/layouts/Layout.astro` - Header, Footer, Navigacija

**Zasebne stranice:**
- `src/pages/index.astro` - Naslovnica
- `src/pages/o-nama.astro` - **← DODAJ sadržaj o studiju i učiteljima**
- `src/pages/program.astro` - **← DODAJ opise satova i cjenik**
- `src/pages/dogadanja.astro` - **← DODAJ opise događanja**
- `src/pages/galerija.astro` - **← DODAJ fotografije**
- `src/pages/kontakt.astro` - Kontakt (već popunjeno)

#### Kako dodati sadržaj:

1. Otvori željenu datoteku (npr. `o-nama.astro`)
2. Pronađi komentare oblika `<!-- Ovdje će biti tvoj sadržaj -->`
3. Zamijeni komentare sa svojim sadržajem
4. Spremi promjene
5. Stranica se automatski ažurira u dev serveru

**Napomena:** Backup stare one-page verzije nalazi se u `src/pages/index-old.astro`

## 📄 Stranice

Stranica je organizirana kao **multi-page website** s odvojenim stranicama:

### 1. **Naslovnica** (`/`)
- Hero sekcija s glavnim sloganom
- Pregled B.A.S.I. certifikacije
- Pregled programa
- CTA za kontakt

### 2. **O nama** (`/o-nama`)
- Informacije o studiju i B.A.S.I. Pilates
- Sekcija o Petri Habun (vlasnica i učiteljica)
- Dodatni učitelji (spremno za dodavanje)
- **→ Ovdje dodaj svoj sadržaj o studiju i učiteljima**

### 3. **Program** (`/program`)
- Pilates mašine (detaljno)
- Power Vinyasa Yoga
- Opis satova
- Cjenik
- **→ Ovdje dodaj detaljne opise satova i cjenik**

### 4. **Događanja** (`/dogadanja`)
- Pilates radionica
- Develop na otoku Rabu
- Prenatal workshop
- Dan pilatesa
- B.A.S.I. weekend
- **→ Ovdje dodaj sadržaj o svakom događanju**

### 5. **Galerija** (`/galerija`)
- Fotografije studija
- Arhiva fotografija
- **→ Ovdje dodaj fotografije**

### 6. **Kontakt** (`/kontakt`)
- Kontakt forma
- Email: petra@flexio.com.hr
- Telefon: 099 2157 495
- Facebook link

### Zajednički elementi (Layout)
- **Navigation** - Sticky navigacija s mobilnim menijem (prisutna na svim stranicama)
- **Footer** - Navigacijske linkove i društvene mreže (prisutna na svim stranicama)

## 📱 Mobilna verzija

Stranica je potpuno responzivna s breakpoints:

- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

Mobilni meni se automatski prikazuje na malim ekranima.

## 🔧 Deployment

### Vercel (preporučeno)

1. Push kod na GitHub
2. Povežite repozitorij s Vercel
3. Vercel će automatski detektirati Astro i deployati stranicu

### Netlify

1. Push kod na GitHub
2. Povežite repozitorij s Netlify
3. Build command: `npm run build`
4. Publish directory: `dist`

### GitHub Pages

```bash
npm run build
# Deploy sadržaj `dist` foldera na GitHub Pages
```

## 📧 Kontakt forma

Trenutno kontakt forma koristi `mailto:` link koji otvara klijentov email program.

Za produkciju preporučujemo:

- **Formspree** - https://formspree.io/
- **Web3Forms** - https://web3forms.com/
- **EmailJS** - https://www.emailjs.com/
- Ili vlastiti backend endpoint

## 🌐 Browser podrška

Stranica podržava sve moderne browsere:

- Chrome (najnovija verzija)
- Firefox (najnovija verzija)
- Safari (najnovija verzija)
- Edge (najnovija verzija)

## 📄 Licenca

© 2008 - 2025 Flexio Pilates Yoga Studio. Sva prava pridržana.

## 🤝 Kontakt

Za pitanja o web stranici:

- **Email**: petra@flexio.com.hr
- **Telefon**: 099 2157 495
- **Facebook**: https://www.facebook.com/flexio.hr

---

Made with ❤️ using Astro & Tailwind CSS
