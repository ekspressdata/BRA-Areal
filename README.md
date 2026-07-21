# BRA Areal - Arealmåling i nettleseren

https://github.com/user-attachments/assets/881b4f37-079d-4c64-9e65-69ac387900a0

BRA Areal er en nettapp som måler arealer i plantegninger etter
norske regler (NS 3940, matrikkelføringsinstruksen). Brukeren laster
opp plantegninger, setter målestokker, tegner opp rommene – og får nøyaktige areal
i m².

🔗 **Prøv den her: [braareal.no](https://braareal.no)**

---

## Hva den gjør

- **Last opp plantegning** – PDF, PNG eller JPEG. Alt skjer lokalt i
  nettleseren; ingen tegninger forlater maskinen.
- **Sett målestokk manuelt** – klikk to punkter med kjent avstand, skriv inn
  lengden, og appen regner ut px/m for siden. Flere målestokklinjer per side
  gir et snitt med avviksvarsel.
- **Tegn polygoner** – klikk opp hjørnene, med snapping mot vegglinjer og
  hjørner for presise omriss.
- **Få arealet** – levende m²-utregning per polygon, med et
  usikkerhetsestimat (±) basert på sidens egne målestokklinjer.
- **Navigasjon** – jevn zoom og panorering, sidenavigasjon, rotasjon i 90°, og
  en lupe som forstørrer tegningen mens du plasserer punkter.

Måleprinsippet er bygget rundt **riktige tall først** 

---

## Teknologi

| Område | Valg |
|---|---|
| Språk | TypeScript (strict) |
| Byggverktøy | Vite |
| UI-rammeverk | Svelte 5 (runes) |
| Styling | Tailwind CSS 4 + shadcn-svelte |
| PDF-rendering | pdf.js 6 |
| Overlay/tegning | SVG (deklarativt) |
| OCR (planlagt) | Tesseract.js |
| Testing | Vitest |
| Kvalitetssikring | ESLint, Prettier, `tsc --noEmit` |
| Backend & auth | Supabase (Postgres, EU – Stockholm), magisk-lenke-innlogging |
| Transaksjonell e-post | Brevo |
| Webanalyse | Umami (cookieless, EU) |
| Hosting | Cloudflare (Worker med statiske filer) |

---

## Domeneregler

Arealene følger norsk standard og forvaltningspraksis:

- **NS 3940** – måleregler for areal og volum i bygninger
- **Matrikkelføringsinstruksen** – offentlig regelverk for matrikkelregistrering

---



---

*Utviklet i Norge.*



