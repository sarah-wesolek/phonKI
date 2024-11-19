# phonKI

## Beschreibung
**phonKI** ist eine interne Website, die unsere Gruppe nutzen kann. Die Website wurde mit [Quarto](https://quarto.org) erstellt und wird über GitHub Pages gehostet.
**Ich bin noch dabei, rauszufinden, wie ich sie am besten hoste, so dass sie nur intern zugänglich ist**, aber ihr könnt schon daran arbeiten und die Website lokal öffnen.

---

## Installation und Website rendern
Um die Website lokal auszuführen oder Änderungen vorzunehmen, folgt diesen Schritten:

1. Repository klonen:
   ```bash
   git clone https://github.com/sarah-wesolek/phonKI.git
   cd phonKI

oder einfach, wie ich, mit [GitDesktop](https://desktop.github.com/download/) arbeiten...

2. [LaTeX](https://www.latex-project.org/get/) herunterladen und installieren, wenn nicht nicht erfolgt.
3. [Quarto](https://quarto.org) installieren, falls noch nicht erfolgt.
4. R-Projekt in R-Studio öffnen.
5. Tinytex-Dstribution installieren in R Konsole:
   ```bash
   install.packages("tinytex")
6. Pfad in *R Terminal* festlegen auf Unterordner *website*. In meinem Falle:
   ```bash
    cd /Users/sarahwesolek/Documents/phonKI/website
7. Website rendern
   ```bash
   quarto render

Öffne nun den den Ordner *_site* im Odner *website*, und klicke auf die Datei *index.html*, um die Website lokal anzusehen.

---
## Änderungen vornehmen
Um Änderungen vorzunehmen, öffne den Unterordner *notes* im Order *website*. Dort finden sich drei .qmd-Dokumente, die frei bearbeitet werden können/sollen.
1. *index.qmd* - für die Übersicht
2. *resources.qmd* - für die Ressourcen
3. *reports.qmd* - für die Meeting Berichte

Wenn du Änderungen vornimmst, speichere das jeweilige file mit cmd+s und gehe zur R-Studio Konsole, um es wieder zu rendern.
   ```bash
   quarto render

Du kannst nun wieder die Datei *index.html* öffnen, um die Website lokal anzusehen.

Wenn Du fertig bist, committe und pushe die Änderungen in das GitHub-Repository.
