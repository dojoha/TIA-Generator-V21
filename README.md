# TIA-Generator-V21

Deutsch | [English](#english)

## Deutsch

Tool zur automatisierten Erstellung und Bearbeitung von TIA-Portal-Projekten über die **TIA Portal Openness API**.

## Aktuell umgesetzte Funktionen

### Projektgenerierung

- Installierte TIA-Portal-Openness-Public-API über die Windows-Registry erkennen und zur Laufzeit laden.
- TIA Portal über Openness mit Benutzeroberfläche starten und die gestartete Instanz anzeigen.
- Eine Konfiguration (`.xlsx`/`.xlsm`) laden.
- Ein neues TIA-Projekt mit Name, Pfad, Autor und Kommentar anlegen.
- Stationen mit Bestellnummer, Version, Name und Beschreibung anlegen.
- Vorhandene Stationen erkennen und nach Bestätigung löschen und neu anlegen.
- Module an konfigurierten Positionen stecken und Startadressen setzen.
- PLC-Variablen inklusive Gruppe, Datentyp, Adresse, Kommentar, Typeobject-ID und Versions-ID erzeugen.
- Programmblausteine aus Typical-Vorlagen erzeugen, Platzhalter ersetzen, in Bausteingruppen importieren und den Importfortschritt anzeigen.
- Projekt speichern.
- Den vollständigen Ablauf als eine Projektgenerierung mit Einzelschritten, Fortschritt und Abbruchmöglichkeit ausführen.

### Projektübersicht

- Projektstruktur in einer Baumansicht anzeigen.
- Details zu Stationen, Modulen, PLC-Variablen und Programmbausteinen anzeigen.
- Status von TIA Portal, Verbindung, Projekt und gestarteter Instanz inklusive Prozess-ID und Version anzeigen.

### Typical-Editor

- TIA-Portal-XML-Dateien laden und typische Bausteine mit ihren Netzwerken, Parts, Access-Elementen und Verbindungen darstellen.
- Metadaten wie Bausteinname, Bausteinnummer, Bausteintyp, Programmiersprache und Engineering-Version anzeigen.
- Platzhalter automatisch vorschlagen oder für einzelne Netzwerke bzw. das gesamte Typical löschen.
- Access-Typen und Datentypen für unterstützte Elemente bearbeiten.
- Typical-XML mit gesetzten Platzhaltern speichern.
- Eine grafische Netzwerkansicht öffnen.
- Eine Excel-Konfigurationsvorlage für Typical-Instanzen exportieren.

### Bausteinexporter

- Aktive TIA-Portal-Instanzen mit geöffnetem Projekt suchen.
- Mit einer ausgewählten Projektinstanz verbinden und deren PLC-Bausteine einlesen.
- Bausteine aus der Projektstruktur für den Export auswählen.
- Exportliste bearbeiten und Duplikate verhindern.
- Bausteine als XML-Dateien in ein Zielverzeichnis exportieren.
- Vorhandene Exportdateien einzeln zum Überschreiben bestätigen.
- Exportfortschritt anzeigen.

### Bedienung und Lokalisierung

- Deutsch und Englisch als Benutzeroberfläche.
- Asynchrone Aktionen mit Statusmeldungen und Fortschrittsanzeigen.
- Abbruch des laufenden Software-/Bausteinimports.
- Sicherheitsabfragen vor dem Löschen oder Überschreiben vorhandener Daten.

## Voraussetzungen

- Windows 64 Bit
- TIA Portal mit installierter Komponente **TIA Portal Openness**
- Benutzerkonto in der lokalen Windows-Gruppe **Siemens TIA Openness**
- .NET Framework 4.8 Developer Pack oder Visual Studio 2022 mit .NET-Desktopentwicklung
- TIA-Portal V21, deren installierte Openness-Assembly über die Registry gefunden werden kann
- Freigabe der Anwendung in der TIA-Portal-Openness-Firewall, falls beim ersten Zugriff angefordert

## Starten

1. Archiv in ein beliebiges Verzeichnis entpacken und ausführen.


<a id="english"></a>

## English

Tool for automating the creation and editing of TIA Portal projects through the **TIA Portal Openness API**.

## Implemented features

### Project generation

- Detect and load the installed TIA Portal Openness Public API through the Windows registry at runtime.
- Start TIA Portal through Openness with its user interface and display the started instance.
- Load an configuration file (`.xlsx`/`.xlsm`).
- Create a new TIA project with name, path, author, and comment.
- Check the project directory before overwriting it and replace existing contents after confirmation.
- Create stations with order number, version, name, and description.
- Detect existing stations and delete/recreate them after confirmation.
- Plug modules at configured positions and set their start addresses.
- Generate PLC tags including group, data type, address, comment, type-object ID, and version ID.
- Generate program blocks from Typical templates, replace placeholders, import them into block groups, and report import progress.
- Save the project.
- Run the complete workflow as one project-generation operation with step-by-step progress and cancellation.

### Project overview

- Display the project structure in a tree view.
- Display details for stations, modules, PLC tags, and program blocks.
- Display TIA Portal, connection, project, and started-instance status, including process ID and version.

### Typical editor

- Load TIA Portal XML files and display Typical blocks with networks, parts, access elements, and connections.
- Display block name, block number, block type, programming language, and engineering version.
- Suggest placeholders automatically or clear them for individual networks or the complete Typical.
- Edit access types and data types for supported elements.
- Save Typical XML with assigned placeholders.
- Open a graphical network view.
- Export an Excel configuration template for Typical instances.

### Block exporter

- Find active TIA Portal instances with an open project.
- Connect to a selected project instance and read its PLC blocks.
- Select blocks from the project structure for export.
- Edit the export list and prevent duplicates.
- Export blocks as XML files to a target directory.
- Confirm overwriting existing export files individually.
- Display export progress.

### User interface and localization

- German and English user interface.
- Asynchronous actions with status messages and progress indicators.
- Cancellation of an ongoing software/block import.
- Confirmation dialogs before deleting or overwriting existing data.

## Requirements

- 64-bit Windows
- TIA Portal with **TIA Portal Openness** installed
- User account in the local Windows group **Siemens TIA Openness**
- .NET Framework 4.8 Developer Pack or Visual Studio 2022 with .NET desktop development
- TIA Portal V21 whose installed Openness assembly can be found through the registry
- Application approval in the TIA Portal Openness firewall if requested on first access

## Running

1. Download the archive, extract it to a folder and run the app
