# CLAUDE.md – TPB-B-hnenplan (öffentlich, GitHub Pages)

Bühnenplaner unter https://leouli23.github.io/TPB-B-hnenplan/: eine Seite (`index.html`) mit eigenen Bibliotheken in `bibliothek/` (jsPDF, pdf.js mit Worker, supabase-js). Gemeinsame Aufstellungen speichert er in Supabase über den Login der TPB-App (`tpb-auth`). Sicherheitsregeln: `SICHERHEIT.md`.

## Prüfung

Die Prüfskripte liegen im privaten Repository TPB-Backup (`app-werkzeug/pruefung/buehnen-test.js`, 27 Prüfungen; Pfad zu diesem Repository in `BUEHNE_DIR`). Sie laufen bei jedem Pull Request als „Release Prüfung“, dazu Gitleaks (`.gitleaks.toml`). Geprüft werden auch: kein Abruf bei fremden Servern, 375 px ohne seitliches Scrollen.

## Regeln

- Änderungen nur nach Leos Go als Pull Request; Leo mergt, Claude mergt nie.
- Keine Geheimwerte, keine personenbezogenen Daten in diesem öffentlichen Repository. Bibliotheken nur aus `bibliothek/`, nie von CDNs laden.
- Gedächtnis-Dokumente schreibt nur der App-Chat (siehe CLAUDE.md der TPB-App).
