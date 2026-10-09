# Extension Gallery

Turn a Chrome/Chromium extension ZIP into a product showcase.

## MVP
- Browser-side ZIP parsing with JSZip: extension archives stay on your device.
- Manifest V2/V3 extraction, localized name and description, icon, version and permissions.
- Editable product details, links, screenshots and responsive live preview.
- Export showcase JSON locally.

## Run
```bash
npm install
npm run dev
npm run build
```

## Limitations
This is a prototype, not a live extension publishing or hosting service. There is no database, accounts, public product URLs, malware scanning, or ZIP hosting. Upload limit is 25 MB / 1500 ZIP entries; images under 4 MB. Parsed permissions are **not** a safety verification. Do not install untrusted extensions. The extension archive is never uploaded to a server.
