# Icon-Pack-Preview

Public preview catalog for the **Icon Pack** Android app.

Icons here are shown as **Coming soon / Ready for next update**.
They do **not** apply in launchers until they are shipped inside the main Icon-Pack APK.

## Live URLs (GitHub Pages)

After Pages is enabled on `main` / root:

- Catalog: https://tarunverma959.github.io/Icon-Pack-Preview/catalog.json
- Example icon: https://tarunverma959.github.io/Icon-Pack-Preview/icons/sample.png

## Layout

```
catalog.json   # preview list the app fetches
icons/         # preview images (png/webp)
```

## Status values

| Status | Meaning |
|---|---|
| `coming_soon` | Designed, not in APK yet |
| `ready_for_next_update` | Will ship in the next Play Store release |
| `released` | Already shipped (optional history) |

## Workflow

1. Receive icon request (email/ZIP from the app)
2. Design icon
3. Add image under `icons/`
4. Add entry to `catalog.json`
5. When releasing: copy SVG + appfilter into the main Icon-Pack repo
6. Publish Play Store update
7. Mark catalog entry `released` or remove it

## catalog.json example

```json
{
  "version": 1,
  "updatedAt": "2026-09-09",
  "icons": [
    {
      "id": "whatsapp",
      "label": "WhatsApp",
      "packageName": "com.whatsapp",
      "image": "icons/whatsapp.png",
      "status": "coming_soon"
    }
  ]
}
```
