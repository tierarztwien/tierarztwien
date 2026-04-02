# Projekt-Status: DDr. Antolini Website

**Stand:** 2. April 2026

---

## Erledigt

### Website
- [x] Website im Villa-Classica-Design erstellt (index.html)
- [x] SEO-optimiert (Schema.org VeterinaryCare, FAQ, Meta-Tags, Keywords)
- [x] DSGVO-konform (Fonts lokal, Maps 2-Klick, Cookie-Banner mit Consent)
- [x] Impressum erstellt (impressum.html) — ECG § 5, UID ATU 38190505
- [x] Datenschutzerklärung erstellt (datenschutz.html) — Art. 13 DSGVO
- [x] Galerie-Sektion mit Lightbox
- [x] Instagram-Feed-Sektion
- [x] FAQ-Bereich (5 Fragen, Google Rich Snippets)
- [x] Notfall-Button + WhatsApp-Button (floating)
- [x] Responsive Design (Mobile, Tablet, Desktop)
- [x] Scroll-Animationen
- [x] robots.txt

### Hosting & Deployment
- [x] GitHub-Repository: https://github.com/tierarztwien/tierarztwien
- [x] Netlify Deployment: https://jade-quokka-09d023.netlify.app
- [x] Domain `tierarztantolini.at` in Netlify als Custom Domain hinzugefügt
- [x] DNS bei one.com geändert:
  - A-Record: `tierarztantolini.at` → `75.2.60.5`
  - CNAME: `www` → `jade-quokka-09d023.netlify.app`
- [ ] DNS-Propagation abwarten (bis zu 24h)
- [ ] HTTPS-Zertifikat wird automatisch von Netlify erstellt nach DNS-Verifizierung

### CMS (Netlify/Decap CMS)
- [x] Admin-Panel erstellt (admin/index.html + config.yml)
- [x] Collections: Galerie, Bewertungen, Leistungen, Instagram, Einstellungen
- [ ] Netlify Identity aktivieren (Enable Identity, Invite Only, Git Gateway)
- [ ] Benutzer einladen (E-Mail von René + Dr. Antolini)
- [ ] Erster Login auf /admin/ testen

### Dokumentation
- [x] SEO & Marketing-Plan (docs/seo-marketing-plan.md)
- [x] Instagram-Automatisierung (docs/instagram-automation.md)
- [x] Setup-Anleitung (docs/setup-anleitung.md)
- [x] Dieser Projekt-Status (docs/projekt-status.md)

---

## Offen / Nächste Schritte

### Sofort (wenn DNS durch ist)
1. HTTPS prüfen — sollte automatisch von Netlify kommen
2. Netlify Identity aktivieren + Benutzer einladen
3. Admin-Panel testen: `https://tierarztantolini.at/admin/`
4. Alte WordPress-Seite bei one.com vorerst als Backup lassen

### Woche 1
5. Echte Fotos hochladen (Villa, Behandlungsräume, Garten, Team)
6. Bewertungen durch echte Kundenstimmen ersetzen (oder Google Reviews einbinden)
7. Google Business Profil erstellen: https://business.google.com
8. Google Search Console einrichten: https://search.google.com/search-console

### Woche 2-4
9. Lokale Verzeichnisse eintragen (Herold, DocFinder, Gelbe Seiten, Tierärztekammer)
10. Instagram-Posting starten (@tierarztvienna, 3x/Woche)
11. Domain `tierarztwien.at` ggf. als Redirect auf tierarztantolini.at einrichten
12. Ersten Blog-Artikel veröffentlichen

### Monat 2-3
13. Google Ads Kampagne starten (Budget: 500-800 EUR/Monat)
14. Bewertungs-QR-Code in der Ordination aufstellen
15. WordPress-Hosting bei one.com kündigen (wenn alles stabil)
16. Erste KPI-Review

---

## Zugänge & Accounts

| Service | URL | Status |
|---------|-----|--------|
| GitHub | https://github.com/tierarztwien/tierarztwien | Aktiv |
| Netlify | https://app.netlify.com | Aktiv |
| Netlify Site | https://jade-quokka-09d023.netlify.app | Live |
| one.com (Domain) | https://www.one.com | Zugang vorhanden |
| Domain | tierarztantolini.at | DNS wird umgestellt |
| Admin-Panel | /admin/ | Noch nicht aktiviert (Identity fehlt) |

---

## Dateistruktur

```
tierarztwien/
├── index.html              Website (Hauptseite)
├── impressum.html          Impressum (ECG § 5)
├── datenschutz.html        Datenschutzerklärung (DSGVO)
├── robots.txt              Suchmaschinen-Anweisungen
├── netlify.toml            Netlify-Konfiguration
├── .gitignore              Git-Ignore-Regeln
├── admin/
│   ├── index.html          CMS Admin-Panel (Decap CMS)
│   └── config.yml          CMS-Konfiguration
├── content/
│   ├── galerie/            Galerie-Bilder (Markdown)
│   ├── bewertungen/        Kundenbewertungen
│   ├── leistungen/         Services
│   ├── instagram/          Instagram-Post-Entwürfe
│   └── settings/
│       └── general.json    Allgemeine Einstellungen
├── fonts/                  Lokal gehostete Schriftarten (DSGVO!)
│   ├── cormorant-garamond-*.ttf
│   └── montserrat-*.woff2
├── images/
│   ├── uploads/            CMS-Uploads
│   └── galerie/            Galerie-Fotos
└── docs/
    ├── seo-marketing-plan.md      90-Tage Marketing-Strategie
    ├── instagram-automation.md    Instagram-Automatisierung
    ├── setup-anleitung.md         Technische Setup-Anleitung
    └── projekt-status.md          Dieser Status
```

---

## Technische Details

| Eigenschaft | Wert |
|-------------|------|
| Design | Villa Classica (Cream, Gold, Braun) |
| Fonts | Cormorant Garamond (Serif), Montserrat (Sans) — lokal gehostet |
| CMS | Decap CMS (ehem. Netlify CMS) |
| Hosting | Netlify (Free Tier) |
| Domain-Registrar | one.com |
| SSL/HTTPS | Let's Encrypt via Netlify (automatisch) |
| Tracking | Keines (DSGVO-konform) |
| Google Maps | 2-Klick-Lösung (erst nach Consent) |
| Cookie-Banner | DSGVO-konform, sofort sichtbar, granular |
