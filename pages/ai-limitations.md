---
layout: section
transition: slide-left
---

# Van Concept naar Realiteit

De evolutie van AI van theoretisch concept naar praktische toepassingen

---
layout: section
transition: slide-left
hideInToc: true
---

## De limitaties

---
layout: default
transition: slide-left
---

# Limitations van Generatieve AI

<div class="grid grid-cols-2 gap-6">
<div>

## Hallucinations
- AI genereert plausibele maar onjuiste informatie
- Voorbeeld: ChatGPT maakt foutieve samenvatting van een boek

```text
Prompt: Maak een korte samenvatting van het boek 
'Het verdriet van België' door Louis-Paul Boon.

ChatGPT 3.5: "Het verdriet van België" ("The Sorrow 
of Belgium") door Louis-Paul Boon is een 
semi-autobiografische roman...
```

- **Belangrijk**: Foundation Models weten niets, ze berekenen alleen waarschijnlijkheden

</div>
<div>

## Kennisbeperkingen
- Kennis bevroren op trainingsmoment
- Geen besef van actualiteit na trainingsdatum

```text
Prompt: Ik wil The Crooked House bezoeken, een 
historische 18e-eeuwse pub in Staffordshire. 
Wat moet ik weten?

ChatGPT 3.5: Een bezoek aan The Crooked House 
klinkt fantastisch! Hier is wat je moet weten: ...
```

- The Crooked House brandde af in 2023, maar ChatGPT 3.5 werd getraind tot januari 2022

</div>
</div>

---
layout: default
transition: slide-up
hideInToc: true
---

# Meer Beperkingen van AI

<div class="grid grid-cols-2 gap-6">
<div>

## Inconsistente Wiskundige Vaardigheden
- Moeite met eenvoudige berekeningen
- Verwarrende tijdsperceptie

```text
Prompt: Geef een woord met precies 3 b's, 2 a's en een e.

ChatGPT 3.5: Het woord "beanbag" voldoet aan je criteria: 
het heeft 3 b's, 2 a's en een e.
```

```text
Prompt: Wat gebeurde eerder: het zinken van The Herald 
of Free Enterprise of het 'Heizeldrama'?

ChatGPT 3.5: Het zinken van de Herald of Free Enterprise 
vond plaats op 6 maart 1987, terwijl het Heizeldrama 
plaatsvond op 29 mei 1985.
```

</div>
<div>

## Sterk in Standaardproblemen
- Goed in het oplossen van bekende vraagstukken
- Volgt aangeleerde methodieken

```text
Prompt: Twee auto's rijden noordwaarts. De eerste rijdt 
40 km/u, de tweede vertrekt 3 uur later en rijdt 60 km/u. 
Hoe lang na het vertrek van de tweede auto haalt deze 
de eerste in?

Bing Copilot: 
Laat T de tijd voorstellen die de eerste auto rijdt.
De tweede auto start 3 uur later, dus zijn tijd is (T - 3).
Afstand eerste auto: 40T kilometer.
Afstand tweede auto: 60(T - 3) kilometer.
40T = 60(T - 3)
40T = 60T - 180
-20T = -180
T = 9
Antwoord: 6 uur na vertrek tweede auto.
```

</div>
</div>
