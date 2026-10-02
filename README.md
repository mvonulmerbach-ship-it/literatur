# Weltliteratur – Lernkarten

Lernkarten-App fürs Handy zu den wichtigsten Werken der Weltliteratur – pro Buch ein Paket aus Inhalt, Autor, Interpretation und Einfluss.

**Live:** https://mvonulmerbach-ship-it.github.io/literatur/

## Inhalt

53 Werke mit zusammen 844 Karten (12–28 je Werk), dazu eine Einführungskarte je Werk. Kartenarten: Inhalt, Autor, Interpretation, Einfluss; ein Teil als Auswahlfragen mit Erklärung. Kanon-Auswahl u. a. nach dtv-Literaturkanon, „Die besten aller Zeiten“ und buchtipp.de; alle Texte sind eigenständig formuliert, keine Originalzitate.

## Funktionen

- **Werkliste** mit Titel, Autor · Jahr und Land · Epoche; Auswahlfeld **Epoche** filtert die Liste.
- Ein Werk antippen: Lernrunde mit allen Karten dieses Werks.
- **Alles gemischt:** Die Werke kommen in zufälliger Reihenfolge, die Karten eines Werks bleiben als Paket zusammen. Eine Runde nimmt ganze Pakete, bis mindestens 20 Karten erreicht sind, und endet an dieser Paketgrenze. Danach Zusammenfassung (gewusst / nicht gewusst) und **Nächste Runde** mit den übrigen Werken.
- Karte lesen, „Antwort zeigen“, dann selbst einschätzen (✓ Gewusst / ✗ Nicht gewusst); Auswahlfragen werden direkt ausgewertet.
- Punkte (⭐) und Zahl der gewussten und nicht gewussten Karten werden im Browser gespeichert (`localStorage`, Schlüssel `lit_store`).
- Hell/Dunkel oben rechts: ◐ System (Standard) · ☀️ Hell · 🌙 Dunkel (`lit_theme`).

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | die ganze App (HTML, CSS, JavaScript, alle Werke und Karten) – ca. 210 KB |
| `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `icon-maskable.png` | Installation als App |
| `sw.js` | Service Worker für den Offline-Betrieb |

Das zugehörige Nachschlagewerk: https://mvonulmerbach-ship-it.github.io/literatur-nachschlagewerk/

## Auf dem Handy installieren

Seite in Chrome öffnen → Menü ⋮ → „Zum Startbildschirm hinzufügen“ (Safari: Teilen → „Zum Home-Bildschirm“).

## Offline

Nach dem ersten Öffnen läuft die App ohne Netz (Service Worker, network first mit Cache als Rückfall).
