# Talleventyret 🌟

Et mattespill for 1.–2. klasse laget for en 6-åring som gjøres klar til 2. klasse.

🎮 **[Spill her](https://michaelaglen.github.io/Talleventyret/)**

---

## Om spillet

Talleventyret er et enkelt, mobilevennlig mattespill med mørkt space-tema. Ingen innlogging, ingen reklame, ingen app å installere — bare åpne lenken og spill.

### Segmenter

| | Segment | Hva |
|---|---|---|
| 🔢 | Tall og mengder | Tell og gjenkjenn tall 1–10 |
| 🥚 | Vennetall | Tallpar som gir 10 |
| ➕ | Addisjon | Legg sammen innen 10 |
| ➖ | Subtraksjon | Ta bort og tell innen 10 |
| 🔡 | Tallrekken | Rekkefølge og mønster til 20 |

Trykk **ℹ** på et segment for å lese hva barnet lærer.

### Oppgavetyper

6 ulike interaksjoner holder det variert:

- **Knapper** — velg riktig svar
- **Skyveknapp** — dra til riktig tall
- **Tallinje** — trykk på riktig posisjon
- **Trykk-for-å-fjerne** — ta bort emojier
- **Fyll inn** — fyll eggekartong til 10
- **Sorter** — plasser tall i riktig rekkefølge

### Gamification

- ⭐ 0–3 stjerner per segment basert på andel riktige
- 🔥 Streak-indikator ved 3+ riktige på rad
- Rangsystem basert på totale stjerner:
  - 📚 Matteelev → ⭐ Mattestjerne → 🚀 Romfarer → 🌌 Galaksemester → 🌟 Universets Helt
- Ny tittel-popup ved rangopprykk
- Stjernedusj ved perfekt runde (3 stjerner)
- Fremgang lagres i nettleseren (localStorage)

---

## Deploy til GitHub Pages

1. Fork eller last opp `index.html` til et nytt GitHub-repo
2. Gå til **Settings → Pages**
3. Under *Source*: velg `main` branch, rot `/`
4. Trykk **Save** — appen er live etter ~30 sekunder på `https://[brukernavn].github.io/[repo-navn]`

Ingen build-steg, ingen avhengigheter å installere. Én enkelt HTML-fil.

> **Merk:** Bakgrunnsmusikk krever at siden hostes på http/https (GitHub Pages). Åpner du `index.html` lokalt fra disk spilles syntetisk ambient-musikk i stedet.

---

## Teknisk

- React 18 via CDN, JSX transpilert med Babel Standalone
- Web Audio API for spilllyder (riktig, feil, streak, seier)
- YouTube IFrame API for bakgrunnsmusikk
- `localStorage` for lagring av fremgang
- Ingen build-steg, ingen `node_modules`, ingen konfigurasjon
- Fungerer på mobil, iPad og PC
