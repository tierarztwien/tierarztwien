# Setup-Anleitung: Website DDr. Antolini

## Schnellstart: In 10 Minuten online

### Schritt 1: GitHub Repository
1. Erstelle ein GitHub-Repository (z.B. `tierarzt-antolini-website`)
2. Pushe alle Dateien dieses Ordners dorthin
3. Repository kann privat sein

### Schritt 2: Netlify Deployment
1. Gehe zu https://app.netlify.com
2. "Add new site" → "Import an existing project"
3. Wähle dein GitHub-Repository
4. Klicke "Deploy site" — fertig!

Die Website ist jetzt unter `random-name.netlify.app` erreichbar.

### Schritt 3: Custom Domain anbinden
1. In Netlify: "Domain settings" → "Add custom domain"
2. Gib `tierarztantolini.at` ein
3. Netlify zeigt dir DNS-Einstellungen die du beim Domain-Registrar setzen musst
4. Warte auf DNS-Propagation (~1-24 Stunden)
5. HTTPS wird automatisch aktiviert

### Schritt 4: CMS aktivieren (Netlify Identity)
1. In Netlify: "Site settings" → "Identity" → "Enable Identity"
2. "Registration preferences" → "Invite only"
3. "Services" → "Git Gateway" → "Enable Git Gateway"
4. "Identity" → "Invite users" → E-Mail von Dr. Antolini eingeben
5. Dr. Antolini erhält eine E-Mail mit Login-Link

### Schritt 5: Admin-Panel testen
1. Gehe zu `https://tierarztantolini.at/admin/`
2. Login mit der eingeladenen E-Mail
3. Galerie-Bilder hochladen, Bewertungen bearbeiten, Instagram-Posts erstellen

---

## Dateien-Übersicht

```
/
├── index.html              ← Die Website
├── admin/
│   ├── index.html          ← CMS Admin-Panel (Decap/Netlify CMS)
│   └── config.yml          ← CMS-Konfiguration (Collections, Felder)
├── content/
│   ├── galerie/            ← Galerie-Bilder (Markdown-Dateien)
│   ├── bewertungen/        ← Kundenbewertungen
│   ├── leistungen/         ← Angebotene Services
│   ├── instagram/          ← Instagram-Posts (Entwürfe & Geplant)
│   └── settings/
│       └── general.json    ← Allgemeine Einstellungen
├── images/
│   ├── uploads/            ← Vom CMS hochgeladene Bilder
│   └── galerie/            ← Galerie-Fotos
├── docs/
│   ├── seo-marketing-plan.md      ← SEO & Marketing-Strategie
│   ├── instagram-automation.md    ← Instagram-Automatisierung
│   └── setup-anleitung.md         ← Diese Datei
├── netlify.toml            ← Netlify-Konfiguration
└── robots.txt              ← Suchmaschinen-Anweisungen
```

---

## CMS-Bedienung für Dr. Antolini

### Galerie-Bild hinzufügen
1. Einloggen auf `tierarztantolini.at/admin/`
2. "Galerie" → "Neues Galerie-Bild"
3. Titel eingeben, Bild hochladen
4. Kategorie wählen (Villa, Behandlung, Team, etc.)
5. "Veröffentlichen" klicken
6. Fertig! Bild erscheint auf der Website.

### Bewertung hinzufügen
1. "Bewertungen" → "Neue Bewertung"
2. Kundenname, Text, Tier-Emoji eingeben
3. "Veröffentlichen"

### Instagram-Post erstellen
1. "Instagram Posts" → "Neuer Instagram Post"
2. Thema und Bild eingeben
3. Caption (Text) schreiben
4. Hashtags anpassen
5. Status auf "Geplant" setzen
6. Text in Meta Business Suite kopieren zum Veröffentlichen

---

## Wichtige Hinweise

- **Bilder optimieren:** Vor dem Upload auf max. 1200px Breite skalieren
- **Alt-Texte:** Immer eine Bildbeschreibung eingeben (für SEO und Barrierefreiheit)
- **Backups:** Netlify + GitHub = automatisches Backup bei jedem Commit
- **SSL:** Wird automatisch von Netlify bereitgestellt (Let's Encrypt)
