# Personalausweis‑Prüfziffer‑Demo (7‑3‑1 Checksumme)

Dieses Projekt demonstriert die Berechnung von Prüfziffern nach dem 7‑3‑1‑Gewichtungsverfahren,
wie es in maschinenlesbaren Zonen (MRZ) von Ausweisdokumenten verwendet wird.
Es handelt sich um ein **reines Lern- und Demonstrationsprojekt** in HTML/JavaScript.

> **Hinweis zur Herkunft:**  
> Dies ist eine **fehlerbereinigte Version** des ursprünglich hier veröffentlichten Skripts:  
> http://jaaan.bplaced.net/Privat/Personalausweisgenerator_v1.2.html

## Funktionsumfang
- Generierung zufälliger Ziffernfolgen (z. B. Wohnsitz-Kennzahl, laufende Zahl, Geburtsdatum YYMMDD, Ablaufdatum YYMMDD).
- Berechnung und Prüfung der Prüfziffern mit dem **7‑3‑1‑Verfahren**.
- Formularoberfläche zur Eingabe und Validierung mit klaren Fehlermeldungen.
- Korrekte Datumshandhabung inkl. gregorianischer Schaltjahre.

## Zweck
- **Algorithmisches Lernen**: Verständnis der Prüfziffernberechnung mit wechselnden Gewichten.
- **Demonstration**: Einfache UI-Logik in Vanilla JavaScript.
- **Kein Praxisbezug**: Alle erzeugten Daten sind fiktiv und ohne amtliche Relevanz.

## Wichtiger Hinweis / Disclaimer
- Die erzeugten Nummern sind **keine echten Personalausweisnummern**.
- Der Code **dient ausschließlich zu Bildungs- und Demonstrationszwecken**.
- **Jegliche Nutzung zur Umgehung von Altersverifikationen, Identitätsprüfungen oder anderen Sicherheitsmechanismen ist illegal** (u. a. Betrug/Computerbetrug).
- Der Autor dieses Projekts distanziert sich ausdrücklich von jeder missbräuchlichen Verwendung.

## Verwendung
1. Dieses Repository herunterladen oder klonen.
2. `index.html` lokal im Browser öffnen.
3. Felder ausfüllen und über **„Generieren“** Nummern mit Prüfziffern erzeugen oder über **„Prüfen“** bestehende Eingaben validieren.

## Technische Details / Änderungen gegenüber dem Original
- Ersetzt veraltete `getYear()`-Verwendung durch `getFullYear()`.
- Korrigierte Monats- und Tageslogik (0-basierte Monate, gregorianische Schaltjahre, `daysInMonth`).
- Entfernt unsichere/nutzlose Teile (`eval`, unbenutzte Funktion `randd`, `with`-Blöcke).
- Strikte Ziffernvalidierung und **strikte Vergleiche** (Number vs. String).
- Verbesserte Fehlermeldungen, saubere HTML-Struktur, semantische Felder (`fieldset`, `label`).

## Lizenz
Siehe [LICENSE](LICENSE). Standard: MIT.
