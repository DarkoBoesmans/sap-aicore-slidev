---
layout: section
transition: slide-up
---

# AI binnen IVAGO

<div class="flex justify-center">
  <div class="text-center max-w-2xl">
    <p class="text-xl mt-4 opacity-80">
      Computer Vision voor afvalherkenning
    </p>
  </div>
</div>

<!-- 
  Darko
-->

<!-- TODO: Info verdelen want het is te veel op een slide -->
<!-- TODO: Stijl aanpassen zodat het bij de rest hoort -->
<!-- TODO: Info op de slide aanpassen -->

---
layout: image-right
image: https://images.unsplash.com/photo-1605600659908-0ef719419d41
transition: slide-left
hideInToc: true
---

# Afvalherkenning

## Project Overzicht
- **Doel**: Automatisch herkennen van afvaltypes
- **Technologie**: SAP AI Core & Computer Vision

## Huidige Workflow
1.	App stad Gent.
2.	SAP CRM bij stad Gent.
3.	Via CPI naar SAP Ivago.
4.	Beschikbaar in tcode ZW_CASEMANAGER.

---
layout: image-left
image: https://miro.medium.com/v2/resize:fit:1100/format:webp/1*lzQfAi97YH_Fs_GtdOBhNQ.png
transition: slide-left
hideInToc: true
---

# Technische Details

## Huidige Tutorial
Doorloop van de "Use Computer Vision Package to Train AI Model for Meter Reading" tutorial waarbij we een model trainen om automatisch meterstanden af te lezen van foto's.

- **SAP AI Core** met Computer Vision Package
- **Meter Reading Model** gespecialiseerd in cijferherkenning
- **SAP BTP** voor applicatie-hosting
- **CAP** voor gestructureerde data-integratie

---
layout: image-right
image: https://user-images.githubusercontent.com/1381301/66535560-d3422200-eace-11e9-9123-5535d469db19.png
transition: slide-left
---

<!-- TODO: Info aanpassen -->

# Afvalherkenning

- Getraind op afbeeldingen van sluikstort
- Onderscheidt **8 verschillende afvaltypes**:
  - Huishoudelijk afval
  - Bouwafval
  - Groenafval
  - Elektronisch afval
  - Plastic
  - Meubels
  - Gevaarlijk afval
  - Gemengd afval

<!-- 

## Uitdagingen
- Variabele lichtomstandigheden
- Gedeeltelijk zichtbaar afval
- Meerdere afvaltypes in één beeld
- Seizoensgebonden variaties

-->