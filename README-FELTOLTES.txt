SOMZON STUDIO - FELTOLTESI UTMUTATO (v2 - fejlesztett verzio)

UJDONSAGOK EBBEN A VERZIOBAN:
- Portfolio szekcio: valodi projektek (VindPro Service linkkel, Stop Dance Party, sajat jatekok) a korabbi "demo otletek" helyett.
- Kapcsolati urlap: mailto helyett Netlify Forms (AJAX kuldes, siker/hiba uzenet mindharom nyelven, honeypot spam-vedelem). Netlify-n automatikusan mukodik, semmit nem kell beallitani.
- Tipografia: Space Grotesk cimsorok + Inter szoveg (Google Fonts, preconnect-tel).
- SEO: JSON-LD strukturalt adat (ProfessionalService), og:locale, theme-color; a felesleges meta keywords torolve.
- Akadalymentesites: "Ugras a tartalomhoz" link, lathato fokusz (focus-visible), prefers-reduced-motion tamogatas.
- Szovegek: a "belso jegyzet" jellegu mondatok (pl. "amig nincs sok ugyfelprojekt...", "ez segit, hogy az ugyfel...") atirva valodi marketingszovegre mindharom nyelven.
- SEO szekcio: kulcsszofelho helyett konkret, pipas lista arrol, mit tartalmaz a SEO-munka.
- Kalkulator: uj cim/szoveg + "iranyar" megjegyzes.
- Apro javitasok: mobil menu, select opciok sotet hattere, localStorage try/catch (privat mod), ev automatikus frissitese nyelvvaltasnal is.

Fajlok:
- index.html
- styles.css
- script.js
- favicon.svg
- robots.txt
- sitemap.xml

Feltoltes Netlify-re:
1. Csomagold ki a ZIP-et.
2. Netlify -> Add new site -> Deploy manually.
3. Huzd be a teljes somzon_site mappat.
4. Az elso deploy utan a Forms fulon megjelenik a "contact" urlap - itt allithatsz be email ertesitest (Form notifications).
5. Ha mukodik, add hozza a sajat domaint.

Amit elesites elott cserelj:
- hello@somzon.dk -> sajat email (index.html: 3 helyen + script.js hibauzenetek + JSON-LD)
- +45 00 00 00 00 -> sajat telefonszam (vagy torold a sort, ha nem akarsz telefonszamot kiirni)
- https://somzon.dk/ -> valodi domain (index.html: canonical + og:url, sitemap.xml, robots.txt)
- og-image.jpg -> keszits egy 1200x630 px megoszto kepet es told fel a gyokerbe (vagy torold az og:image sort)
- Stop Dance Party: ha szeretnel Play Store linket a kartyara, add hozza az index.html-ben

Megjegyzes: Cloudflare Pages-en az urlap NEM mukodik (a Netlify Forms Netlify-specifikus).
Ha Cloudflare-re mesz, csereld az urlapot Formspree-re (action="https://formspree.io/f/AZONOSITO").
