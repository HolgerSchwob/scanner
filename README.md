# Barcode-Checker

Zwei Barcodes nacheinander scannen – die App prüft, ob sie **identisch** sind. Führende Nullen werden ignoriert (z. B. `001234` = `1234`). Stimmen die restlichen Zahlen nicht, erscheint **FEHLER**.

- Für iPhone (z. B. iPhone 13 mini) und andere Geräte
- Eine einzige HTML-Datei, kein Build nötig
- ZXing lädt per CDN (Internet nötig)

## Auf deinem iPhone nutzen (GitHub Pages)

1. **Neues Repository auf GitHub anlegen**
   - GitHub → **New repository**
   - Name z. B. `barcode-checker`
   - Public, **ohne** README/Lizenz anlegen (leeres Repo)

2. **Projekt hochladen** (am PC in diesem Ordner, PowerShell oder CMD):

   Falls Git dich noch nie nach Name/E-Mail gefragt hat, einmalig ausführen:
   ```bash
   git config --global user.email "deine@email.de"
   git config --global user.name "Dein Name"
   ```

   Dann in diesem Ordner:
   ```bash
   cd "c:\Users\Holge\Desktop\scanner satinee"
   git add index.html README.md
   git commit -m "Barcode-Checker für GitHub Pages"
   git branch -M main
   git remote add origin https://github.com/DEIN-BENUTZERNAME/barcode-checker.git
   git push -u origin main
   ```

   Ersetze `DEIN-BENUTZERNAME` durch deinen GitHub-Benutzernamen und `barcode-checker` durch den gewählten Repo-Namen. (Repo ist hier bereits mit `git init` vorbereitet.)

3. **GitHub Pages aktivieren**
   - Im Repo: **Settings** → **Pages**
   - Unter "Source": **Deploy from a branch**
   - Branch: **main**, Ordner: **/ (root)** → **Save**

4. **Webseite öffnen**
   - Nach 1–2 Minuten: `https://DEIN-BENUTZERNAME.github.io/barcode-checker/`
   - Auf dem iPhone: Link in Safari öffnen oder als Lesezeichen/Startseite speichern.

**Hinweis:** Kamera-Zugriff muss im Browser erlaubt werden (Safari fragt nach Berechtigung).
