# Lastenheft – 360 Grad Plattform App

## 1. Einleitung
**Projektname:** 360 Grad Plattform App  
**Ziel:** Entwicklung einer webbasierten Plattform zur Vermittlung von 360°-Fotograf:innen an Auftraggeber:innen mit integrierter Matching-, Buchungs- und Upload-Funktion.  
**Projektträger:** Klaus Baldauf (Solo-Entwicklung mit Beratungsteam der 7GB GmbH)

---

## 2. Zielsetzung und Zweck
Die Plattform soll eine digitale Infrastruktur bereitstellen, um Anbieter:innen von 360°-Fotografie-Dienstleistungen mit potenziellen Kund:innen zu vernetzen. Ziel ist ein niederschwelliger Zugang zu immersiven Medien und deren Produzent:innen.

---

## 3. Geltungsbereich
- Webplattform (Desktop, mobilfähig, PWA-fähig)
- MVP-Version mit Kernfunktionen (siehe Funktionsübersicht)
- Ziel: mittelfristige Erweiterung als Cross-Plattform-App für iOS und Android (z. B. via React Native / Expo)
- Sprachen: zunächst Deutsch (später erweiterbar)

---

## 4. Zielgruppen
- **B2B:** Immobilienmakler:innen, Wohnungsgesellschaften, Hotels, Museen, Restaurants, Stadtmarketing- und Regionalmarketing-Verantwortliche, Hochschul- und Bildungseinrichtungen, Eventagenturen
- **B2F:** Fotograf:innen mit Spezialisierung auf 360°-Aufnahmen, virtuelle Touren, Drohnenanwendungen (Einsteiger & Profis)

---

## 5. Anforderungen an das System

### 5.1 Funktionale Anforderungen (MVP)
1. **Nutzerverwaltung**
   - Registrierung & Login (Fotograf:in / Kund:in)
   - Profilverwaltung mit Portfolio, Kameraausstattung, Region

2. **Such- & Filterfunktion**
   - Filter nach Ort, Preis, Verfügbarkeit, Technik, Bewertung

3. **Matching-Modul (Basis)**
   - Regelbasiertes Vorschlagswesen (später KI-Erweiterung)

4. **Tour-Upload & Vorschau**
   - 360°-Content-Upload (JPEG, mp4, etc.)
   - Viewer-Integration auf Profil- und Projektseite

5. **Buchungssystem (Basisversion)**
   - Terminanfrage & Bestätigung
   - Kalenderansicht für Fotograf:innen

6. **Zahlungsmodul (Basisversion)**
   - Start mit PayPal
   - Stripe-Integration vorbereiten (für spätere Skalierung)
   - Option: parallele Nutzung von PayPal & Stripe

7. **Bewertungsfunktion**
   - Sterne-/Textbewertung nach Projektabschluss

8. **Community-Elemente (Basic)**
   - Öffentliche Fotowand / interner Blog / News-Feed

### 5.2 Nicht-funktionale Anforderungen
- Responsive Design (Mobile First)
- DSGVO-konforme Datenverarbeitung
- Performanceoptimiert (Ladezeit < 2 Sek.)
- SEO-Basics (strukturierte Daten, Open Graph)

---

## 6. Technische Randbedingungen

### Rechtliche Grundlagen (geplant bis Beta-Phase)

#### Buchungsbedingungen
1. Buchungsanfrage & Bestätigung (48h-Frist)
2. Verbindlichkeit bei Annahme
3. Stornierung durch Kund:in (bis 48h kostenfrei, <24h = 70 % Gebühr)
4. Stornierung durch Fotograf:in nur in Ausnahmefällen
5. Terminverschiebung in gegenseitigem Einvernehmen
6. No-Show = voller Betrag fällig
7. Kommunikation nur über Plattform
8. Vorauszahlung über PayPal oder Stripe
9. Automatisierte Rechnung & Gutschrift

#### Allgemeine Geschäftsbedingungen (AGB)
1. Geltungsbereich: Vermittlung von Dienstleistungen
2. Plattform als Vermittler, nicht Vertragspartner
3. Buchung & Bezahlung mit Provision
4. Stornierungen & Gebühren
5. Bewertungen mit Moderation
6. Haftungsausschluss für Dienstleistungsqualität
7. DSGVO-konforme Datenverarbeitung
8. Deutsches Recht, Gerichtsstand Frankfurt (Oder)

### Weitere rechtliche Aspekte
- Datenschutz & Einwilligungen
- Widerrufsrecht für Verbraucher:innen
- Gebührenstruktur: Plattformprovision (10–15 %)
- Zahlungsgebühren: PayPal & Stripe (ca. 2,5 % + Fixbetrag)
- Rechnungsstellung: automatisiert via Drittanbieter

### Technologischer Stack
- **Frontend:** React / Next.js
- **Backend:** Node.js / Firebase (oder Alternative)
- **Datenhaltung:** JSON / NoSQL (MongoDB)
- **Hosting:** Vercel / Netlify
- **Viewer:** Integration externer 360°-Viewer (z. B. Kuula)

---

## 7. Schnittstellen / Erweiterungen (optional)
- Stripe-Zahlungsschnittstelle
- Export zu VR/AR-Anwendungen (Q4-Roadmap)
- API für Tour-Sharing (Einbettung in externe Seiten)

---

## 8. Projektorganisation
- Einzelentwicklung mit iterativer Abstimmung im Beratungsteam
- Testphase mit 5–10 Pilotnutzer:innen in Q2
- Laufende Dokumentation über GitHub / Confluence

---

## 9. Zeitplanung
- **Q2:** Alpha-Version (Registrierung, Upload, Matching)
- **Q3:** Beta-Version (Buchung & Bewertung)
- **Q4:** Launch (Community & Zahlungsmodul)

---

## 10. Abgrenzung
Nicht Bestandteil des MVP:
- Native Mobile App (nur perspektivisch)
- Vollautomatisiertes KI-Matching
- Mehrsprachigkeit / Internationalisierung

---

**Letzte Aktualisierung:** 28.03.2025  
**Hinweis:** Die Plattform wird als responsive Webanwendung mit PWA-Funktionalität entwickelt. Eine native App ist für spätere Projektphasen vorgesehen.



---

## 5.4 Speicherung & Verwaltung von 360°-Aufnahmen

1. **Wahlmöglichkeit für Datenhaltung**
   - Plattform-Hosting (z. B. via Firebase Storage, Cloudflare R2, Amazon S3)
   - Eigenes Hosting durch Nutzer:innen (externe URL oder FTP)

2. **Verwaltung**
   - Nutzerkonten mit Projektordnern, Tagging, Versionsverlauf
   - Speicherlimits abhängig vom Nutzungsmodell (z. B. Free/Premium)

3. **DSGVO-konforme Speicherung**

---

## 7. Schnittstellen / Erweiterungen (erweitert)

- Schnittstelle zu Stripe (Zahlung)
- Export zu VR/AR-Anwendungen (Roadmap Q4)
- API für Tour-Sharing (z. B. Einbettung in externe Webseiten)
- **Einbettung in Kund:innen-Webseiten** (Embed-Code, QR, API)
- **Kompatibilität mit externen Plattformen** (z. B. Immobilienportale, VR-Headsets)

---

## 11. Plattformökosystem & Partnernetzwerk (neu)

Die Plattform wird als Ökosystem gedacht, das die Zusammenarbeit mit Dritten fördert:

- **Vermittlung von Freelancer:innen** für Bearbeitung und Postproduktion
- **Zusammenarbeit mit Dienstleister:innen aus Tourismus, Bildung, Immobilien, Kultur**
- **Integration externer Tools und Plattformen** (z. B. für KI-Bearbeitung, virtuelle Räume)
- **Zukunftsvision:** Aufbau eines kuratierten Partner:innen-Marktplatzes