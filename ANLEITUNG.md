# Portfolio — Anleitung

Dein Portfolio als normaler Ordner. Alles darin gehört dir, du brauchst dafür
niemanden mehr.

```
portfolio/
├── index.html      ← die Seite selbst (Texte und Aufbau)
├── media/          ← alle Videos und Bilder
└── ANLEITUNG.md    ← diese Datei
```

---

## 1. Ansehen

Doppelklick auf `index.html`. Die Seite öffnet sich im Browser. Das funktioniert
ohne Internet und ohne dass irgendetwas online ist.

---

## 2. Ein Video austauschen

Das ist der häufigste Fall und dauert eine Minute.

1. Schau im Ordner `media/` nach, wie die alte Datei heißt.
   Die Namen sagen, wo sie sitzen: `vision-ekstase_01_promo.mp4` ist das erste
   Video bei Vision Ekstase, `kanal_01_grwm.mp4` das erste auf deinem Kanal.
2. Benenne dein neues Video **genau so** wie das alte.
3. Lege es in `media/` und überschreibe die alte Datei.

Fertig. Du musst nichts am `index.html` ändern.

**Format:** MP4, hochkant 9:16, Ton darf drin bleiben.
**Größe:** unter 5 MB pro Video, sonst lädt die Seite auf dem Handy langsam.
Wenn dein Video größer ist, kannst du es kostenlos verkleinern —
in CapCut beim Export die Auflösung auf 720p stellen.

Zu jedem Video gibt es eine `_vorschau.jpg`. Das ist das Standbild, das zu
sehen ist, bevor das Video startet. Du kannst es mitaustauschen, musst aber nicht —
ohne passendes Vorschaubild bleibt die Fläche kurz dunkel.

---

## 3. Ein neues Projekt hinzufügen

1. Öffne `index.html` in einem Texteditor (TextEdit reicht, oder VS Code).
2. Suche nach **NEUES PROJEKT HINZUFUEGEN**. Dort steht eine fertige Vorlage
   zwischen `***** ANFANG VORLAGE *****` und `***** ENDE VORLAGE *****`.
3. Kopiere alles zwischen diesen beiden Markierungen.
4. Füge es an der Stelle ein, an der das Projekt stehen soll — die Projekte
   stehen zwischen `<section id="arbeiten">` und `</section>`, jedes beginnt
   mit `<article class="case">`.
5. Ersetze die GROSSGESCHRIEBENEN Stellen durch deine Texte.
6. Lege deine Videos in `media/` und trage die Dateinamen ein.

**Wichtig:** Beim Einfügen die Zeichen `<!--` am Anfang und `-->` am Ende
weglassen. Solange die dranstehen, ist der Block ein Kommentar und wird nicht
angezeigt.

Willst du mehr als zwei Videos im Projekt? Kopiere einen der
`<figure class="phone">`-Blöcke und ändere den Dateinamen.

---

## 4. Einen Text ändern

`index.html` im Texteditor öffnen, den Satz suchen, überschreiben, speichern.
Lass die spitzen Klammern in Ruhe — nur den Text dazwischen anfassen.

---

## 5. Online stellen

Einmalig einrichten, danach ist jede Änderung in zwei Minuten live.

**Schritt 1 — GitHub**

1. Konto anlegen auf github.com (kostenlos).
2. Oben rechts auf **+** → **New repository**.
3. Name: `portfolio`. Auf **Public** lassen. **Create repository**.
4. Auf der nächsten Seite: **uploading an existing file**.
5. Ziehe `index.html` und den ganzen Ordner `media` in das Fenster.
6. Unten auf **Commit changes**.

**Schritt 2 — Vercel**

1. Konto anlegen auf vercel.com (kostenlos, "Hobby"-Plan) und dabei
   **Continue with GitHub** wählen.
2. **Add New** → **Project** → dein Repository `portfolio` → **Import**.
3. Nichts einstellen, einfach **Deploy**.
4. Nach etwa einer Minute bekommst du deine Adresse, zum Beispiel
   `portfolio-rosalina.vercel.app`. Das ist der Link, den du verschickst.

**Ab jetzt:** Wenn du etwas änderst, lädst du die geänderte Datei bei GitHub
hoch (im Repository auf die Datei klicken → Stift → ersetzen → Commit).
Vercel merkt das von allein und aktualisiert die Seite. **Die Adresse bleibt
immer dieselbe** — auch alte Links funktionieren weiter.

Beides ist und bleibt kostenlos, solange die Seite privat und ohne Werbung ist.

---

## 6. Was du besser nicht anfasst

- Alles zwischen `<style>` und `</style>` — das ist das Design.
- Alles zwischen `<script>` und `</script>` — das sind die Pfeile, die
  Ton-Buttons und die Steuerung, welches Video gerade läuft.

Wenn doch mal etwas kaputtgeht: Die Datei ist nur Text. Mach dir vorher eine
Kopie, dann kannst du jederzeit zurück.

---

## 7. Gut zu wissen

- Die Seite lädt nur die Videos, die gerade sichtbar sind. Deshalb ist sie
  schnell, auch auf dem Handy.
- Videos starten stumm — das schreiben alle Browser so vor. Über den kleinen
  Lautsprecher unten rechts im Video schaltet man den Ton an.
- Bei Videoreihen, die breiter sind als der Bildschirm, erscheinen links und
  rechts Pfeile zum Durchklicken.
