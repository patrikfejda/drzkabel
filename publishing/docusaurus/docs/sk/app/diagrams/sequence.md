---
title: Sequence diagram
sidebar_label: Sequence
---

# Sequence diagram

Scenár: „Používateľ získa odporúčania na uloženie káblov pre nový stôl“

Sekvencia:
1. Používateľ vyplní konfiguráciu nového pracovného miesta v Mobile App
2. Aplikácia pošle na Backend Service požiadavku `CreateWorkspace(configData)`
3. Backend uloží dáta, vygeneruje `workspaceId` a spustí `GenerateRecommendations`
4. Recommendation Engine načíta detaily pracovného miesta a vypočíta odporúčania (plánovanie, checklist)
5. Backend vráti do aplikácie „Recommendations + DiagramData“
6. Používateľ si pozrie odporúčania a uloží setup (voliteľne synchronizuje)

![Sequence diagram](/img/app/diagram-sequence.png)

---
**Navigation:** [⬆️ Up](../index.md) · [🏠 Home](/sk)


