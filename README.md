# Legal Documents — Crewzilla

Diese Dateien sind die **Single Source of Truth** für die Datenschutzerklärung.

## Hosting
- GitHub Pages serviert dieses Verzeichnis öffentlich.
- Repo-Settings → Pages → Source: `main` branch, folder `/legal`.
- Erreichbar unter z.B. `https://<owner>.github.io/<repo>/privacy-de/`
  bzw. via CNAME unter `https://crewzilla.app/legal/privacy-de/`.

## App-Bundle-Sync
Bei jeder Änderung müssen die Markdown-Dateien in das App-Bundle kopiert werden:

```bash
cp legal/privacy-de.md projektfriends/Resources/Legal/PrivacyPolicy.de.md
cp legal/privacy-en.md projektfriends/Resources/Legal/PrivacyPolicy.en.md
```

Diese Kopien werden im App-Build mitausgeliefert (über `fileSystemSynchronizedGroups`).

## Platzhalter vor Veröffentlichung füllen
- `{VERANTWORTLICHER_NAME}` — Name des Inhabers (Gewerbe)
- `{ANSCHRIFT}` — Ladungsfähige Anschrift
- `{KONTAKT_EMAIL}` — Datenschutz-Kontakt
- `{USTID}` — optional, falls vorhanden

## Live URLs

- Deutsch: `<FINALE_URL_DE>` — nach Aktivierung von GitHub Pages eintragen
- English: `<FINALE_URL_EN>` — nach Aktivierung von GitHub Pages eintragen

Diese URLs werden in App Store Connect → App Privacy → Privacy Policy URL eingetragen.
