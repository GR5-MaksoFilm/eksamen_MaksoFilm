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

# API endpoints

• Vi har lavet vores database i Supabase. Herunder findes API url og key, som også findes under Card.astro component.

- url:
  https://uhcutojnbibslmplbwqd.supabase.co/rest/v1/Portfolio?select=*

- Key:
  eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InVoY3V0b2puYmlic2xtcGxid3FkIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NDc3Mjc5NTcsImV4cCI6MjA2MzMwMzk1N30.gUKjETMs5zvXh4Hhw059erhs-V19eoJSiUCNXidk-V0
