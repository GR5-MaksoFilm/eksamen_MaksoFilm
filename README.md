# Teknisk dokumentation for Gruppe 5 – 2. Semester eksamensprojekt

Herunder er der dokumentation der fastsætter regler for hvordan projektet kodes så der er et fælles udgangspunkt i syntax og navngivning, for at holde koden ensartet og effektiv. Dette gør også problemløsning og det overordnede visuelle udtryk lettere at vedligeholde.

## Projektstruktur:

Der arbejdes i Astro og derfor bruger vi også Astros egen filstruktur med vores egne tilføjede mapper og filer.
• Elementer der går igen bygges som components
• Fonte, farver og lignende laves som variables i global.css
• Billeder, video og andre tungere resourcer placeres i assets under src og importeres gennem Astro

## Navngivning:

• Alle filer og mapper navngives i lowercase, dog med undtagelse for Astro Layouts og Components
• Der bruges ingen mellemrum i navngivning, i stedet navngives filer som fx ”style_index.css” dette eksempel er for CSS specifikt til forsiden
• Filer der hører specifikt til bestemte sider navngives også som ovenfor med ”filfunktion_side.filtype”

## Link til scripts:

• Eventuelle scripts placeres i bunden af dets respektive component eller page

## Git branches:

• Branchens navngives som følgende eksempel ”feature_navn"

## Arbejdsflow:

• INGEN arbejder i main, medmindre det er aftalt på forhånd
• INGEN merger deres branch ind i main før det er godkendt
• Commit messages skal være beskrivende omkring hvad der er tilføjet og/eller fjernet, brug eventuelt CoPilot til at navngive commits

## Kode:

• Eventuelle funktioner i JS laves som arrow functions
• Der bruges class selector til CSS af elementer der navngives ”klassens-funktion_beskrivelse” som fx ”grid_none-to-3” for et layout der går fra intet grid til column af 3
• Der bruges id selector til elementer der skal påvirkes af eventuel JS´
• CSS laves i hvert dokument i et <style> tag, global CSS laves i global.css dokumentet der findes i styles mappen

# Funktionalitet

• Der hentes data til portfolio gennem API til en database lavet med Supabase
• Dynamisk visning af enkelte elementer fra portfolio

Dette afsnit skal forklare hvad I konkret har arbejde med, for at udvikle websitet. Tænk over hvilke interaktioner brugeren kan foretage på sitet? Eller hvordan websitet håndterer og præsenterer data? Eksempler på funktionalitet, der kan beskrives:

- Hentning af produkter fra API.
- Filtrering af produkter baseret på brugerens valg.
- Dynamisk visning af produkter i HTML.

Brug korte beskrivelser, som i eksemplerne herover

/////////////////////////////////////////////////////////////////////////////////

# API endpoints

Dette afsnit skal liste de endpoints fra API'et i har benyttet:

- (fx. https://dummyjson.com/products)

# Dokumentation af Funktion

Dette afsnit skal beskrive en funktion I selv har udviklet. Det kunne eksempelvis være en funktion der generere en listen over fx. produkter:

- Beskrivelse: Hvad gør funktionen? Hvordan spiller den sammen med resten af koden?
- Parametre: Hvilke input forventes (fx en værdi fra en dropdown eller URL'en)?
- Returnerer: Beskriv, om funktionen returnerer en værdi eller blot manipulerer DOM’en.
- Eksempel på brug: Indsæt funktions-koden herunder(der hvor koden er i eksemplet) og vis, hvordan funktionen kaldes:

```javascript
//funktionens kode:
function voresFunktion(sprog) {
  console.log(`${sprog} syntax highlighting`);
}
//hvordan funktionen kaldes:
voresFunktion("JavaScript");
```
