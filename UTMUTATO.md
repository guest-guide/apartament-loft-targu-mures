# Két kép hozzáadása a saját weboldaladhoz

1. GitHub Desktop: válaszd ki az apartman repozitóriumát. Repository > Show in Explorer. Ebben a mappában dolgozz.
2. Másold a csomag assets mappájában lévő két JPG-képet a saját assets mappádba.
3. Nyisd meg a saját content.json fájlodat VS Code-ban. Ctrl+F: "id": "arrival". Ennél az egy bejegyzésnél a title mező hu, ro és en értéke legyen Check-in. Az images tömböt cseréld a modositasok.json arrival/images részére.
4. Ctrl+F: "id": "parking". Csak ennek a bejegyzésnek az images tömbjét cseréld a modositasok.json parking/images részére. Ha nincs images mező, a bejegyzésen belül add hozzá. Ügyelj a JSON-mezők közötti vesszőre.
5. A saját body szövegeidet, parkolási adataidat és a többi mezőt hagyd meg. A modositasok.json csak másolási minta: ne nevezd át content.json-ra, nem teljes adatfájl.
6. Ctrl+S. A két kártya a meglévő elrendezésben számítógépen egymás mellett, telefonon egymás alatt jelenik meg. A CSS-t nem kell módosítanod.
7. GitHub Desktop > Changes: ellenőrizd a két új képet és a content.json módosítását. Summary: Check-in és parkolási képek. Commit to main (vagy az aktuális ág), majd Push origin. Ha a program előbb távoli frissítést kér, Fetch/Pull után folytasd.
8. Ha GitHub Pages már a használt ágat publikálja, a weboldal automatikusan frissül. Szükség esetén Ctrl+F5-tel töltsd újra.

A teljes weboldal ZIP-jét nem kell rámásolnod a saját mappádra. Ez a kis csomag megőrzi a közben átírt szövegeidet.
