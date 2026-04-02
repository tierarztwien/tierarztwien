# Todo-Liste — Website DDr. Antolini

**Stand:** 02.04.2026  
**Legende:** [x] erledigt | [ ] offen | [!] hohe Prioritaet

---

## BEREITS ERLEDIGT (diese Session)

- [x] Instagram-Profil korrigiert: @tierarztvienna → @tierarzt_wien (alle Referenzen)
- [x] 6 ungenutzte Fotos aus Fotos/-Ordner eingebunden (Galerie + Instagram-Sektion)
- [x] Favicon und Logo von externem WordPress-Server auf lokal umgestellt
- [x] Service-Icons durch lokale SVGs ersetzt (keine externe Abhaengigkeit mehr)
- [x] Team-Sektion "Unser Team" mit DDr. Antolini Portrait hinzugefuegt
- [x] Navigation um "Team"-Link erweitert (Desktop + Footer)
- [x] Instagram-Sektion: Platzhalter-Emojis durch echte Fotos ersetzt
- [x] Copyright-Jahr 2024 → 2025 aktualisiert
- [x] Schema.org Logo-URL auf lokale Datei umgestellt
- [x] Fotoshooting-Plan erstellt (docs/fotoshooting-plan.md)

---

## OFFENE AUFGABEN — TECHNIK

### Hohe Prioritaet
- [!] **Bilder komprimieren** — Alle Fotos sind 2-3 MB gross. Fuer Web sollten sie max. 200-400 KB sein. Tools: Squoosh, TinyPNG oder ImageOptim
- [!] **WebP-Format** — Zusaetzlich zu JPEG auch WebP-Versionen erstellen (50-70% kleiner)
- [!] **Responsive Images** — `srcset` und `sizes` Attribute hinzufuegen fuer verschiedene Bildschirmgroessen
- [!] **Sitemap.xml erstellen** — In robots.txt referenziert, existiert aber vermutlich nicht
- [ ] **Schema.org erweitern** — `Person`-Schema fuer DDr. Antolini hinzufuegen (Arzt-Profil)

### Mittlere Prioritaet
- [ ] **Online-Terminbuchung** — WhatsApp-Business oder Calendly-Integration statt nur Telefon-Link
- [ ] **Google Reviews Widget** — Echte Google-Bewertungen einbinden statt statischer Testimonials
- [ ] **404-Seite erstellen** — Aktuell keine benutzerdefinierte Fehlerseite
- [ ] **Impressum pruefen** — Ist die Impressum-Seite aktuell und DSGVO-konform?
- [ ] **Instagram API** — Echte Instagram-Posts automatisch laden (via Instagram Basic Display API)

### Niedrige Prioritaet
- [ ] **Performance-Audit** — Lighthouse-Test durchfuehren, Core Web Vitals pruefen
- [ ] **Decap CMS testen** — Ist das CMS Admin-Panel funktional? Galerie-Upload testen
- [ ] **Social Media Meta-Tags** — og:image auf ein hochwertigeres Foto aktualisieren
- [ ] **Breadcrumb erweitern** — Nur Homepage definiert, keine Unterseiten

---

## OFFENE AUFGABEN — CONTENT

### Hohe Prioritaet
- [!] **Fotoshooting durchfuehren** — Siehe docs/fotoshooting-plan.md
- [!] **Villa-Aussenfoto** — Fehlt komplett, groesster Content-Mangel
- [!] **Tiervielfalt** — Katzen, Kaninchen, andere Hunderassen fotografieren
- [ ] **DDr. Antolini Portrait** — Professionelles Einzelportrait fuer "Ueber Uns" und Google

### Mittlere Prioritaet
- [ ] **Leistungs-Unterseiten** — Eigene Seiten fuer jede Leistung (SEO-Vorteil)
- [ ] **Blog/Ratgeber starten** — "Zeckenvorsorge Wien", "Erste Hilfe Hund" etc.
- [ ] **Echte Bewertungen sammeln** — Kunden aktiv um Google-Bewertungen bitten
- [ ] **Instagram-Content-Plan** — Regelmaessige Posts (2-3x/Woche) planen

### Niedrige Prioritaet
- [ ] **Video-Content** — Kurze Praxis-Tour, "Ein Tag beim Tierarzt"
- [ ] **FAQ erweitern** — Haeufige Fragen aus der Praxis ergaenzen
- [ ] **Mehrsprachigkeit** — Englische Version fuer Expats in Wien?

---

## OFFENE AUFGABEN — MARKETING

### Hohe Prioritaet
- [!] **Google Business Profil** — Ist es vollstaendig? Fotos hochladen, Oeffnungszeiten pruefen
- [!] **Google Ads** — "Tierarzt Wien" Kampagne aufsetzen (Budget: ab EUR 300/Monat)
- [ ] **Local SEO** — Eintraege in Branchenverzeichnissen (Herold, WKO, Docfinder)

### Mittlere Prioritaet
- [ ] **Instagram Ads** — Gezielte Werbung im Einzugsgebiet (1130, 1140, 1120 Wien)
- [ ] **Empfehlungsprogramm** — "Empfehlen Sie uns weiter" mit Anreiz
- [ ] **Kooperationen** — Tierhandlungen, Hundeschulen in Hietzing

---

## Notizen

- Die `Fotos/`-Ordner enthaelt 16 Originalfotos, davon 6 jetzt eingebunden
- 4 Fotos im `images/`-Ordner waren vorher ungenutzt und sind jetzt teilweise integriert
- Die Website hat KEIN Analytics-Tool — Empfehlung: datenschutzkonformes Tool wie Plausible oder Fathom
- CMS (Decap) ist konfiguriert aber Galerie-Uploads scheinen leer zu sein
