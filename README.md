# Legal Documents — Crewzilla

Diese Dateien sind die **Single Source of Truth** für Datenschutzerklärung und Nutzungsbedingungen.

## Dokumente
- `privacy-de.md` / `privacy-en.md` — Datenschutzerklärung (Privacy Policy)
- `terms-de.md` / `terms-en.md` — Nutzungsbedingungen (Terms of Use)
- `index.md` — Übersicht / Landing-Page

## Hosting
- GitHub Pages serviert dieses Verzeichnis öffentlich.
- Repo-Settings → Pages → Source: `main` branch, folder `/legal`.
- Erreichbar unter z.B. `https://<owner>.github.io/<repo>/privacy-de/` bzw. `.../terms-de/`,
  via CNAME unter `https://crewzilla.app/legal/privacy-de/` bzw. `.../terms-de/`.

## App-Bundle-Sync
Bei jeder Änderung müssen die Markdown-Dateien in das App-Bundle kopiert werden:

```bash
cp legal/privacy-de.md projektfriends/Resources/Legal/PrivacyPolicy.de.md
cp legal/privacy-en.md projektfriends/Resources/Legal/PrivacyPolicy.en.md
cp legal/terms-de.md   projektfriends/Resources/Legal/Terms.de.md
cp legal/terms-en.md   projektfriends/Resources/Legal/Terms.en.md
```

Diese Kopien werden im App-Build mitausgeliefert (über `fileSystemSynchronizedGroups`).

## USt-ID
- Falls keine USt-ID vorhanden, in `privacy-de.md`/`privacy-en.md` Zeile mit `{USTID}` löschen.

## Live URLs

- Privacy DE: `<FINALE_URL_PRIVACY_DE>` — nach Aktivierung von GitHub Pages eintragen
- Privacy EN: `<FINALE_URL_PRIVACY_EN>`
- Terms DE:   `<FINALE_URL_TERMS_DE>`
- Terms EN:   `<FINALE_URL_TERMS_EN>`

- Privacy-URL → App Store Connect → App Privacy → Privacy Policy URL
- Terms-URL → App Store Connect → General → App Information → License Agreement (optional, sonst gilt Apple Standard-EULA) sowie Marketing-Materialien
