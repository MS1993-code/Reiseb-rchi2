# Navia

Reisebegleiter fürs Handy. **Alles bleibt auf dem Gerät** – keine Cloud, kein Konto, keine KI.

## Auf GitHub Pages legen (wie die andere App)

1. Bei GitHub ein **neues öffentliches Repository** anlegen, z. B. `navia`.
2. Alle Dateien aus diesem Ordner hochladen (Drag & Drop im Tab *Uploading files*).
3. Im Repo: **Settings → Pages**
   - Source: *Deploy from a branch*
   - Branch: `main`
   - Folder: **`/docs`**
   - Save
4. Eine Minute warten. Oben in Settings → Pages steht dann die Adresse, etwa:

   `https://DEIN-NAME.github.io/navia/`

5. Diese Adresse auf dem Handy im Browser öffnen.
   - **iPhone:** Teilen → *Zum Home-Bildschirm*
   - **Android:** Menü → *App installieren*

Fertig. Die App im Ordner `docs/` ist schon gebaut – du brauchst kein Terminal und kein Vercel.

## Was wo liegt

| Ordner | Bedeutung |
| --- | --- |
| `docs/` | Die fertige App. GitHub Pages liest nur diesen Ordner. |
| `src/`, `public/`, `package.json` | Quellcode, falls du später selbst weiterbauen willst. |

Daten (Reisen, Guides, Fotos) speichert die App lokal im Browser des Handys. Ein Backup machst du in der App unter **Profil → Sichern**.

Karten und Wetter brauchen Internet, wenn du sie nutzt. Der Rest funktioniert offline, sobald die App einmal geladen ist.

## Optional: selbst bauen

Nur nötig, wenn du den Code änderst:

```bash
npm install
npm run build
```

Danach den Inhalt von `docs/` erneut auf GitHub legen.
