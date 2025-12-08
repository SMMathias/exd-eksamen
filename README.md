# exd-eksamen

# EXD – Akvariespil (Forbedret eksamensversion)

Denne README giver et hurtigt overblik over de forbedringer, jeg har lavet i projektets filer frem mod eksamen. Fokus har været på datastruktur, UX-flow og spilfunktionalitet.

---

## index.html

Ingen ændringer fortaget

---

## style.css

Ingen ædringer fortaget

---

## script.js

Her ligger hoveddelen af forbedringerne i projektet:

### **Forbedring 1 – Samlet datastruktur**

- Samlet alle fisk i én datastruktur (`fishCards`) for at skabe konsistens.
- Fjernet gamle/uopdaterede properties (fx GIFs), så datastrukturen er ren og ensartet.
- Alt UI (modal, info-view, selection og gameplay) trækker nu fra samme datasæt.

### **Forbedring 2 – Ny top-view spilkarakter + playableImg**

- Tilføjet en ny property `playableImg` til datastrukturen (`fishCards`).
- Gameplay bruger nu et nyt top-view billede, mens modal/infoscreen stadig bruger side-view.
- Implementeret if/else fallback så spillet fungerer med eller uden playableImg.
- Justeret fiskens størrelse i canvas for bedre gameplay.

### **Forbedring 3 – Forbedret karaktervalg-flow**

- `selectedFishIndex` starter nu i en neutral state (`null`) i stedet for 0.
- Implementeret validation: brugeren kan ikke starte spillet uden et aktivt valg.
- Tilføjet UI-feedback via `.selected` class.
- Nulstilling af state, når brugeren går tilbage til menuen.

---

## figma prototype

- Redesignet modals og gjort dem til komponenter.
- Oprettet component-states for fisk (neutral og selected).
- Tilføjet Smart Animate transitions mellem frames.
- Lavet top-view figur til gameplay, så prototype og spil hænger sammen.
- Opbygget flow: Info → Selection → Gameplay → Game Over.

---

## Fokus for forbedringerne

- Et tydeligere og mere logisk UX-flow.
- Bedre state management i spillet.
- Mere konsistent datastruktur i JavaScript.
- Større sammenhæng mellem design (Figma) og kode (JavaScript).
