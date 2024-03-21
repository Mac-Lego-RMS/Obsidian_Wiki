---
Owner: FFlorian Hoos
tags:
  - Programmierung
Last edited time: 2024-02-26T13:27
---
Github ist eine Cloudplattform von Microsoft, die die Nutzung von GIT im Team streamlined.

# Repository

Repositories funktionieren wie Ordner. Hier werden die tatsächlichen Dateien gespeichert, mitsamt ihrer Ordnerstruktur.

# Organisationen

Mithilfe von Organisationen können mehrere Github-Nutzer auf ein oder mehrere Repositories zugreifen.

# Funktionen von Git/Github:

## Fetch

Mit Fetch wird ein Repository mitsamt sämtlicher Branches heruntergeladen.

## Branch

Erstellt einen Snapshot vom aktuellen Branch. Alle Änderungen, die auf dem neuen Branch passieren, haben keine Auswirkungen mehr auf den vorigen Branch.

## Commit

Hat man ein Ziel erreicht, eine Funktion implementiert oder ist sonstwie fertig mit seinen Arbeiten, kann man einen _Commit_ erstellen. Auch hier wird ein Snapshot der aktuellen Dateien erstellt. Der Commit hat eine ID, einen Namen und eine Beschreibung. Man sollte hier die Änderungen beschreiben und erklären.

## Push

Mit Push wird die lokale Version des Repositories inklusive aller Branches in die Cloud "geschoben". Dabei muss darauf geachtet werden, dass die Änderungen keine Konflikte mit dem jeweiligen Branch verursachen. Daher sollte in den meisten Fällen jeder Programmierer seinen eigenen Branch haben.

## Pull Request

Sind alle Änderungen in einem Branch implementiert und getestet, können sie durch das Erstellen einer Pull Request in den `main`-Branch eingeknüpft werden. Dabei können explizit Nutzer erwähnt werden, die diese Änderungen übersehen sollen.

## Merge

Ist die Pull Request erfolgreich, kann nun der fertige Code aus dem Branch mit dem `main`-Branch gemerged werden.

# Github im RMS Robotik Team

Unsere Github-Organisation heißt [Mac-Lego-RMS](https://github.com/Mac-Lego-RMS). Wir haben nach einer gründlichen Aufräumaktion aktuell 4 aktive Repositories:

- [Spike_Python](https://github.com/Mac-Lego-RMS/Spike_Python) - hier befinden sich alle aktuellen Programme
- [3D-Model](https://github.com/Mac-Lego-RMS/3D-Model) - hier liegt das [Stud.io](http://stud.io/) CAD-Modell des Roboters
- [robot-design](https://github.com/Mac-Lego-RMS/robot-design) - hier liegt die RobotDesign-Präsentation
- [Forschungsprojekt](https://github.com/Mac-Lego-RMS/Forschungsprojekt) - hier ist manchmal die neue PPP zu finden

# Arbeiten mit Github / _Loki Laufeyson als Programmierer_

Git basiert auf Branches (Zweigen). Dabei gibt es einen `main`-Branch, der mit der _sacred timeline_ aus Loki verglichen werden kann.  
Wenn ein Programmierer arbeitet, erzeugt er vorher sein eigenes  
_Nexus event_ und befindet sich ab dann auf einer _branched timeline_ - bzw. einem Branch/Zweig, wie es auf Github heißt. Der Programmierer hat nun das neue Feature fertiggestellt und einen Commit  
Das Programmieren mit Github lässt sich sehr gut mit der Show  
_Loki_ vergleichen. Es geht wie folgt:

## Nexus Event

Der Programmierer befindet sich anfangs auf dem `main`-Branch - vergleichbar mit der _Sacred Timeline_. Jetzt erzeugt er einen _Branch_. So wie ein _Nexus Event_ wird durch das Erstellen eines Branches eine Momentaufnahme des Repositories erstellt, die sich ab dann unabhängig von der _Sacred Timeline_ weiterentwickelt (bzw. dem `main`-Branch).

## Branched Timeline

Alle Änderungen, die auf dem Branch stattfinden, haben keinerlei Auswirkungen auf die _Sacred Timeline_ bzw. den `main`-Branch. Hier kann der Programmierer ungestört von der _TVA_ programmieren, ohne sich vor einem _Pruning_ fürchten zu müssen.

## God of Stories

Ist der Programmierer fertig mit seinen Änderungen, erstellt er einen `Commit`. Er erklärt die Änderungen, die er in die _Sacred Timeline_ einbringen möchte.  
Anders als in Staffel 1 hat jetzt  
_Loki_ als _God of Stories_ die Möglichkeit, die Zweige der Entwickler zu verspinnen. Wird eine _Pull Request_ bestätigt, können die Änderungen aus der _Branched Timeline_ in die _Sacred Timeline_ übernommen werden (also in den `main`-Branch)