# 🛡️ BlueTeam Suite

**BlueTeam Suite** ist eine eigenständige, lokale Desktop-Kommandozentrale für **Incident Response, Threat Intelligence, Digitale Forensik und SOC-Einsatzplanung** unter Linux – vollständig offline nutzbar, ohne Cloud-Zwang und ohne manuelle Paket-Nachinstallationen.

---

##  Enthaltene Werkzeuge

* **📝 BlueTeam Pad:** Strukturierter Vorfalls- & Analyse-Editor mit Word-Ribbon-Oberfläche, Tabellen, eigenen Favoriten, Farb-Themes sowie integrierter **C2- & CTI-MindMap** inklusive Komplett-PDF-Export.
* **📋 Incident Planning Tool:** 3-Spalten-Kanban-Board (*Offen / Triage*, *In Analyse / Eindämmung*, *Abgeschlossen / Gehärtet*) mit Schnellverschiebung per Doppelklick und PDF-Maßnahmenplan.
* **📅 BlueTeam Calendar:** Schicht-, Patch-Fenster- und Incident-Review-Kalender mit visueller Tagesmarkierung und PDF-Export.
* **🔬 Forensic & Hash Analyzer:** Drag-&-Drop-Triage für verdächtige Dateien (MD5, SHA1, SHA256, Magic-Bytes-Dateityperkennung, Shannon-Entropie-Messung sowie automatischer String- & IoC-Extractor).
* **🔓 Cyber-Decoder:** Lokaler Offline-Deobfuscator für Base64, PowerShell (`-EncodedCommand` UTF-16LE), Hex, URL-Encoding, ROT13 sowie IoC-Defang/Refang (`hxxp://`, `[.]`).
* **📖 Integriertes Handbuch:** Direkt abrufbare Schritt-für-Schritt-Hilfe zu allen Modulen und Tastenkürzeln.

---

## 🔒 Sicherheit & Datenschutz

* **100 % Lokal:** Alle Berichte, Aufgaben, Kalendereinträge und Einstellungen werden ausschließlich im persönlichen Benutzerverzeichnis unter `~/BlueTeamSuite/` gespeichert.
* **Kryptografischer Zugangsschutz:** Beim ersten Start wird ein lokales Benutzerkonto eingerichtet. Das Passwort wird mit **PBKDF2-HMAC-SHA256** (200.000 Iterationen + Zufalls-Salt) gesichert.
* **Integrierter Online-Updater:** Über die Einstellungen lässt sich jederzeit auf neue Releases prüfen und die Anwendung direkt aktualisieren, ohne dass bestehende Daten verloren gehen.

---

##  Installation & Start (Linux 64-Bit)

Es werden **weder Python noch zusätzliche Bibliotheken** benötigt – alle Abhängigkeiten sind bereits im Paket enthalten.

1. Laden Sie die aktuelle **`BlueTeamSuite-Linux.tar.gz`** aus dem Bereich **[Releases](../../releases)** herunter.
2. Entpacken Sie das Archiv und richten Sie die App inklusive Startmenü-Icon ein:
   ```bash
   tar -xzvf BlueTeamSuite-Linux.tar.gz
   cd BlueTeamSuite_Release
   ./App_Einrichten.sh
   ```
3. Starten Sie die **BlueTeam Suite** anschließend über Ihr Anwendungsmenü oder direkt per Doppelklick auf **`BlueTeam Suite Starten.desktop`** (bzw. `./BlueTeamSuite`).

---

## 📋 Systemvoraussetzungen

* **Betriebssystem:** 64-Bit Linux mit grafischer Oberfläche (Kali Linux, Debian, Ubuntu, Linux Mint)
* **Abhängigkeiten:** Keine (Standalone-Paket)
