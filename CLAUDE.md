# kaminer

Samlingsrepo för två kaminsajter i nätverket: **bastakaminen.se** och
**kamininstallation.se**. Båda är i dagsläget minimala "kommer snart"-sidor
(lansering 2026) byggda som varsitt fristående Astro 5-projekt med en enda
sida (`src/pages/index.astro`). Repot innehåller även en affärsanteckning
(`Ny(tt) Textdokument.txt`) om en eventuell försäljning av domänen kamin.se.

## Kommandon

Kör kommandon inne i respektive sajtmapp (`bastakaminen.se/` eller
`kamininstallation.se/`):

```bash
npm install        # installera beroenden (per sajt)
npm run dev        # dev-server
npm run build      # bygger till dist/
npm run preview    # förhandsgranska bygget
```

## Viktigt

- Två separata npm-projekt i samma repo — de delar ingen kod och har varsin
  `package.json`, `node_modules/` och `dist/`. Rotmappen har ingen egen
  `package.json`.
- Ingen deploy-konfiguration (netlify.toml/vercel.json) finns i repot.
- Sajterna är rena enkelsidor utan datakälla — allt innehåll ligger inline i
  `index.astro`.

## Nätverkskunskap (vu-skill-catalog)

Innan större ändringar (feed-import, cache/ISR, SEO/indexering, cron, nya routes):
läs `~/projekt/vu-skill-catalog/INDEX.md` — en rad + beskrivning per löst problem
och playbook i nätverket. Öppna bara filer vars beskrivning träffar ärendet.
