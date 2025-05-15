# Telco Klantverloop Analyse (Churn Analyse)

Een datagedreven analyse van klantverloop (churn) bij een telecombedrijf op basis van klantsegmentatie en AI-gestuurde inzichten.

##  Projectoverzicht

Deze repository bevat een end-to-end analyse van klantverloop bij Telco, inclusief:

- Data-preprocessing en feature engineering
- Klantsegmentatie op basis van tenure, contracttype, leeftijd en technologiegebruik
- Berekening van churn-ratio’s per segment
- Toepassing van churn-voorspellingsmodellen
- AI-gestuurde interventiestrategieën (use case: jong & senior klantprofielen)

##  Doelstellingen

- Begrijpen welke klantgroepen het meest churn-gevoelig zijn
- Segmenten met een hoog risico identificeren
- Praktische aanbevelingen doen op basis van AI-inzichten
- Strategische acties simuleren (zoals gepersonaliseerde campagnes)

##  Dataset

- Bron: Anonieme Telco klantendataset
- Aantal rijen: 7.044 klanten
- Belangrijke variabelen: `tenure`, `contract`, `monthly charges`, `churn`, `tech services`

##  Data Voorbereiding

- Leeftijdsgroepen (`SeniorCitizen`) omgezet naar `J` (Jong) en `S` (Senior)
- Tenure gecategoriseerd in: `0–6`, `7–16`, `17+` maanden
- Contracttypes hernoemd: `MM` (Maand tot Maand), `OY`, `TY`
- Nieuwe variabele: Technologiegebruik (gebruikt ten minste één digitale dienst)
- Samengestelde segmentvariabele: `Customer Profile Segment`

##  Segmentatie & Churn Analyse

- Churn-ratio berekend per klantsegment
- Voorbeeld: Segment `J-7-16-MM-teknologisch` → churn-rate van **41%**
- Inzicht: Maandcontracten en korte loyaliteit (tenure) verhogen churn-risico

##  AI Use Cases

### Case 1: Jong, 7–16 maanden, maandcontract, gebruikt technologie
- Churn risico: Hoog
- AI-aanpak: Targeted social media-data, gepersonaliseerde databundels, digitale communicatie

### Case 2: Senior, 0–6 maanden, geen technologiegebruik
- Churn risico: Zeer hoog
- AI-aanpak: Belcampagnes, gedrukte brochures, gesimplificeerde factuuruitleg


##  Belangrijkste Inzichten

- Technologiegebruik alleen is geen garantie tegen churn
- Contracttype en tenure zijn kritieke factoren
- AI-interventies helpen bij het behouden van specifieke doelgroepen

