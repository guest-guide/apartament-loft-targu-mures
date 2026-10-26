# Apartament Loft Târgu Mureș. Webes vendégkalauz

## GitHubra feltöltés

1. Csomagold ki a ZIP-et. A ZIP-et magát ne töltsd fel weboldalként.
2. A kicsomagolt fájlokat és az assets mappát együtt másold a GitHub-repozitórium gyökerébe. Az index.html közvetlenül a gyökérben legyen, ne egy újabb csomagmappában. Az almappák szerkezete maradjon meg.
3. Ha meglévő oldalt frissítesz, az azonos nevű fájlokat cseréld le, a régi, már nem használt fájlokat távolítsd el.
4. GitHub: Settings > Pages > Source: Deploy from a branch. Branch: main (vagy a használt ág), folder: /(root), majd Save.
5. A Pages részen megjelenő linket nyisd meg. Saját domain nem szükséges.

Ez kész statikus weboldal. Nincs szükség npm-re, fordításra, adatbázisra vagy fizetős tartalomkezelőre. A .nojekyll fájlt is tartsd meg. A képek helyben, az assets mappában vannak. A videókhoz, térképekhez és külső oldalakhoz internet kell.

Hivatalos útmutató: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Adatvédelem és hozzáférés

A csomag az apartman aktuális változatát tartalmazza, a bejutási kóddal, a Wi-Fi-jelszóval és a megadott elérhetőségekkel együtt. Nyilvános GitHub-repozitóriumban ezek a forrásfájlokból is kiolvashatók. A szokásos GitHub Pages-oldal nyilvános akkor is, ha a forrásrepo privát. A jelenlegi Sites-oldal privát hozzáférését a ZIP nem viszi át a GitHubra.

A noindex,nofollow,noarchive metaelem megmaradt. Ez keresőrobotoknak szóló kérés, nem hozzáférés-védelem. Nem akadályozza meg a link továbbküldését, a tartalom megnyitását vagy a letöltését. A kulcsszéf kódját nyilvános oldal helyett célszerű külön, privát vendégüzenetben megadni. Valódi hozzáférés-védelemhez külön, kiszolgálóoldali hitelesítést biztosító tárhely szükséges; JavaScriptben tárolt jelszó nem elegendő.

## Tartalom szerkesztése

Az editor.html oldalon módosíthatók a tartalmak és az elérhetőségek. A mentés az adott böngésző helyi tárhelyére történik. Ez nem közös online adminisztráció és nem írja át automatikusan a vendégoldalt.

A szerkesztőből exportáld a JSON-t, majd a GitHubon cseréld le vele a content.json fájlt. Frissítés után teszteld a vendégoldalt. Az editor.html nem kér bejelentkezést; a helyi szerkesztés nem ad másoknak jogosultságot a GitHub-fájlok átírására.

## Érvényesség és ellenőrzés

A vendégoldal csak approved státuszú, aktuális időszakra érvényes tartalmakat mutat. Az adatok jelenlegi validUntil dátuma több helyen 2026-11-26. Lejárat után a kártyák eltűnnek. Ellenőrzés után a checkedAt és validUntil dátumokat is frissítsd; ne csak a szöveget.

A content.json a Loft adatait, a template.json a márkafüggetlen kiinduló sablont tartalmazza. A sablon nem kész vendégoldal: új szálláshelynél a saját adatokat és fordításokat ki kell tölteni és ellenőrizni.

## Fájlok

index.html: vendégfelület. app.js: működés és felületi fordítások. style.css: megjelenés. content.json: háromnyelvű tartalom és elérhetőségek. assets/: fotók. editor.html és editor.js: helyi szerkesztő. template.json: újrafelhasználható sablon. UTMUTATO.md: karbantartás és bevezetés. TARTALOM_HU_RO_EN.md: háromnyelvű szöveges áttekintés.

## Kipróbálás

A fájl közvetlen dupla kattintásos megnyitása a JSON-betöltés miatt nem minden böngészőben működik. Használj helyi webszervert, például VS Code Live Servert, vagy teszteld a feltöltött oldalt.

Ellenőrizd a három nyelvet, a fotókat és nagyításukat, a jelszómásolást, a videókat, a térképet, a WhatsApp- és telefongombokat, a Google Maps-adatlap linkjét, valamint a mobilnézetet. A külső helyek aktuális adatait és a képek felhasználási jogát a szállásadó ellenőrizze.
