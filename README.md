# Projektjournal Fachblock 10 – SMB

## Inhaltsverzeichnis  
- [Einleitung](#einleitung)  
- [Verwendete Technologien](#verwendete-technologien)  
- [Funktionen](#funktionen)  
- [Mockup](#mockup)
- [UML-Klassendiagramm & Validation](#uml-klassendiagramm--validation)
- [Umsetzung](#umsetzung)

## Einleitung  
Ich dokumentiere in diesem Projektjournal die Entwicklung meiner Website, die ich im Rahmen des Fachblocks 10 erstellt habe.

## Verwendete Technologien  
- **C#** – Zur Programmierung der Applikation  
- **Figma** – Zur Skizzierung des Designs

## Funktionen  
- Interaktive Navigation  
- Bewertungssystem für Kurse

## Mockup  
Ich habe mithilfe von Figma ein Mockup erstellt, um das Design meiner Applikation zu planen. Hier ist ein Screenshot des Mockups:

![image](https://github.com/user-attachments/assets/f1429fbe-6a17-4f23-9f9e-ccf2b912c8ae)

Ich habe vier verschiedene Kurse erstellt, die jeweils eine eigene Seite besitzen. Diese Seiten sind über die Navigation erreichbar. Die Kurse sind: *Wandern für Anfänger*, *Survival-Training*, *Bogenschiessen* und *Kräuterwanderung*.

Zusätzlich habe ich eine Seite zur Bewertung der Kurse erstellt. Die Kurse können mit einem Sternchen-System bewertet werden. Optional kann man auch einen Kommentar und seinen Namen hinterlassen.

Beim Skizzieren des Designs habe ich darauf geachtet, dass die Seiten übersichtlich gestaltet sind und die wichtigsten Informationen schnell gefunden werden können.

Link zum Mockup: [Figma Mockup](https://www.figma.com/proto/xDM8tOmfVx6oGUaGwT0ljC/MoodTracker_Mockup?node-id=4-112&p=f&t=BgtEZogCLrswh6zW-1&scaling=scale-down&content-scaling=fixed&page-id=0%3A1)

## UML-Klassendiagramm & Validation


## Umsetzung  
Ich habe die bereitgestellte JSON-Datei überarbeitet, da ich meine eigenen Kurse erstellt habe.
```
{
  "courses": [
    {
      "name": "Wandern für Anfänger (ab 12)",
      "description": "Geführte Einsteigerwanderungen mit Tipps zu Ausrüstung, Orientierung und Sicherheit im Gelände.",
      "location": "Eingang Hauptgebäude",
      "date": "2025-07-09",
      "time": "08:00 - 15:30",
      "age": "12",
      "materials": "Rucksack, Wanderschuhe, eine Flasche Wasser, etwas zum Grillen, gute Laune",
      "feedback": {
        "enabled": true,
        "type": "rating",
        "hint": "Bewerten Sie den Kurs mit 1 bis 5 Sternen."
      },
      "rating": null,
      "rating_timestamp": null,
      "comment": null
    },
    {
      "name": "Survival-Training (ab 16)",
      "description": "Lernen, wie man ohne moderne Hilfsmittel in der Natur überlebt. Feuer machen, einen Unterschlupf bauen und Wasser finden.",
      "location": "Eingang Hauptgebäude",
      "date": "2025-07-11",
      "time": "08:00 - 15:30",
      "age": "16",
      "materials": "Rucksack, Wanderschuhe, eine Flasche Wasser, etwas zum Grillen, Messer",
      "feedback": {
        "enabled": true,
        "type": "rating",
        "hint": "Bewerten Sie den Kurs mit 1 bis 5 Sternen."
      },
      "rating": null,
      "rating_timestamp": null,
      "comment": null
    },
    {
      "name": "Bogenschiessen (ab 10)",
      "description": "Einführung in traditionelles Bogenschiessen in Wald- oder Feldumgebung.",
      "location": "Eingang Hauptgebäude",
      "date": "2025-07-10",
      "time": "13:15 - 15:30",
      "age": "10",
      "materials": "eine Flasche Wasser",
      "feedback": {
        "enabled": true,
        "type": "rating",
        "hint": "Bewerten Sie den Kurs mit 1 bis 5 Sternen."
      },
      "rating": null,
      "rating_timestamp": null,
      "comment": null
    },
    {
      "name": "Kräuterwanderung (ab 8)",
      "description": "Geführte Tour durch Wald und Wiese mit Fokus auf essbare Wildkräuter und deren Anwendung.",
      "location": "Eingang Hauptgebäude",
      "date": "2025-07-01",
      "time": "08:00 - 11:45",
      "age": "8",
      "materials": "Rucksack, Wanderschuhe, eine Flasche Wasser",
      "feedback": {
        "enabled": true,
        "type": "rating",
        "hint": "Bewerten Sie den Kurs mit 1 bis 5 Sternen."
      },
      "rating": null,
      "rating_timestamp": null,
      "comment": null
    }
  ]
}
```


Dann habe ich es in meiner App umgesetzt. Die App liest die Kurse aus der JSON-Datei aus, wandelt sie in Objekte um und zeigt sie automatisch in der Oberfläche an, sobald das ViewModel geladen wurde. Änderungen in der JSON-Datei werden nach einem Neustart der App übernommen.

![image](https://github.com/user-attachments/assets/b815346e-7a81-4fbe-b411-6685c6c64444)



