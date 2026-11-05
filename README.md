# Westnut website — versie 4

Deze statische website werkt met **Cloudflare Pages** en **Pages CMS**.

## Publiceren
1. Pak het ZIP-bestand uit. Upload **alle bestanden en mappen** (ook `.pages.yml`) naar de hoofdmap van GitHub-repository `FilipDonck/westnut-website` op branch `main`. Upload de ZIP zelf niet.
2. Cloudflare dashboard → Workers & Pages → Create → Pages → Connect to Git → selecteer `westnut-website`.
3. Framework preset: **None**. Build command: **leeg laten**. Build output directory: **/** (repository root; als Cloudflare `.` verwacht, gebruik `.`). Deploy.
4. Ga naar https://app.pagescms.org en meld aan via GitHub; geef Pages CMS toegang tot `westnut-website`. Open de repository op branch `main`.
5. Wijzig Website-instellingen, Hazelnootrassen, Producten of Nieuws. Opslaan schrijft naar GitHub; Cloudflare bouwt opnieuw.

## Belangrijk
- De website laadt JSON-bestanden via `fetch`. Daarom werkt dubbelklikken op `index.html` niet altijd; test via de Cloudflare-URL of met `python -m http.server 8000` in deze map.
- `info@westnut.be` werkt pas nadat je het domein hebt gekocht en e-mailrouting hebt ingesteld.
- Prijzen en beschikbaarheid worden getoond, maar er is **geen winkelmandje, betaling of bestelsysteem**.
- Voor het CMS is een GitHub-toestemming nodig; de website zelf heeft geen eigen admin-login.
- De huidige productfoto toont **proefrecepturen**.
- De website bevat Google Fonts; deze worden extern geladen.
- Voeg vóór een zakelijke lancering de juiste bedrijfsgegevens en privacyinformatie toe.
