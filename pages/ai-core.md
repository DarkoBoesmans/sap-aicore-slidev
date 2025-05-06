---
layout: section
transition: slide-left
hideInToc: true
---

## AI Core

<!-- 
  Darko
-->

---
layout: default
transition: slide-left
---

# SAP AI Core: Kostenstructuur

<div class="grid grid-cols-2 gap-6">
<div>

## Capacity Units (CU)
- Computationele kracht voor training/inferentie
- Berekend per Node Hours per Month
- Kosten variëren op basis van CPU/GPU configuratie

</div>
<div>

## Storage Costs
- Standard SSD Volumes voor data en modelopslag
- Berekend als **0.0003 CU / GB / Hour**
- Voor trainingsdata, model artifacts, logs

</div>
</div>

---
layout: default
transition: slide-left
hideInToc: true
---

# SAP AI Core: Baseline & Optimalisatie

<div class="grid grid-cols-2 gap-6">
<div>

## Vaste clusterresources
- **1.2241 CU / Hour** voor basisinfrastructuur
- Onafhankelijk van workload en gebruik
- Benodigd voor orchestratie en beheer
- Wordt gedeeld over alle workloads

</div>
<div>

## Optimalisatiestrategieën
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

<div class="grid grid-cols-2 gap-6">
<div>

## Inleiding & Requests
- Gespecialiseerd voor generatieve AI
- Eenvoudiger prijsmodel dan standard AI Core
- **Requests**: 0.0048 CU/maand
- Berekend op basis van tokengebruik
- Input en output tokens apart berekend

</div>
<div>

## Orchestration & Specificaties
- **Orchestration**: 0.0007 CU/maand
- Coördinatie van AI-stromen
- Text Blocks orchestratie
- Model selectie (naam en versie)
- Input/output tokens configuratie

</div>
</div>

---
layout: default
transition: slide-left
---

# Vergelijking: Toepassingsgebieden & Kostenmodellen

<div class="grid grid-cols-2 gap-6">
<div>

## Standard AI Core
- **Focus**: Algemene AI-workloads, training & deployment
- **Kostenmodel**: Instance-gebaseerd (CPU/GPU)
- Storage kosten (0.0003 CU/GB/Hour)
- Vaste clusterkosten (1.2241 CU/Hour)
- Geoptimaliseerd voor rekenintensieve taken

</div>
<div>

## Generative AI Hub
- **Focus**: Specifiek voor generatieve AI, LLM toepassingen
- **Kostenmodel**: Token-gebaseerd
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

<div class="grid grid-cols-2 gap-6">
<div>

## Standard AI Core
- Voor custom model training
- Computer Vision projecten
- Machine Learning workflows
- Predictive analytics
- Wanneer infrastructuurbeheer belangrijk is

</div>
<div>

## Generative AI Hub
- Voor chatbot applicaties
- LLM-gebaseerde toepassingen
- Content generatie
- Text-to-image conversie
- Wanneer eenvoud en API-focus belangrijk is

</div>
</div>

---
layout: default
transition: slide-left
---

# Prijsvoorbeelden (1 CU = €1,04)

<div class="grid grid-cols-2 gap-6">
<div>

## Standard AI Core Voorbeeld
- **Basisinfrastructuur**: 
  1,2241 CU/uur × 24 uur × 30 dagen × €1,04 = **€916,13/maand**
- **Training workload**: 
  GPU server (4 CU/uur) × 8 uur × €1,04 = **€33,28/dag**
- **Storage kosten**: 
  100GB × 0,0003 CU/GB/uur × 720 uur × €1,04 = **€22,46/maand**
- **Totale maandelijkse kosten**: 
  Basisinfrastructuur + Training + Storage = **±€971,87/maand**

</div>
<div>

## Generative AI Hub Voorbeeld
- **10.000 requests/maand**:
  10.000 × 0,0048 CU × €1,04 = **€49,92/maand**
- **Orchestration van 50.000 text blocks**:
  50.000 × 0,0007 CU × €1,04 = **€36,40/maand**
- **Totale maandelijkse kosten**:
  Requests + Orchestration = **€86,32/maand**
- **Kostprijs per request**:
  €86,32 ÷ 10.000 = **€0,00863 per request**
 
</div>
</div>