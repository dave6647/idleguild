# 📱 UI/UX-Konzept – "Guild Life"

---

## 🌍 Grundkonzept

Das Interface folgt dem **BitLife-Prinzip**: Alles wird über **vertikale Listen, Menüs und Tap-Aktionen** gesteuert. Keine Open-World-Map, keine komplexe Navigation. Der Spieler scrollt durch Optionen und tippt auf Aktionen. Das Spiel muss **mit einer Hand** spielbar sein.

### Kernregeln

| Regel | Entscheidung |
|---|---|
| 📖 Tutorial | Nein, Learning-by-Doing (wie BitLife) |
| ⏳ Idle-Elemente | Nein, rein rundenbasiert (Saison-System) |
| 🌙 Dark Mode | Ja, dunkles Pergament mit heller Schrift |
| 📱 Ausrichtung | Nur Portrait (wie BitLife) |

---

## 📐 Design-Prinzipien

| Prinzip | Umsetzung |
|---|---|
| 📱 **Mobile-First** | Alles für vertikales Handy-Display optimiert |
| 👆 **One-Hand-Play** | Alles erreichbar mit Daumen |
| 📜 **Scroll & Tap** | Hauptnavigation durch Listen und Tippen |
| 🎨 **Mittelalter-Stil** | Pergament-Optik, Siegelwachs-Buttons, Holzrahmen |
| 🔔 **Klare Feedback-Loops** | Jede Aktion zeigt sofort das Ergebnis |
| 🧭 **Max. 3 Taps** | Jede Aktion in max. 3 Schritten erreichbar |

---

## 🏠 Hauptbildschirm

Der Hauptbildschirm zeigt alle wichtigen Infos auf einen Blick und dient als Ausgangspunkt für alles.

### Layout

```
┌─────────────────────────────────┐
│  ☀️ SOMMER · Anno 1425          │
│  📍 Augsburg                     │
│  ⏳ Aktionen: ●●●○○○  2/3       │
├─────────────────────────────────┤
│                                 │
│  👤 Heinrich Steinbach          │
│  🎂 30 Jahre · 🔨 Schmied       │
│  📋 Handelsherr                 │
│                                 │
│  ❤️ ██████████░░ 78             │
│  ⭐ ██████░░░░░░ 55             │
│  💰 234 Gold                    │
│  👁️ ███░░░░░░░░░ 12             │
│  ✝️ ██████████░░ 72             │
│                                 │
├─────────────────────────────────┤
│                                 │
│  📰 Neuigkeiten:                │
│  "Konrad Falkenberg wurde zum   │
│   Ratsherren gewählt."          │
│  "Getreidepreise steigen."      │
│                                 │
├─────────────────────────────────┤
│                                 │
│  [🏘️ Stadt]  [👤 Charakter]     │
│  [👨‍👩‍👧‍👦 Familie]  [📊 Betriebe]   │
│                                 │
└─────────────────────────────────┘
     🏘️      👤      👨‍👩‍👧‍👦     ⚙️
    Stadt  Charakter Familie  Menü
```

### Elemente

| Element | Funktion |
|---|---|
| **Header** | Aktuelle Saison, Jahr, Stadt, verbleibende Aktionen |
| **Charakter-Karte** | Name, Alter, Beruf, Titel, wichtige Werte als Balken |
| **Neuigkeiten** | Letzte Events, Gerüchte, Weltereignisse |
| **Quick-Buttons** | Schnellzugriff auf die 4 Hauptbereiche |
| **Bottom-Navigation** | Feste Navigationsleiste (immer sichtbar) |

---

## 🏘️ Stadt-Menü

Orte nach Kategorien sortiert. Gesperrte Orte zeigen ein Schloss. Saisonale Events werden hervorgehoben.

```
┌─────────────────────────────────┐
│  🏘️ STADT · Augsburg            │
│  ☀️ Sommer · ⏳ 2/3 Aktionen    │
├─────────────────────────────────┤
│                                 │
│  🏠 PRIVAT                      │
│  ├─ 🏡 Dein Zuhause             │
│                                 │
│  💼 WIRTSCHAFT                   │
│  ├─ 🔨 Deine Schmiede    ⭐⭐    │
│  ├─ 🏪 Marktplatz               │
│  ├─ 🏦 Kontor/Bank       🔒     │
│                                 │
│  🏛️ POLITIK                     │
│  ├─ 🏛️ Rathaus                  │
│  ├─ ⚖️ Gericht           🔒     │
│  ├─ 📜 Zunfthalle               │
│                                 │
│  ⛪ KIRCHE & BILDUNG             │
│  ├─ ⛪ Kirche/Dom                │
│  ├─ 📚 Universität       🔒     │
│  ├─ 🏥 Hospital                 │
│                                 │
│  🍺 SOZIALES                    │
│  ├─ 🍺 Taverne                  │
│  ├─ 🎪 Sommerturnier ☀️  NEU!   │
│  ├─ 💀 Hintergasse       🔒     │
│                                 │
│  🗺️ AUßERHALB                   │
│  ├─ 🌾 Bauernland               │
│  ├─ 🌲 Wald                     │
│  ├─ ⛏️ Bergwerk          🔒     │
│                                 │
└─────────────────────────────────┘
```

---

## 🔨 Ort-Detail (Beispiel: Schmiede)

```
┌─────────────────────────────────┐
│  🔨 DEINE SCHMIEDE  ⭐⭐ Mittel  │
│  ⏳ 1 Aktion                    │
├─────────────────────────────────┤
│                                 │
│  👷 Arbeiter: 4/5               │
│  📦 Lager:                      │
│     🗡️ Schwerter (3)            │
│     🛡️ Rüstungen (1)           │
│     🔧 Werkzeuge (5)            │
│  💰 Gewinn letzte Saison: 45g   │
│                                 │
├─────────────────────────────────┤
│                                 │
│  [⚒️ Produzieren]        1 Aktion│
│  [👷 Arbeiter einstellen]1 Aktion│
│  [📦 Lager → Markt]      1 Aktion│
│  [🏗️ Ausbauen (150g)]   1 Aktion│
│  [📋 Gildenauftrag]      1 Aktion│
│                                 │
│  [← Zurück zur Stadt]          │
│                                 │
└─────────────────────────────────┘
```

---

## 👤 Charakter-Bildschirm

```
┌─────────────────────────────────┐
│  👤 CHARAKTER                    │
├─────────────────────────────────┤
│                                 │
│  Heinrich Steinbach             │
│  🎂 30 Jahre · 🔨 Schmied       │
│  📋 Titel: Handelsherr          │
│  🏆 Stand: Handwerker           │
│                                 │
│  ── ATTRIBUTE ──                │
│  💪 Stärke:      ████████░░ 76  │
│  🎯 Geschick:    ██████░░░░ 58  │
│  🗣️ Charisma:    █████░░░░░ 45  │
│  🧠 Intelligenz: ███████░░░ 63  │
│  🙏 Frömmigkeit: ██████░░░░ 55  │
│                                 │
│  ── SEKUNDÄRWERTE ──            │
│  ❤️ Gesundheit:  ████████░░ 78  │
│  ⭐ Ansehen:     ██████░░░░ 55  │
│  💰 Reichtum:    234 Gold       │
│  👁️ Verdacht:    ██░░░░░░░░ 12  │
│  ✝️ Glaube:      ████████░░ 72  │
│                                 │
│  ── TRAITS ──                   │
│  🔥 Ehrgeizig · 💪 Zäh          │
│                                 │
│  ── BERUF ──                    │
│  🔨 Schmied (Meister)           │
│  📜 Gilde: Schmiedegilde        │
│  🏆 Rang: Gildenmeister         │
│                                 │
│  [📊 Abgeleitete Aktionen]      │
│  [📜 Lebenslauf]                │
│                                 │
└─────────────────────────────────┘
```

---

## 👨‍👩‍👧‍👦 Familie- & Beziehungs-Bildschirm

```
┌─────────────────────────────────┐
│  👨‍👩‍👧‍👦 FAMILIE                     │
├─────────────────────────────────┤
│                                 │
│  💑 EHEPARTNER                  │
│  ├─ Anna Steinbach (28)         │
│  │  ❤️ ████████░░ 82 (Vertraut) │
│  │  [🗣️ Reden] [🎁 Geschenk]   │
│  │  [👶 Kind] [🏡 Abend]        │
│                                 │
│  👶 KINDER                      │
│  ├─ 👦 Friedrich (8)     ❤️ 75  │
│  │  💪32 🎯28 🗣️25 🧠41 🙏30   │
│  │  [📚 Erziehen] [🗡️ Training] │
│  │                              │
│  ├─ 👧 Margarethe (5)    ❤️ 70  │
│  │  💪18 🎯35 🗣️42 🧠38 🙏28   │
│  │  [🤱 Kümmern]                │
│                                 │
│  👴 ELTERN                      │
│  ├─ Wilhelm Steinbach (61) ❤️55 │
│                                 │
│  ── BEZIEHUNGEN ──              │
│  🤝 Hans der Brauer       ❤️ 65 │
│  ⛪ Pater Thomas          ❤️ 58 │
│  😡 Konrad Falkenberg     💔-45 │
│  😐 Krämer Ludwig        😐 +12 │
│                                 │
│  [👤 Person antippen für        │
│   verfügbare Aktionen]          │
│                                 │
└─────────────────────────────────┘
```

### Personen-Detail (Tap auf NPC)

```
┌─────────────────────────────────┐
│  👤 Konrad Falkenberg            │
│  🎂 35 Jahre · 🚢 Fernhändler   │
│  💔 Beziehung: -45 (Rivale)     │
├─────────────────────────────────┤
│                                 │
│  ── VERFÜGBARE AKTIONEN ──      │
│                                 │
│  😡 FEINDLICHE AKTIONEN         │
│  [📜 Verleumden]     +5 Verdacht│
│  [🔧 Sabotieren]    +15 Verdacht│
│  [📜 Anklagen]       Beweise?   │
│  [💰 Unterbieten]    Gold nötig │
│                                 │
│  🤝 FRIEDLICHE AKTIONEN         │
│  [🗣️ Unterhalten]    Charisma   │
│  [🤝 Friedensangebot] Charisma  │
│  [🎁 Geschenk]       50–200g   │
│                                 │
│  [← Zurück]                    │
│                                 │
└─────────────────────────────────┘
```

---

## 📊 Betriebe-Bildschirm

```
┌─────────────────────────────��───┐
│  📊 DEINE BETRIEBE               │
│  📋 Titel: Handelsherr (2/2)    │
├─────────────────────────────────┤
│                                 │
│  🔨 Schmiede         ⭐⭐ Mittel │
│  👷 4/5 Arbeiter                │
│  📦 9 Waren im Lager            │
│  💰 +45g letzte Saison          │
│  [Verwalten →]                  │
│                                 │
│  ─────────────────────────      │
│                                 │
│  🍺 Brauerei          ⭐ Klein  │
│  👷 1/2 Arbeiter                │
│  📦 3 Waren im Lager            │
│  💰 +12g letzte Saison          │
│  [Verwalten →]                  │
│                                 │
│  ─────────────────────────      │
│                                 │
│  💰 Gesamt letzte Saison: +57g  │
│  📈 Nächster Titel: Ehrbarer    │
│     Kaufmann (300g, Meister)    │
│                                 │
└─────────────────────────────────┘
```

---

## ⏳ Saison-Übergang

Wenn alle 3 Aktionen verbraucht sind oder der Spieler manuell weiterspringt:

```
┌─────────────────────────────────┐
│                                 │
│    ☀️ SOMMER 1425 → ENDE        │
│                                 │
│  ── ZUSAMMENFASSUNG ──          │
│                                 │
│  💰 Einnahmen:      +57 Gold    │
│  💸 Ausgaben:       –22 Gold    │
│  📦 Produziert:     6 Waren     │
│  ⭐ Ansehen:        +3          │
│  ❤️ Gesundheit:     –2          │
│  👁️ Verdacht:       0           │
│                                 │
│  📰 Events:                     │
│  • Deine Schmiede produzierte   │
│    3 Schwerter (automatisch)    │
│  • Getreidepreise gestiegen     │
│  • Konrad Falkenberg verbreitet │
│    Gerüchte über dich (–3 ⭐)   │
│                                 │
│  ┌─────────────────────────┐    │
│  │  🍂 Weiter zum HERBST   │    │
│  └─────────────────────────┘    │
│                                 │
└─────────────────────────────────┘
```

---

## 📅 Jahresende

```
┌─────────────────────────────────┐
│                                 │
│    📅 JAHRESBILANZ 1425          │
│                                 │
│  ── FINANZEN ──                 │
│  💰 Einnahmen gesamt:  +228 Gold│
│  💸 Ausgaben gesamt:   –145 Gold│
│  💰 Steuern:           –23 Gold │
│  📈 Netto-Gewinn:      +60 Gold │
│  🏦 Vermögen:          294 Gold │
│                                 │
│  ── CHARAKTER ──                │
│  ⭐ Ansehen:   55 → 61  (+6)   │
│  ❤️ Gesundheit: 78 → 74  (–4)  │
│  👁️ Verdacht:  12 → 9   (–3)   │
│  ✝️ Glaube:    72 → 75  (+3)   │
│                                 │
│  ── FAMILIE ──                  │
│  👦 Friedrich ist jetzt 9       │
│  👧 Margarethe ist jetzt 6      │
│                                 │
│  ── HIGHLIGHTS ──               │
│  🏆 Gildenmeister geworden!     │
│  📜 1 Gildenauftrag erfüllt     │
│  😡 Neue Rivalität: Georg H.    │
│                                 │
│  ┌─────────────────────────┐    │
│  │  🌸 Weiter zu 1426      │    │
│  └─────────────────────────┘    │
│                                 │
└─────────────────────────────────┘
```

---

## 🎨 Aktions-Feedback

Jede Aktion zeigt sofort ein Ergebnis-Popup:

```
┌─────────────────────────────────┐
│                                 │
│    ⚒️ PRODUZIERT!                │
│                                 │
│    Du hast 2 Schwerter          │
│    geschmiedet.                 │
│                                 │
│    🗡️🗡️                         │
│                                 │
│    📦 Lager: Schwerter (5)      │
│    💰 Wert: ~75 Gold            │
│                                 │
│    ⏳ Aktionen übrig: 1/3       │
│                                 │
│  ┌─────────────────────────┐    │
│  │        OK ✅              │    │
│  └─────────────────────────┘    │
│                                 │
└─────────────────────────────────┘
```

### Event-Popup (Zufallsevent)

```
┌─────────────────────────────────┐
│                                 │
│    🦠 SEUCHE IN AUGSBURG!        │
│                                 │
│    Eine Pestwelle hat die Stadt │
│    erreicht. Die Bevölkerung    │
│    ist in Panik.                │
│                                 │
│    ❤️ Gesundheit: –10           │
│    💰 Heilmittel-Preise: +200%  │
│    👷 2 Arbeiter erkrankt       │
│                                 │
│  Was tust du?                   │
│  [🏥 Hospital (1 Aktion, 15g)]  │
│  [⛪ Beten (1 Aktion)]          │
│  [🏡 Zuhause bleiben]           │
│  [🌲 Stadt verlassen (riskant)] │
│                                 │
└─────────────────────────────────┘
```

---

## 🔔 Benachrichtigungen

Wichtige Events werden als Banner oben eingeblendet.

| Typ | Farbe | Beispiele |
|---|---|---|
| 🔴 **Dringend** | Rot | Anklage, Belagerung, Tod, Seuche |
| 🟡 **Wichtig** | Gelb | Wahl, Geburt, Rivale handelt |
| 🟢 **Info** | Grün | Gewinn, Auftrag erfüllt, Saison-Start |
| 🔵 **Historisch** | Blau | Weltereignisse (Buchdruck, Pest etc.) |

---

## ⚙️ Menü-Bildschirm

```
┌─────────────────────────────────┐
│  ⚙️ MENÜ                        │
├─────────────────────────────────┤
│                                 │
│  [📜 Lebenslauf]     Chronik    │
│  [🏆 Errungenschaften]          │
│  [📊 Statistiken]    Zahlen     │
│  [🏛️ Stadtinfo]     Gesetze    │
│  [📅 Historische Events]        │
│  [⚙️ Einstellungen]             │
│  [💾 Speichern]                 │
│                                 │
└─────────────────────────────────┘
```

---

## 📱 Bottom-Navigation

Die untere Navigationsleiste ist **immer sichtbar** und bietet schnellen Zugriff.

| Icon | Bereich | Funktion |
|---|---|---|
| 🏘️ | **Stadt** | Orte besuchen, Aktionen ausführen |
| 👤 | **Charakter** | Attribute, Traits, Beruf, Status |
| 👨‍👩‍👧‍👦 | **Familie** | Familie, Beziehungen, NPCs |
| ⚙️ | **Menü** | Einstellungen, Chronik, Speichern |

---

## 🎨 Visueller Stil

| Element | Stil |
|---|---|
| **Hintergrund** | Pergament-Textur, leicht vergilbt (Light) / Dunkles Pergament (Dark) |
| **Buttons** | Holzoptik mit Siegelwachs-Akzenten |
| **Schrift** | Mittelalterlich angehauchte Schrift (aber gut lesbar!) |
| **Icons** | Emojis (einfach, universal, kostenlos) |
| **Farben** | Warme Erdtöne: Braun, Gold, Dunkelrot, Dunkelgrün |
| **Animationen** | Minimal – sanftes Einblenden, Balken-Bewegungen |
| **Sound** | Optional: Mittelalterliche Musik, Ambience (Markt, Schmiede) |
| **Dark Mode** | Dunkles Pergament mit heller Schrift, gleiche Akzentfarben |