# 🎄 Familien Adventskalender

Ein interaktiver digitaler Adventskalender mit Familienbildern für jeden Tag im Dezember.

## 🚀 Setup-Anleitung

### Schritt 1: Bilder vorbereiten
1. Wähle 24 Familienbilder aus (eins für jeden Tag)
2. Benenne sie um zu: `1.jpg`, `2.jpg`, `3.jpg`, ... `24.jpg`
   - Alternativ: `.jpeg`, `.png` oder `.gif` - der Kalender erkennt das Format automatisch!
   - Du kannst auch verschiedene Formate mischen (z.B. `1.jpg`, `2.png`, `3.jpeg`)

### Schritt 2: Bilder auf GitHub hochladen
1. Erstelle einen Ordner `images` in deinem Repository:
   - Klicke auf "Add file" → "Create new file"
   - Gib als Dateinamen ein: `images/placeholder.txt`
   - Schreibe irgendwas rein und klicke "Commit changes"

2. Gehe in den `images` Ordner
3. Klicke "Add file" → "Upload files"
4. Lade deine 24 umbenannten Bilder hoch
5. Klicke "Commit changes"

### Schritt 3: GitHub Pages aktivieren
1. Gehe zu Settings → Pages
2. Bei "Source": Wähle "Deploy from a branch"
3. Bei "Branch": Wähle "main" und "/ (root)"
4. Klicke "Save"

### Schritt 4: Fertig! 🎉
Dein Kalender ist jetzt online unter:
```
https://emsibeach.github.io/Adventskalender/advent-calendar.html
```

## 🎮 Funktionen

- ✅ 24 Türchen, eines für jeden Tag im Dezember
- ✅ Türchen öffnen sich nur ab dem jeweiligen Tag
- ✅ Heutiges Türchen wird hervorgehoben (pulsierend)
- ✅ Geöffnete Türchen werden markiert
- ✅ Zufällige Fragen zu jedem Bild: "Weißt du noch?", "Wo war das?", etc.
- ✅ Weihnachtliche Schnee-Animation
- ✅ Responsive Design für Handy & Desktop

## 🔧 Technische Details

- Keine Datenbank benötigt
- Bilder werden direkt von GitHub geladen
- Geöffnete Türchen werden im Browser-LocalStorage gespeichert
- Funktioniert vollständig im Browser (nur HTML/CSS/JavaScript)

## 📱 Teilen

Teile einfach den Link mit deiner Familie:
```
https://emsibeach.github.io/Adventskalender/advent-calendar.html
```

Jedes Familienmitglied kann den Kalender täglich besuchen und neue Türchen öffnen!

## ⚙️ Anpassungen

### Datum für Tests ändern
In `advent-calendar.html` die Funktion `getCurrentDate()` anpassen:
```javascript
function getCurrentDate() {
    // Für Tests kannst du hier ein festes Datum setzen:
    // return { month: 12, day: 10 };
    
    const now = new Date();
    return {
        month: now.getMonth() + 1,
        day: now.getDate()
    };
}
```

### Neue Fragen hinzufügen
Im Array `questions` in `advent-calendar.html` können weitere Fragen ergänzt werden.

### Design anpassen
Alle Farben und Styles sind im `<style>`-Bereich am Anfang der HTML-Datei definiert.

## 🎄 Viel Spaß mit dem Adventskalender!
