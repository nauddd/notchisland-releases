# Notch Island installeren

Notch Island maakt van de notch van je MacBook een klein bedieningspaneel. Je ziet er wat er speelt in Spotify of Muziek, je volgende afspraak, een snelle notitie en een plek om bestanden even neer te zetten. Ook het volume en de helderheid verschijnen er netjes in.

## Wat heb je nodig?

- Een **MacBook met een notch**: een MacBook Pro 14" of 16" (2021 of nieuwer) of een MacBook Air (2022 of nieuwer).
- **macOS 14 Sonoma** of nieuwer.

Zonder notch (of met alleen een extern scherm) toont de app niets.

## Installeren

1. Download het bestand **NotchIsland-….dmg** onder *Assets*.
2. Open het bestand. Er verschijnt een venster.
3. Sleep **Notch Island** naar de map **Programma's**.
4. Open Notch Island vanuit Programma's.

## "Niet geopend" / "Not Opened"

De eerste keer zegt macOS dat het niet kon controleren of de app vrij is van malware. In het Engels heet die melding *"NotchIsland" Not Opened*. Dat is normaal: de app staat niet in de App Store en is niet bij Apple aangemeld. Zo open je hem toch.

1. Klik in de melding op **Gereed** (Engels: **Done**). Klik **niet** op *Verplaats naar prullenmand* (*Move to Bin*).
2. Open **Systeeminstellingen → Privacy en beveiliging** (Engels: **System Settings → Privacy & Security**).
3. Scrol helemaal naar beneden naar **Beveiliging** (*Security*). Daar staat dat NotchIsland is geblokkeerd. Klik op **Toch openen** (*Open Anyway*).
4. Bevestig met je wachtwoord of Touch ID, en klik in de nieuwe melding nog een keer op **Toch openen** (*Open Anyway*).

Dit hoeft maar één keer.

De knop **Toch openen** staat er ongeveer een uur nadat je de app probeerde te openen. Zie je hem niet? Open de app dan eerst nog een keer vanuit Programma's, klik op **Gereed** (*Done*), en kijk opnieuw.

### Lukt het niet?

Open **Terminal** (via Spotlight: ⌘-spatie, typ "Terminal"). Plak deze regel en druk op Enter:

```
xattr -dr com.apple.quarantine /Applications/NotchIsland.app
```

Je ziet geen bericht; dat is goed. Open daarna Notch Island gewoon vanuit Programma's. Deze regel haalt alleen de blokkade weg van deze ene app.

## Toestemmingen

De app vraagt pas om toestemming op het moment dat je een functie gebruikt. Je mag alles weigeren; dan werkt alleen dat ene onderdeel niet.

| Toestemming | Waarvoor |
|---|---|
| **Agenda** | Je volgende afspraken in de notch, en een seintje 10 minuten van tevoren. |
| **Spotify en Muziek** (Automatisering) | Laten zien wat er speelt, en afspelen, pauzeren en doorspoelen vanuit de notch. |
| **Notities** (Automatisering) | Je notitie uit de notch bewaren in de Notities-app, alleen als je daar zelf op klikt. |
| **Toegankelijkheid** | De volume- en helderheidstoetsen opvangen, zodat de balk in de notch verschijnt in plaats van de melding van macOS. |

De app leest of bewaart nooit wat je typt. Bij Toegankelijkheid kijkt hij alleen naar de volume- en helderheidstoetsen.

## Tip: slepen naar de notch

Je kunt bestanden naar de notch slepen om ze daar even neer te zetten. Gaat er dan steeds Mission Control open? Zet dit uit:

**Systeeminstellingen → Bureaublad en Dock → Mission Control → "Sleep vensters naar bovenkant van scherm om Mission Control te openen"**.

## Updates

Komt er een nieuwe versie, dan zie je dat in de notch: **"Nieuwe versie … beschikbaar"**.

1. Klik op **Bekijk** om te zien wat er nieuw is.
2. Klik op **Download**. Het bestand komt in je map Downloads en gaat vanzelf open.
3. Sleep Notch Island weer naar **Programma's** en kies **Vervang**.

Je kunt ook zelf zoeken: klik op het Notch Island-icoon in de menubalk → **Zoek naar updates…**.

Na een update moet je soms de toestemming voor **Toegankelijkheid** opnieuw aanzetten: Systeeminstellingen → Privacy en beveiliging → Toegankelijkheid. Zet Notch Island uit en weer aan, of verwijder hem met **–** en voeg hem opnieuw toe.

## Optioneel: Claude Code

Gebruik je Claude Code? Dan kun je de toestemmingsvragen van Claude Code in de notch beantwoorden, en krijg je een melding als Claude klaar is.

Kies daarvoor in het menubalk-menu **Koppel aan Claude Code…**. De app legt eerst uit wat er verandert, en maakt een back-up van je instellingen. Met **Ontkoppel Claude Code** haal je het weer weg.

Gebruik je Claude Code niet, dan hoef je hier niets mee te doen.

## Stoppen of verwijderen

- **Stoppen:** menubalk-icoon → **Stop**.
- **Niet meer automatisch openen:** menubalk-icoon → zet **Open bij inloggen** uit.
- **Verwijderen:** stop de app en sleep hem uit Programma's naar de prullenmand.
