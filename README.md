# Trimble Connect MiniMap 🗺️

Trimble Connect MiniMap er en kart-utvidelse (Workspace API Extension) utviklet for Trimble Connect. Utvidelsen synkroniserer kameraets posisjon i 3D-modellen med et dynamisk 2D-kart, noe som gir en sømløs kobling mellom BIM-modellen og geografiske GIS-data. 

Spesialtilpasset for norsk samferdselsprosjektering med støtte for NTM- og UTM-koordinatsystemer.

## ✨ Hovedfunksjoner
* **Sanntidssynkronisering:** 2D-kartet følger automatisk etter deg når du navigerer i 3D-vinduet i Trimble Connect.
* **Norske koordinatsystemer:** Innebygd støtte for EUREF89 NTM (sone 5-30) og UTM (sone 32 og 33).
* **Pre-definerte kartlag:** Ferdig oppsatt med Norges Grunnkart, Flyfoto, Vektorkart, Matrikkel, FKB og NVDB-data. 
* **Dynamisk WMS-støtte:** Legg til egne eksterne kartlag via WMS direkte i utvidelsen ved behov.
* **Automatisk tegnforklaring (Legend):** Henter og viser tegnforklaring for aktive WMS-lag asynkront.
* **Adressesøk:** Innebygd integrasjon mot Kartverkets REST-API for å flytte kartet til spesifikke adresser.
* **Street View:** Hopp direkte fra 3D-kameraets posisjon og ned på bakken i Google Street View med ett klikk.

## 🛠️ Installasjon og oppsett i Trimble Connect

Det er ikke nødvendig å laste ned noen filer for å ta i bruk utvidelsen. Alt gjøres direkte inne i Trimble Connect:

1. Åpne prosjektet ditt i **Trimble Connect for Browser** (3D Viewer).
2. Gå til **Extensions** (Puslespill-ikonet) i menyen til venstre.
3. Klikk på **Add Extension** (eller "+"-ikonet).
4. Lim inn følgende URL:
   `https://vidmet.github.io/wms-service/wms.json`
5. Utvidelsen (MiniMap) vil nå dukke opp i listen din og er klar til bruk!

## 📌 Slik bruker du kartet
1. **Velg koordinatsystem:** Ved oppstart, velg hvilket koordinatsystem 3D-modellen er prosjektert i (f.eks. NTM Sone 11). Kartet vil umiddelbart hoppe til riktig lokasjon når du beveger deg i 3D.
2. **Lagstyring:** Bruk lag-ikonet øverst til høyre på selve kartet for å bytte bakgrunnskart, og for å slå av/på transparente overlag (WMS).
3. **Manuelt WMS-tillegg:** Hvis du raskt trenger et lag som ikke ligger i standardmenyen, limer du inn WMS GetCapabilities-URLen og et lagnavn under punkt 2 i panelet. Systemet vasker automatisk URLen for deg og legger det i kartet.

---
***Utviklet av** Vidar Metveit* ***for** Norconsult Norge AS.*