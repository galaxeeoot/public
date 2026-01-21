# 3D eventyrspill (åpen verden) – konsept

Dette dokumentet beskriver et forslag til et **3D eventyrspill** med sverd, fiender, boss og høy vanskelighetsgrad i en åpen verden. Målgruppen er spillere som liker krevende kamp og utforsking.

## Kjerneidé
- **Sjanger:** 3D action‑eventyr i åpen verden.
- **Fokus:** Taktisk sverdkamp, utforsking, og krevende bosskamper.
- **Tone:** Mørk fantasi med mystiske ruiner og farlige villmarker.

## Spillerens rolle
- En ensom vandrer som bærer et eldgammelt sverd.
- Oppdraget er å gjenopprette balansen i en verden der monstre har tatt over tidligere kongedømmer.

## Verden
- **Åpen verden** delt inn i 4 regioner:
  1. **Tåke‑skogene** (tett vegetasjon, raske fiender).
  2. **Aske‑ørkenen** (lang sikt, snikende jegere).
  3. **Storm‑kysten** (vertikale klipper, vind som påvirker kamp).
  4. **Ruinkrateret** (sentral hub, tilgang til dungeons).
- **Dynamiske værforhold**: regn gjør bakken glattere, torden kan avsløre skjulte stier.

## Kampsystem
- **Sverdkamp** med fokus på timing og posisjonering.
  - **Lett angrep**: raskt, lav skade.
  - **Tungt angrep**: tregt, høy skade, bryter skjold.
  - **Parering**: presis timing åpner for kritiske treff.
  - **Unnvik**: rull og sidehopp med stamina‑kostnad.
- **Stamina** styrer hvor mye spilleren kan angripe og unnvike.

## Vanskelighetsgrad
- **Høy utfordring** fra start, men rettferdig.
- Fiender lærer spilleren mønstre og timing.
- Bossene krever mestring av blokkering, parering og posisjon.

## Fiender
- **Skogsvoktere**: raske, aggressive, tvinger spilleren til å bevege seg.
- **Askejegere**: sniker seg og angriper bakfra.
- **Stormriddere**: tung rustning, sakte men harde slag.
- **Ruinbeist**: store, tilfeldige angrepsmønstre.

## Boss‑design
- **Navn:** Kraterets Vokter.
- **Fase 1:** Store, telegrapherte slag og sjokkbølger.
- **Fase 2:** Får nye angrep med magisk energi og raskere kombinasjoner.
- **Arena:** Rund slette med søyler som kan brukes til dekning.

## Fremdrift
- Utforsking låser opp nye ferdigheter og områder.
- **Relikvier** gir permanente oppgraderinger.
- **Skjulte helligdommer** gir midlertidige buffs for bosskamper.

## Spillerprogresjon
- **Oppgraderinger:**
  - Økt stamina.
  - Bedre pareringstiming.
  - Nye sverdteknikker.
- **Utstyr:** Sverd og rustning med små, men merkbare forbedringer.

## Hovedloop
1. Utforsk region → finn ruiner og fiendetyper.
2. Samle relikvier og oppgraderinger.
3. Gå inn i dungeon → bekjemp miniboss.
4. Åpne ny region eller bossarena.

## Mini‑mål for prototype
- En liten åpen verden med én region.
- 2 fiendetyper + 1 miniboss.
- Grunnleggende sverdkamp (lett/tung/parering/unnvik).
- Enkel stamina‑bar.

## Unreal Engine‑fokus
Hvis du vil lage prototypen i **Unreal Engine**, kan du starte slik:

### Anbefalt oppsett
- **Prosjektmal:** Third Person (gir ferdig kamera og bevegelse).
- **Kampsystem:** Legg til svingslag med Animation Montages og hit‑traces.
- **Parering/unnvik:** Bruk animasjonsnotifier + timing‑vinduer i Blueprint.
- **Stamina:** Variabel på Character + binding til UI i UMG.

### Prototype‑milepæler (Unreal)
1. **Bevegelse + kamera** fungerer stabilt i åpen verden.
2. **Sverdkamp** med lett/tung angrep + enkel trefflogikk.
3. **Stamina og UI** viser ressurs og hindrer spamming.
4. **Én fiendetype** med enkel AI (patrulje → jag → angrep).
5. **Miniboss** med 2 angrepsmønstre og fasebytte.

### Bygg app (Unreal)
- **Build/Package:** Bruk *File → Package Project* for målplattformen (Windows/Mac/Linux).
- **Konfigurasjon:** Test i **Development** før **Shipping** for endelig build.
- **Innhold:** Sjekk at alle nivåer og assets er inkludert i Project Settings → Packaging.

### Neste steg
Hvis du vil kan jeg også:
- Lage en mer detaljert **game design document (GDD)**.
- Skissere **kontroller** og **UI**.
- Lage et **implementasjonsnotat** spesielt for Unreal (Blueprint/C++).
