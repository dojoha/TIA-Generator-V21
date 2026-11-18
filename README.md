# TIA-Generator-V21

Deutsch | [English](#english)

## Deutsch

**Aus einer Excel-Tabelle wird ein fertiges TIA-Portal-Projekt.**

Wer viele gleichartige Anlagen oder Maschinen projektiert, kennt das: Stationen anlegen, Module stecken,
Variablen eintragen, Bausteine kopieren und anpassen – jedes Mal von Hand, jedes Mal dasselbe.
Der TIA-Generator nimmt Ihnen diese Fleißarbeit ab. Sie beschreiben Ihr Projekt einmal in Excel,
der Generator baut es in TIA Portal V21 für Sie auf – in Minuten statt Stunden und ohne Tippfehler.

### Wofür eignet sich das Programm?

- **Serienprojekte:** Gleiche oder ähnliche Anlagen immer wieder neu projektieren.
- **Große Projekte:** Hunderte Variablen, viele Stationen und Module ohne Handarbeit anlegen.
- **Einheitliche Qualität:** Alle Projekte folgen denselben Vorgaben, Namen und Strukturen.
- **Wiederverwendung:** Bewährte Bausteine einmal als Vorlage („Typical“) hinterlegen und beliebig oft einsetzen.

### Was macht der Generator?

Anhand Ihrer Excel-Konfiguration legt er automatisch an:

| Was | Beispiel |
|---|---|
| **TIA-Projekt** | Name, Speicherort, Autor, Kommentar |
| **Stationen** | Steuerungen mit Bestellnummer, Version, Name und Beschreibung |
| **Netzwerke** | Subnetze und deren Zuordnung zu den Stationen, IO-Devices an ihren IO-Controllern |
| **Module** | Baugruppen auf den richtigen Steckplätzen, inklusive Startadressen |
| **PLC-Variablen** | Gruppe, Datentyp, Adresse und Kommentar |
| **Standardbausteine** | Ihre Bibliothek bewährter Bausteine, in jede Steuerung importiert |
| **Programmbausteine** | Aus Ihren Vorlagen (Typicals) werden fertige Bausteine, Instanzen und Instanz-DBs |

Am Ende speichert der Generator das Projekt und erstellt auf Wunsch einen **Generierungsbericht** (PDF),
in dem Sie nachlesen können, was angelegt wurde.

### So arbeiten Sie damit

1. **Konfiguration vorbereiten:** Sie füllen die Excel-Datei mit Ihren Stationen, Modulen, Variablen und Bausteinen.
2. **Konfiguration laden:** Das Programm prüft die Tabelle und zeigt Ihnen Fehler und Unstimmigkeiten
   *vor* der Generierung an – zum Beispiel doppelte Namen, ungültige IP-Adressen oder fehlende Angaben.
3. **Projekt generieren:** Ein Klick auf **Projekt generieren** startet TIA Portal und führt alle Schritte nacheinander aus.
   Fortschritt und Einzelschritte sind sichtbar, der Vorgang lässt sich abbrechen.
4. **Ergebnis ansehen:** Die Projektstruktur samt Details sehen Sie direkt im Programm; im TIA Portal ist das Projekt geöffnet.

Wer es lieber Schritt für Schritt mag, kann Projekt, Hardware, Variablen und Software auch einzeln generieren.

### Die Hilfswerkzeuge

**Typical-Editor – Vorlagen selbst erstellen**
Aus einem bestehenden Baustein machen Sie eine wiederverwendbare Vorlage: Sie legen fest, welche Teile
(z. B. Variablen- und Bausteinnamen) später ausgetauscht werden sollen. Das Programm schlägt solche Platzhalter
selbst vor. Danach schreiben Sie die passende Tabelle für die Excel-Konfiguration mit einem Klick. Eine grafische
Netzwerkansicht hilft beim Kontrollieren.

**Bausteinexporter – Bausteine aus einem Projekt holen**
Verbindet sich mit einem geöffneten TIA-Projekt, zeigt dessen Bausteine als Baum und exportiert die ausgewählten
in ein Verzeichnis. So bauen Sie Ihre Vorlagen und Ihre Standardbaustein-Bibliothek auf.

### Sicherheit für Ihre Daten

- Bevor ein vorhandenes Projekt ersetzt oder Stationen gelöscht werden, **fragt das Programm nach**.
- Ein bestehendes Projekt wird vor dem Ersetzen **gesichert**.
- Es werden keine Programme auf reale Steuerungen geladen; der Generator arbeitet ausschließlich **offline im Projekt**.
- Das Programm läuft auf Deutsch und Englisch.

### Voraussetzungen

- Windows 64 Bit
- TIA Portal V21 mit installierter Komponente **TIA Portal Openness**
- Ihr Windows-Benutzer ist Mitglied der Windows-Gruppe **Siemens TIA Openness**
- Beim ersten Start fragt TIA Portal eventuell, ob der Generator zugreifen darf – bitte erlauben.

### Wo liegen meine Dateien?

Beim ersten Start legt das Programm unter `%AppData%\TIA Generator V21` automatisch drei Ordner an:

- `Typicals` – Ihre Vorlagen
- `Standardbausteine` – Ihre Bibliothek bewährter Bausteine
- `Import` – die erzeugten Bausteindateien vor dem Import in TIA Portal

---

<a id="english"></a>

## English

**Turn an Excel spreadsheet into a finished TIA Portal project.**

If you engineer many similar plants or machines, you know the routine: create stations, plug modules,
enter tags, copy and adapt blocks – by hand, every time. The TIA Generator takes this repetitive work off your hands.
Describe your project once in Excel and the generator builds it in TIA Portal V21 – in minutes instead of hours,
and without typos.

### What is it good for?

- **Series projects:** Engineer the same or similar plants again and again.
- **Large projects:** Create hundreds of tags, many stations and modules without manual work.
- **Consistent quality:** Every project follows the same rules, names and structure.
- **Reuse:** Store proven blocks once as a template ("Typical") and use them as often as you like.

### What does the generator do?

Based on your Excel configuration it automatically creates:

| What | Example |
|---|---|
| **TIA project** | Name, location, author, comment |
| **Stations** | Controllers with order number, version, name and description |
| **Networks** | Subnets and their assignment to stations, IO devices assigned to their IO controllers |
| **Modules** | Hardware modules in the right slots, including start addresses |
| **PLC tags** | Group, data type, address and comment |
| **Standard blocks** | Your library of proven blocks, imported into every controller |
| **Program blocks** | Your templates (Typicals) become finished blocks, instances and instance DBs |

At the end the generator saves the project and can create a **generation report** (PDF)
listing everything that was created.

### How you work with it

1. **Prepare the configuration:** Fill the Excel file with your stations, modules, tags and blocks.
2. **Load the configuration:** The program checks the spreadsheet and shows errors and inconsistencies
   *before* generating – for example duplicate names, invalid IP addresses or missing entries.
3. **Generate the project:** One click on **Generate project** starts TIA Portal and runs all steps in sequence.
   Progress and individual steps are visible, and you can cancel at any time.
4. **Review the result:** The project structure and details are shown in the program; the project is open in TIA Portal.

If you prefer to go step by step, you can also generate project, hardware, tags and software individually.

### The helper tools

**Typical editor – create your own templates**
Turn an existing block into a reusable template: you decide which parts (e.g. tag and block names) should be
replaced later. The program suggests such placeholders itself. Then, with one click, you write the matching sheet
for your Excel configuration. A graphical network view helps you check the result.

**Block exporter – get blocks out of a project**
Connects to an open TIA project, shows its blocks as a tree and exports the selected ones to a folder.
This is how you build your templates and your standard block library.

### Safety for your data

- Before an existing project is replaced or stations are deleted, **the program asks for confirmation**.
- An existing project is **backed up** before it is replaced.
- Nothing is downloaded to real controllers; the generator works **offline in the project** only.
- The program is available in German and English.

### Requirements

- 64-bit Windows
- TIA Portal V21 with the **TIA Portal Openness** component installed
- Your Windows user is a member of the **Siemens TIA Openness** group
- On first start TIA Portal may ask whether the generator may access it – please allow.

### Where are my files?

On first start the program automatically creates three folders under `%AppData%\TIA Generator V21`:

- `Typicals` – your templates
- `Standardbausteine` – your library of proven blocks
- `Import` – the generated block files before they are imported into TIA Portal
