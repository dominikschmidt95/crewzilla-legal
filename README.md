# Legal Documents — Crewzilla

Diese Dateien sind die **Single Source of Truth** für Datenschutzerklärung und Nutzungsbedingungen.

## Dokumente
- `privacy-de.md` / `privacy-en.md` — Datenschutzerklärung (Privacy Policy)
- `terms-de.md` / `terms-en.md` — Nutzungsbedingungen (Terms of Use)
- `index.md` — Übersicht / Landing-Page

## Hosting
- Dieses Repo ist privat; GitHub Pages hostet die Legal-Seiten daher über ein Public-Mirror-Repo: [`dominikschmidt95/crewzilla-legal`](https://github.com/dominikschmidt95/crewzilla-legal).
- Bei jedem Push auf `main`, der `legal/**` ändert, spiegelt `.github/workflows/sync-legal.yml` den Folder automatisch ins Public-Repo (Inhalt landet dort im Root).
- Pages-Setup im Public-Repo: Source = `main` branch, folder `/`.
- Erreichbar unter `https://dominikschmidt95.github.io/crewzilla-legal/<slug>/` (z. B. `.../privacy-de/`).

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

- Privacy DE: <https://dominikschmidt95.github.io/crewzilla-legal/privacy-de/>
- Privacy EN: <https://dominikschmidt95.github.io/crewzilla-legal/privacy-en/>
- Terms DE:   <https://dominikschmidt95.github.io/crewzilla-legal/terms-de/>
- Terms EN:   <https://dominikschmidt95.github.io/crewzilla-legal/terms-en/>

- Privacy-URL → App Store Connect → App Privacy → Privacy Policy URL
- Terms-URL → App Store Connect → General → App Information → License Agreement (optional, sonst gilt Apple Standard-EULA) sowie Marketing-Materialien
