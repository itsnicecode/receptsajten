# Receptsajten

En responsiv receptsajt byggd med semantisk HTML och modern CSS. Projektet har utvecklats succesivt under fyra veckor, från en enkel receptsida till en sammanhängande webbplats med startsida, receptsida och formulär för att dela egna recept.

Fokus har legat på tillgänglighet, responsiv design, återanvändbar CSS och ett konsekvent designsystem, helt utan Javascript.

## Innehåll

- Semantisk HTML och tillgänglighetsanpassad struktur
- Responsiv layout med CSS grid och flexbox
- Designsystem med CSS custom properties och OKLCH
- CSS nesting och logiska CSS-egenskaper
- Självhostade typsnitt och optimerade WebP-bilder
- Formulär med inbyggd HTML-validering och visuell återkoppling i CSS
- Gemensam navigation och footer
- Anpassade hover- och fokuslägen
- `Formulärets validering sker helt genom HTML och CSS. Projektet saknar backend och recepten varken sparas eller publiceas`

## Testning

Projektet har testats med både automatiserade verktyg och manuell interaktion.

| Testverktyg / metod    | Resultat                                 |
| ---------------------- | ---------------------------------------- |
| WAVE                   | Inga rapporterade fel                    |
| W3C HTML Validator     | Samtliga sidor validerar utan fel        |
| Tangentbordsnavigation | Manuellt testad                          |
| Skärmläsare            | Manuellt testad                          |
| Responsivitet          | Manuellt testad vid olika skärmstorlekar |

## Changelog - Vecka 4

- [x] Skapat formulärsida för att dela recept
- [x] Semantisk gruppering av formulärfält med `fieldset` och `legend`
- [x] Responsiv formulärlayout med CSS grid och flexbox
- [x] Formulärvalidering med `:user-valid` och `:user-invalid`
- [x] Synliga felmeddelanden med `:has()`
- [x] Kopplat felmeddelanden till formulärfält med `aria-describedby`
- [x] Refaktorerat färgpaletten från HEX till OKLCH
- [x] Sidor använder `aria-current` på länkar i nav
- [x] Finslipat formulärets visuella uttryck och fokusmarkeringar
- [x] Genomfört tillgänglighets-, validerings- och prestandatester

## Changelog - Vecka 3

- [x] Skapat startsida med kategorier och receptkort
- [x] Gemensam navigation och footer
- [x] Flexbox för navigation och kategorier
- [x] CSS grid för startsidans hero
- [x] Responsiva receptkort med `auto-fit` och `minmax()`
- [x] Kolumner för ingredienser och instruktioner
- [x] Gemensam token för hero height

## Changelog - Vecka 2

- [x] Designsystem med reset och tokens
- [x] Självhostade Google typsnitt (Chewy + Atkinson Hyperlegible)
- [x] Ingredienslista använder :has() och stryks över när man bockar av dem.
- [x] Hover- och fokuslägen är tydliga(re).
- [x] Uppdaterat färgschema, favicon, site manifest

- `Atkinson Hyperlegible: Utvecklat av Braille Institute i USA med syftet att göra enskilda bokstäver och tecken lättare att känna igen och skilja från varandra.`

## Checklista - Vecka 1

- [x] Hårdkodade storlekar på bilder så att inget "layout shift" upplevs
- [x] delade upp innehållet i varsin `section` med **aria-labelledby** (och `id` på varje h2, ex. `ingredients-heading`). _Ingredienser_, _Så här gör du_ och _Serveringsförslag_ är tre separata delar med egna rubriker. Kopplingen ger varje sektion ett tillgängligt namn så att skärmläsare kan lista och hoppa mellan dem.
- [x] Checkbox för ingredienser. Varje checkbox ligger inuti en `label` som kopplar samman text och ruta utan att behöva använda `for` och `id`. Detta gör hela raden klickbar.
- [x] `role="list"` på ingrediens-listan då vissa skärmläsare (Safari/VoiceOver) kan strunta i att läsa elementet som en lista.
- [x] `figure` och `figcaption` för serveringsbilder. Bildtext som tillför information utöver bildernas egna `alt`-texter.

## Egna tankar

Under projektets fyra veckor har jag utvecklat min förståelse för semantisk HTML, modern CSS, responsiv design och tillgänglighet.

En viktig lärdom har varit hur ett genomtänkt designsystem gör återanvändbara tokens gör det mycket enklare att vidareutveckla och refaktorera en webbplats utan att behöva ändra på många enskilda komponenter.

Jag har även fått en bättre förståelse för CSS nesting, selectors, pseudoklasser och hur man kan skapa interaktivitet med HTML och CSS utan att använda Javascript.
