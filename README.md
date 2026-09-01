# Vorher VS Nachher

Mobile-First-PWA für Handwerker zur schnellen Arbeitsdokumentation: Vorher-Fotos aufnehmen, Arbeitsstunden eintragen, Nachher-Fotos aufnehmen und eine PDF-Dokumentation erstellen.

## Funktionen

- Vorher- und Nachher-Fotos per Kamera oder Galerie
- Dezimale Arbeitszeit in Stunden – bewusst ohne Timer
- Optionale Kunden-, Projekt-, Adress- und Bildnotizen
- Lokales Auftragsarchiv mit Suche
- Kalenderansicht mit Monats-, Tages- und Zeitraumsauswahl
- Arbeitsnachweis als kompakte oder bebilderte PDF
- Manueller Vorher-/Nachher-Vergleich
- Professionelle PDF-Dokumentation und native Teilen-Funktion
- Installierbare PWA mit Offline-Grundfunktion
- Lokale Speicherung in IndexedDB

## Installation

```bash
git clone <repository>
cd vorher-vs-nachher
npm install
npm run dev
```

## Production Build

```bash
npm run build
```

## Technologie

React 19, TypeScript, Vinext/Vite, Tailwind CSS, IndexedDB, jsPDF und Web Share API.

## Datenspeicherung

Aufträge, Texte, Arbeitsstunden und Fotos werden in der aktuellen Version ausschließlich lokal im Browser auf dem jeweiligen Gerät gespeichert. Es werden keine Fotos oder Kundendaten automatisch hochgeladen.

## Android APK

Die Android-App wird als Trusted Web Activity gebaut. Sie startet Vorher Nachher als eigenständige Vollbild-App und verwendet denselben Web-Ursprung wie die installierte Chrome-Version. Der automatisierte GitHub-Workflow baut eine signierte Release-APK, prüft deren Signatur und veröffentlicht sie im GitHub-Release.

Die fertige APK heißt Vorher-Nachher-v1.0.0.apk.

## Einschränkungen des MVP

- Die lokale Speicherkapazität hängt vom Browser und Gerät ab.
- Geräteübergreifende Synchronisation und Cloud-Backup sind nicht enthalten.
