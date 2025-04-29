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



---
layout: default
transition: slide-left
hideInToc: true
---

<!-- TODO: Info verdelen want het is te veel op een slide -->
<!-- TODO: Stijl aanpassen zodat het bij de rest hoort -->
<!-- TODO: Info op de slide aanpassen -->

# Computer Vision voor Afvalherkenning

<div class="grid grid-cols-2 gap-6">
<div>

## Project Overzicht
- **Doel**: Automatisch herkennen van afvaltypes en sluikstort
- **Technologie**: SAP AI Core met Computer Vision Package
- **Dataset**: Getraind op afbeeldingen van verschillende afvaltypes
- **Integratie**: Verbonden met IVAGO's rapportage- en opvolgingssysteem

## Workflow
1. Foto maken van afval/sluikstort
2. Automatische analyse door CV model
3. Classificatie van afvaltype
4. Suggestie van gepaste opvolgingsactie
5. Rapportage aan juiste afdeling

</div>
<div>

## Technische Implementatie
- SAP AI Core voor modelhosting
- SAP HANA Cloud als data-opslag
- UI5-applicatie voor gebruikersinterface
- CAP (Cloud Application Programming) voor backend

<div class="bg-gradient-to-br from-[#5A32C8] to-[#9F89D7] p-4 rounded-lg text-white mt-4">
  <h3 class="text-lg mb-2">Voordelen</h3>
  <ul class="space-y-1 opacity-90">
    <li>⏱️ Snellere verwerking van meldingen</li>
    <li>🎯 Accurate classificatie (>90% nauwkeurigheid)</li>
    <li>📊 Betere data voor trendanalyse</li>
    <li>🔄 Automatisering van routinetaken</li>
  </ul>
</div>

</div>
</div>

---
layout: image-right
image: https://user-images.githubusercontent.com/1381301/66535560-d3422200-eace-11e9-9123-5535d469db19.png
transition: slide-left
---

<!-- TODO: Info aanpassen -->

# Demo: Afvalherkenning

## Model Training & Performance

- Getraind op **2000+ afbeeldingen** van sluikstort
- Onderscheidt **8 verschillende afvaltypes**:
  - Huishoudelijk afval
  - Bouwafval
  - Groenafval
  - Elektronisch afval
  - Plastic
  - Meubels
  - Gevaarlijk afval
  - Gemengd afval

## Uitdagingen
- Variabele lichtomstandigheden
- Gedeeltelijk zichtbaar afval
- Meerdere afvaltypes in één beeld
- Seizoensgebonden variaties

---
layout: default
transition: slide-left
hideInToc: true
---

<!-- TODO: Info aanpassen -->
<!-- TODO: Info verdelen want het is te veel op een slide -->

# Technische Architectuur

<div class="grid grid-cols-2 gap-6">
<div>

## Frontend Components
- **UI5 Framework** voor gebruikersinterface
- **Camera API** voor afbeeldingscapture
- **Report Service** voor meldingsbeheer
- **Location Service** voor geo-tagging

```typescript
// Voorbeeld: AttachmentService
export class AttachmentService {
  async uploadImage(file: File): Promise<string> {
    // Stuurt afbeelding naar backend voor analyse
    const formData = new FormData();
    formData.append('file', file);
    
    const response = await fetch('/api/upload', {
      method: 'POST',
      body: formData
    });
    
    return response.json();
  }
  
  // ...bestaande code...
}
```

</div>
<div>

## Backend Components
- **CAP Service** voor API-endpoints
- **AI Core Connector** voor modelintegratie
- **HANA Persistence** voor dataopslag

```javascript
// Voorbeeld: Computer Vision integratie in service.js
const cds = require('@sap/cds');
const aiCore = require('@sap/ai-core-sdk');

module.exports = cds.service.impl(async function() {
  this.on('analyzeImage', async(req) => {
    const { imageId } = req.data;
    
    // Haal de image data op
    const image = await SELECT.one.from('Images')
      .where({ ID: imageId });
    
    // Stuur naar AI Core voor analyse
    const prediction = await aiCore.predict({
      deploymentId: 'waste-recognition-model',
      data: image.content
    });
    
    // Verwerk resultaten
    return transformPrediction(prediction);
  });
});
```

</div>
</div>