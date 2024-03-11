# UpgradeVerlichtingsysteem

## Inhoudsopgave

- [UpgradeVerlichtingsysteem](#upgradeverlichtingsysteem)
  - [Inhoudsopgave](#inhoudsopgave)
  - [Doel](#doel)
  - [Team](#team)
  - [Research](#research)
  - [Hardware](#hardware)
  - [Planning](#planning)
  - [BOM](#bom)
  - [Research document](#research-document)
  - [Github](#github)
  - [Powerpoint](#powerpoint)

## Doel
Het doel van het project is het aansturen van verschillende verlichtingspalen die momenteel niet voorzien zijn van bekabeling om aangestuurd te worden. De huidige oplossing is het rondrijden om de verlichting individueel aan te leggen. Op onderstaande foto is te zien over welke verlichtingspalen dit gaan met een gemiddelde afstand van 100m. Hiervoor zal een draadloze oplossing gezocht worden om deze verlichting via de huidige software aan te sturen.

## Team
De groep bestaat uit:
Elias Vanthorre, Xander Claessens, Robbe Verhelst

## Research
- Zigbee : heeft een range beperking waardoor we niet zullen kiezen voor zigbee 
- LoRa : LoRa (Long Range) is een draadloze communicatietechnologie die speciaal is ontworpen voor het Internet of Things (IoT). Het biedt een langeafstandsverbinding met een laag energieverbruik, waardoor het ideaal is voor toepassingen waarbij apparaten op grote afstand van elkaar moeten communiceren. In het context van het gegeven README-bestand wordt LoRa genoemd als een mogelijke technologie voor het aansturen van verlichtingspalen zonder bekabeling. LoRa kan worden gebruikt om draadloze communicatie tussen de verlichtingspalen en de besturingssoftware mogelijk te maken.
Een van de belangrijkste voordelen van LoRa is het bereik. Het kan signalen verzenden en ontvangen over grote afstanden, zelfs in omgevingen met obstakels zoals gebouwen of landschapskenmerken. Dit maakt het ideaal voor toepassingen zoals smart cities, waarbij apparaten verspreid zijn over een groot gebied.
Daarnaast heeft LoRa een laag energieverbruik, waardoor apparaten op batterijen langdurig kunnen werken zonder frequent opladen. Dit is vooral belangrijk voor IoT-toepassingen, waarbij apparaten vaak op afgelegen locaties worden geplaatst en het niet praktisch is om ze regelmatig van stroom te voorzien.
- UNIFI ISP: Unifi ISP biedt draadloze communicatieoplossingen, waaronder UISP (UniFi SmartPanel) 60 GHz draadloos en 5 GHz LTU (Long-Range) systemen, ontwikkeld door Ubiquiti Networks. De 60 GHz-band biedt hoge doorvoer en weinig interferentie, geschikt voor snelle gegevensoverdracht, terwijl de 5 GHz LTU-systemen een bereik van meer dan 30 km bieden. Demo-opstellingen tonen de benodigde apparatuur en geschatte kosten voor tests tussen locaties, zoals tussen Vives Xaverianenstraat en Vives (KU Leuven) Station, waarbij signaalsterkte, stabiliteit en weersbestendigheid worden geëvalueerd.

## Hardware
## Hardware

* LoRa

1. DLOS8N Outdoor LoRaWAN Gateway
<img src="./Documentatie/Foto's/gateway.jpg" alt="gateway" width="300">

2. LoRa Fiberglass Outdoor Antenna with SMA cable
<img src="./Documentatie/Foto's/Receiver.jpg" alt="Receiver" width="300">

3. Arduino MKR WAN 1310 - LoRa
<img src="./Documentatie/Foto's/arduino%20bord.jpg" alt="Arduino board" width="300">

4. SMA verloopkabel
<img src="./Documentatie/Foto's/kopeling.png" alt="SMA verloopkabel" width="300">

* UNIFI

1. LTU Rocket
<img src="./Documentatie/Foto's/LTU%20rocket.png" alt="LTU Rocket" width="300">

2. airMAX 5 GHz, 19/20 dBi Sector (AM-5G19-120)
<img src="./Documentatie/Foto's/antenne.png" alt="airMAX Antenna" width="300">

3. LTU Long-Range
<img src="./Documentatie/Foto's/LTU%20long%20range.png" alt="LTU Long-Range" width="300">

## BOM

* LoRa

| Beschrijving | Hoeveelheid | Prijs |
|--------------|-------------|-------|
| Gateway: DLOS8N outdoor LoRaWAN Gateway | 1 | [€249.95](https://www.antratek.be/dlos8n-outdoor-lorawan-gateway) |
| Receiver: LoRa fiberglass outdoor antenna with SMA cable | 6 | [€234.00](https://www.antratek.be/lora-fiberglass-outdoor-antenna-with-cable) |
| Controllers receiver: recBordje van lora arduino. | 6 | [€239.40](https://www.antratek.be/arduino-mkr-wan-1310-lora) |
| Convert cable. | 6 | [€26.52](https://www.allekabels.be/delock/6335/3387497/sma-verloopkabel.html?mc=nl-be&gad_source=1&gclid=CjwKCAiAlcyuBhBnEiwAOGZ2SwqTmJM-ptgAfea0Q5WTqEbYEkizDlHECH-4VB8BJi3uLMKrc6mXbBoC-k8QAvD_BwE) |
| **Total Price** | - | **€749.87** |


* UNIFI ISP

| Beschrijving | Hoeveelheid | Prijs |
|--------------|-------------|-------|
| Transmitter LTU Rocket | 1 | [€369](https://eu.store.ui.com/eu/en/collections/uisp-wireless-ltu-5-ghz-basestation/products/ltu-rocket) |
| LTU long Range | 6 | [€714](https://eu.store.ui.com/eu/en/collections/uisp-wireless-ltu-5-ghz-client-long-range/products/ltu-lr) |
| airMAX 5 GHz, 19/20 dBi Sector | 1 | [€128](https://eu.store.ui.com/eu/en/collections/uisp-wireless-antennas-sector/products/am-5g2?variant=am-5g19-120) |
| **Total Price** | - | **€1211** |

## Planning

Sprint 1: (Week 1 tot 3)
- Brainstormen en conceptideeën vormen
- Testen en kleine prototypes maken om tot een basisconcept te komen
- Opstellen van een architectuurdocument en checklist voor testen
- Definitief architectuurdocument met testresultaten die de keuzes van componenten onderbouwen
- Bestellijst maken met benodigdheden voor de eerste prototypes

Sprint 2: (Week 4 tot 6)
- Opstellen van een checklist voor het testen van de prototypes
- Bouwen van één of meerdere prototypes om de verschillende aspecten te testen
- Aanpassen van het architectuurdocument waar nodig en documenteren van testresultaten
- Werken naar een eerste werkend prototype van het uiteindelijke product

Sprint 3: (Week 7 tot 10)
- Overgang van de prototypefase naar het eindresultaat (finaal product of proof of concept)
- Testen van elk aspect van het product op functionaliteit en betrouwbaarheid en aanpassingen maken indien nodig
- Opstellen van een checklist voor het debuggen en testen van het eindresultaat

Sprint 4: (Week 11 tot 12)
- Gedetailleerd testen van het eindresultaat aan de hand van de checklist uit de vorige sprint
- Documenteren van alle testresultaten en optimalisaties doorvoeren waar nodig

Presentatie: (Week 13)
- Het presenteren van het gemaakte project aan de volledige opleiding met een vragen moment op het einde.

## Research document

https://docs.google.com/document/d/1G3bZLvqTwI6046OEOXTlWncNH4yMNufj9Are0H7HTGQ/edit?usp=sharing 

## Github

https://github.com/vives-project-xp/UpgradeVerlichtingsysteem


## Powerpoint

https://vivesonline-my.sharepoint.com/:f:/g/personal/r0937303_student_vives_be/Etcbu2drZYJPig6IPUDJIq0BVEMRaauK4c4SZp-p5Y8hbA?e=eQiQK8 
