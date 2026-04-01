# Instagram-Automatisierung: DDr. Antolini

## Konzept

Die Instagram-Posts werden in **drei Stufen** automatisiert:

1. **Content-Generierung** (Claude/KI) — Posts werden automatisch vorbereitet
2. **Review** (Dr. Antolini/René) — Kurzer Check im CMS
3. **Veröffentlichung** (Meta Business Suite) — Automatisch geplant

---

## Stufe 1: Automatische Content-Generierung

### Claude Code Scheduled Agent (empfohlen)

Ein Claude Code Agent wird per Cron-Job wöchentlich ausgeführt und erstellt automatisch Instagram-Posts:

```
Jeden Montag um 9:00 → Claude erstellt 3-4 Posts für die Woche
→ Posts werden als Markdown-Dateien in content/instagram/ gespeichert
→ Bilder werden als Canva-taugliche Beschreibungen hinterlegt
→ Status: "entwurf"
```

### Post-Vorlagen (Prompt-Templates)

**Template 1: Tier-Tipp**
```
Erstelle einen Instagram-Post für @tierarztvienna:
- Thema: [saisonales Thema, z.B. Zeckenschutz im Frühling]
- Ton: warm, kompetent, nicht belehrend
- Lokaler Bezug: Wien/Hietzing erwähnen
- Länge: 150-200 Wörter
- 5-10 relevante Hashtags
- CTA: Termin vereinbaren / Frage stellen
- Emoji-Stil: dezent, nicht überladen
```

**Template 2: Praxis-Einblick**
```
Erstelle einen Instagram-Post für @tierarztvienna:
- Thema: Behind the Scenes unserer Villa-Ordination
- Zeige die einzigartige Atmosphäre
- Betone: historische Villa, Ruhe, Garten, italienisches Flair
- CTA: Besuchen Sie uns
```

**Template 3: Patienten-Story**
```
Erstelle einen Instagram-Post für @tierarztvienna:
- Thema: Erfolgsgeschichte eines Patienten
- Tier: [Hund/Katze/Kaninchen], Name: [Name]
- Geschichte: [kurze Beschreibung]
- Happy End betonen
- CTA: Ihr Tier verdient die beste Betreuung
```

---

## Stufe 2: Content-Kalender (automatisch befüllt)

| KW | Montag (Tipp) | Mittwoch (Praxis) | Freitag (Story) |
|----|--------------|-------------------|-----------------|
| Auto-generiert basierend auf Saison, Feiertagen und Tier-Gesundheitsthemen |

### Saisonale Trigger

| Monat | Automatische Themen |
|-------|-------------------|
| Mär-Apr | Zecken, Frühlings-Vorsorge, Allergien |
| Mai-Jun | Reise mit Tier, Hitze-Tipps, Garten-Gefahren |
| Jul-Aug | Sommer-Hitze, Wasser-Sicherheit, Urlaubsbetreuung |
| Sep-Okt | Herbst-Check, Entwurmung, Fellwechsel |
| Nov-Dez | Silvester-Angst, Weihnachts-Gefahren, Winter-Pflege |
| Jan-Feb | Neujahrs-Vorsorge, Indoor-Beschäftigung, Dental-Monat |

---

## Stufe 3: Veröffentlichung

### Option A: Meta Business Suite (Empfohlen)
- Kostenlos
- Posts im Voraus planen
- Bilder + Text einfügen
- Automatische Veröffentlichung zum geplanten Zeitpunkt
- URL: https://business.facebook.com

### Option B: Later.com / Buffer
- Posts visuell planen (Kalender-Ansicht)
- Kostenpflichtig (~15 EUR/Monat)
- Zusätzliche Analytics

---

## Workflow: Wöchentlich

```
Montag 09:00  → Claude generiert 3-4 Posts (automatisch)
Montag 10:00  → Posts erscheinen im CMS als "Entwurf"
Dienstag      → René/Dr. Antolini reviewed Posts im CMS
                 → Ändert Status auf "geplant"
                 → Kopiert Text in Meta Business Suite
Automatisch   → Meta veröffentlicht zu geplanten Zeiten
```

---

## Bild-Erstellung

### Option A: Canva Templates (Empfohlen für Dr. Antolini)
- Vorgefertigte Templates im Villa-Classica-Design
- Farben: Cream (#faf8f4), Gold (#8b7355), Braun (#2d2926)
- Font: Cormorant Garamond (Headlines), Montserrat (Body)
- Dr. Antolini tauscht nur Text und Bild aus

### Option B: KI-generierte Bilder
- Claude beschreibt das gewünschte Bild
- Midjourney/DALL-E generiert es
- Im CMS hochladen

### Option C: Eigene Fotos (Bestes für Authentizität)
- Handy-Fotos aus der Ordination
- Patienten (mit Erlaubnis)
- Villa, Garten, Team
- Kurzer Bildbearbeitung-Filter für einheitlichen Look

---

## Beispiel: Automatisch generierter Post

```markdown
---
title: "Zeckenzeit: 5 Tipps zum Schutz Ihres Hundes"
image: "/images/instagram/2026-04-zecken.jpg"
caption: |
  🌿 Der Frühling ist da — und mit ihm die Zecken.

  Als Tierarzt in Wien-Hietzing sehe ich jedes Jahr Hunde mit Zeckenbissen,
  die vermeidbar gewesen wären. Hier meine 5 wichtigsten Tipps:

  1️⃣ Zeckenschutz BEVOR die Saison beginnt
  2️⃣ Nach jedem Spaziergang gründlich absuchen
  3️⃣ Zecke sofort und richtig entfernen
  4️⃣ Auf Rötungen an der Bissstelle achten
  5️⃣ Bei Fieber oder Appetitlosigkeit sofort zum Tierarzt

  Fragen? Schreiben Sie uns per WhatsApp oder rufen Sie an.
  ☎️ +43 664 340 35 62

  #TierarztWien #TierarztHietzing #Zeckenschutz #HundeWien
  #TiergesundheitWien #DDrAntolini #Frühling #ZeckenTipps
hashtags: "#TierarztWien #TierarztHietzing #Zeckenschutz #HundeWien #TiergesundheitWien"
date: 2026-04-07T10:00:00
likes: 0
status: "entwurf"
---
```
