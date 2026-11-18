# luca-haenni.ch

Portfolio-Webseite von Luca Hänni.

## Struktur
- `index.html` – die Startseite
- `blog.html` – Blog-Übersicht (listet alle Beiträge automatisch auf)
- `_posts/` – die Blogbeiträge (Markdown)
- `_layouts/` – Layout-Vorlagen (default, post)
- `css/style.css` – Styles
- `assets/img/` – Bilder
- `CNAME` – verknüpft die GitHub-Pages-Seite mit der eigenen Domain
- `_config.yml` – Jekyll-Konfiguration

## Neuen Blogbeitrag erstellen
1. Datei in `_posts/` anlegen, Namensformat: `JJJJ-MM-TT-titel.md`
   (z. B. `2026-10-03-herbstparty.md`)
2. Am Dateianfang den Titel eintragen:
   ```
   ---
   title: "Mein Beitragstitel"
   ---
   ```
3. Darunter den Text in Markdown schreiben
4. Committen (geht auch direkt im Browser über "Add file" → "Create new file" im GitHub-Repo)

Der Beitrag erscheint danach automatisch unter `/blog/`, GitHub Pages
generiert die Seite selbst – kein Build-Schritt nötig.

## Domain verknüpfen (GitHub Pages)
Bei den Nameservern (ch.pro.io / nl.pro.io / p.dnh.net) folgende Einträge setzen:

**A-Records** (Hauptdomain, alle vier eintragen):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME** für `www`:
```
<github-username>.github.io
```

Danach in den Repo-Einstellungen unter *Pages* die Domain `luca-haenni.ch` eintragen
und "Enforce HTTPS" aktivieren, sobald verfügbar.
