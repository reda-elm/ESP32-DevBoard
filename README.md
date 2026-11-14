# ESP32-DevBoard

Carte de développement ESP32 personnalisée conçue sur Altium Designer. Équipée d'une interface USB-série CH340G, d'une alimentation 3.3V et des boutons-poussoirs (BOOT/EN) pour la programmation.

<div align="center">
  <img width="400" alt="Aperçu de la carte ESP32" src="https://github.com/user-attachments/assets/495ce8d5-43ff-45a4-8411-2c77f6f63f3d" />
</div>

## Caractéristiques principales

* **Microcontrôleur :** Module ESP32-WROOM
* **Interface USB-Série :** CH340G avec oscillateur 12 MHz
* **Alimentation :** Régulateur LDO 3.3V (XC6222)
* **Programmation :** Boutons-poussoirs tactiles intégrés (BOOT et EN)
* **Conception :** Circuit imprimé à 2 couches routé sur Altium Designer

## Contenu du dépôt

* **`Altium/`** : Fichiers sources de conception (Schémas et routage PCB)
* **`Fabrication/`** : Fichiers Gerber et de perçage (NC Drill) générés pour JLCPCB
* **`BOM/`** : Bill of Materials(BOM) avec les numéros de pièces Mouser

## Plan de validation matériel 

Lors de la réception de la carte, les étapes de validation suivantes sont effectuées :
1. Inspection visuelle et tests de continuité (recherche de courts-circuits).
2. Vérification de la tension de sortie du régulateur 3.3V.
3. Test de l'énumération USB du pont CH340G sur l'ordinateur.
4. Programmation et téléversement d'un code de test via les boutons BOOT/EN.
5. Vérification du bon fonctionnement du Wifi et Bluetooth de l'ESP32.
