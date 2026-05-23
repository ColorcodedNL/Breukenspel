# Breukenspel

Een interactief breukenspel voor kinderen van groep 3/4 (ca. 6 jaar). Gebouwd als één HTML-bestand zonder dependencies — werkt direct in de browser, ook op iPad en tablet.

🔗 **Live spelen:** [colorcodednl.github.io/Breukenspel](https://colorcodednl.github.io/Breukenspel/)

---

## Wat het doet

Het spel bestaat uit twee modi:

### 🎯 Tellen
Een willekeurige opgave verschijnt bovenaan, bijvoorbeeld "Maak 3/4". Het kind tikt op de taartpunten om segmenten te kleuren. Bij het goede antwoord verschijnt een felicitatiebanner met confetti en een knop voor de volgende opgave. Elke ronde heeft een andere noemer zodat dezelfde opgave niet twee keer achter elkaar verschijnt.

### ➕ Rekenen
Breuken van 1/1 t/m 1/12 staan als knoppen klaar. Het kind klikt er een of meer aan en ziet live in de taart en de som wat de combinatie oplevert. Breuken die niet netjes combineren (waarbij de gemeenschappelijke noemer groter dan 12 zou worden) worden automatisch grijs zodra de eerste keuze is gemaakt. Een korte uitleg verschijnt als het kind toch op een grijze knop tikt.

---

## Kenmerken

- Geen installatie — gewoon `index.html` openen in de browser
- Werkt op iPad, tablet en desktop
- Volledig responsive layout: taartdiagram vult altijd de beschikbare ruimte tussen de vaste elementen boven en onder (`100dvh`)
- Taartdiagram met duidelijke lijntjes per segment
- Elke breuk in de som heeft een eigen kleur die overeenkomt met het taartpunt
- Equivalente breuken carousel: naast de gereduceerde breuk worden links en rechts equivalenten getoond (bijv. bij 1/2 ook 2/4 en 3/6)
- Confetti-animatie bij goed antwoord
- Vriendelijke paarse vormtaal met pill-knoppen
- Combinatielogica: alleen breuken toegestaan waarvan de gemeenschappelijke noemer ≤ 12 blijft (bijv. 1/2 + 1/4 werkt, 1/2 + 1/3 ook, maar 1/2 + 1/5 niet)

---

## Bestanden

| Bestand | Omschrijving |
|---|---|
| `index.html` | Het volledige spel |
| `favicon-32.png` | Favicon (32x32 PNG) |
| `apple-touch-icon.png` | iOS home screen icoon (180x180 PNG) |

---

## Gebruik

```bash
# Clone het repository
git clone https://github.com/ColorcodedNL/Breukenspel.git

# Open het bestand in je browser
open index.html
```

Of download gewoon `index.html` (+ de twee PNG-bestanden) en open het lokaal — geen server nodig.

Of speel direct online via GitHub Pages: https://colorcodednl.github.io/Breukenspel/

---

## Achtergrond

Gemaakt voor mijn dochter (6 jaar) om breuken te oefenen op de iPad. De combinatie van visueel taartdiagram, directe feedback en de koppeling naar percentages en equivalente breuken sluit aan bij wat ze op school leert.

---

## Techniek

- Puur HTML/CSS/JavaScript — geen frameworks, geen build-stap
- Canvas API voor de taartdiagrammen
- Responsive layout via flexbox en `100dvh`
- Alle logica in één bestand

---

## Licentie

MIT — gebruik en pas gerust aan.
