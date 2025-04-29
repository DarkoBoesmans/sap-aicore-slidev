---
layout: default
transition: slide-left
---

# SAP AI Core: Capacity Units

<div class="flex flex-col justify-center">
  <p class="mb-4">SAP AI Core werkt met een Capacity Unit (CU) model voor kostenberekening en resourcetoewijzing.</p>
</div>

<div class="grid grid-cols-1 gap-6">
<div>

## Kostencomponenten: Instances

- Computationele kracht voor model training en inferentie
- Berekend per Node Hours per Month
- Kosten variëren op basis van CPU/GPU configuratie

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# SAP AI Core: Storage Costs

<div class="grid grid-cols-1 gap-6">
<div>

## Storage

- Standard SSD Volumes voor data en modelopslag
- Berekend als **0.0003 CU / GB / Hour**
- Belangrijk voor:
  - Trainingsdata
  - Model artifacts
  - Resultaten en logs

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# SAP AI Core: Baseline kosten

<div class="grid grid-cols-1 gap-6">
<div>

## Vaste clusterresources

- **1.2241 CU / Hour** voor basisinfrastructuur
- Onafhankelijk van workload en gebruik
- Benodigd voor orchestratie en beheer
- Wordt gedeeld over alle workloads in het cluster

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# SAP AI Core: Kostenoptimalisatie

<div class="grid grid-cols-1 gap-6">
<div>

## Strategieën voor optimaal gebruik

- Schaalbaarheid op basis van projectbehoeften
- Training versus inferentie resources
- Levenscyclusbeheer voor ongebruikte resources
- Gedeelde resources binnen subaccounts
- Batch processing voor efficiënt gebruik

</div>
</div>

---
layout: default
transition: slide-left
---

# SAP Generative AI Hub

<div class="grid grid-cols-1 gap-6">
<div>

## Inleiding

- Gespecialiseerde kostenberekening voor generatieve AI
- Ontworpen voor LLM toepassingen en generatieve modellen
- Eenvoudiger prijsmodel vergeleken met standard AI Core
- Focus op API-interacties in plaats van infrastructuur

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# Generative AI Hub: Kostencomponenten

<div class="grid grid-cols-1 gap-6">
<div>

## Requests (0.0048 CU/maand)

- Berekend op basis van tokengebruik
- Afhankelijk van het geselecteerde model
- Input en output tokens worden apart berekend
- Gebaseerd op gebruik per maand

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# Generative AI Hub: Orchestration

<div class="grid grid-cols-1 gap-6">
<div>

## Orchestration (0.0007 CU/maand)

- Coördinatie van AI-stromen
- Text Blocks orchestratie
- Controle en beheer van model-interacties
- Aansturing van meerdere AI-diensten

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# Generative AI Hub: Kostencalculatie

<div class="grid grid-cols-1 gap-6">
<div>

## Instructions Section

- Definitie van tokens per request
- Selectie van beschikbare modellen
- Bepaling van frequentie per maand

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# Generative AI Hub: Specificaties

<div class="grid grid-cols-1 gap-6">
<div>

## Model configuratie

- Model selectie (naam en versie)
- Input tokens configuratie
- Output tokens instelling
- Gebruik per maand

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# Generative AI Hub: Totale kosten

<div class="grid grid-cols-1 gap-6">
<div>

## Kostenoverzicht

- Cumulatief: **0.0055 CU per maand**
- Transparante uitsplitsing componenten
- Betalen naar gebruik (pay-as-you-go)
- Voorspelbare kostenstructuur

</div>
</div>

---
layout: default
transition: slide-left
---

# Vergelijking: Toepassingsgebieden

<div class="grid grid-cols-2 gap-6">
<div>

## Standard AI Core: Focus

- Algemene AI-workloads
- Model training & deployment
- Computer Vision toepassingen
- Predictive analytics
- Custom model ontwikkeling

</div>
<div>

## Generative AI Hub: Focus

- Specifiek voor generatieve AI
- LLM toepassingen
- Text-to-text, text-to-image
- Chatbots en assistenten
- Content generatie

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# Vergelijking: Kostenmodellen

<div class="grid grid-cols-2 gap-6">
<div>

## Standard AI Core

- Instance-gebaseerd (CPU/GPU)
- Storage kosten (0.0003 CU/GB/Hour)
- Vaste clusterkosten (1.2241 CU/Hour)
- Geoptimaliseerd voor rekenintensieve taken

</div>
<div>

## Generative AI Hub

- Token-gebaseerd prijsmodel
- Request-georiënteerd (0.0048 CU/maand)
- Orchestration kosten (0.0007 CU/maand)
- Geoptimaliseerd voor API-interacties

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# Keuze: Standard AI Core vs. Generative AI Hub

<div class="mt-4 p-4 bg-gradient-to-br from-[#5A32C8]/10 to-[#9F89D7]/10 rounded-lg">
  <h3 class="text-xl font-bold mb-3">Wanneer kies je welke calculator?</h3>
  
  <div class="grid grid-cols-2 gap-4">
    <div>
      <h4 class="text-lg font-bold mb-2">Standard AI Core</h4>
      <ul class="space-y-2">
        <li>Voor custom model training</li>
        <li>Computer Vision projecten</li>
        <li>Machine Learning workflows</li>
        <li>Predictive analytics</li>
      </ul>
    </div>
    
    <div>
      <h4 class="text-lg font-bold mb-2">Generative AI Hub</h4>
      <ul class="space-y-2">
        <li>Voor chatbot applicaties</li>
        <li>LLM-gebaseerde toepassingen</li>
        <li>Content generatie</li>
        <li>Text-to-image conversie</li>
      </ul>
    </div>
  </div>
</div>