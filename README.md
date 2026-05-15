# Join — Kanban Project Management Tool

Ein browserbasiertes Kanban-Tool zur Aufgabenverwaltung mit Firebase Realtime Database als Backend.

---

## Starten

Kein Build-Tool erforderlich. Einfach `index.html` im Browser öffnen — oder mit einem Live-Server:

```bash
npm install -g live-server
live-server
```

---

## Features

- Aufgaben erstellen, bearbeiten und löschen
- Kanban-Board mit Drag & Drop (To-do, In Progress, Awaiting Feedback, Done)
- Kontaktverwaltung
- Prioritäten (Urgent, Medium, Low) und Deadlines
- Summary-Dashboard mit Key Metrics
- Login & Registrierung
- Responsive Design

---

## Technologien

| Technologie | Verwendung |
|---|---|
| Vanilla JavaScript | Logik & DOM |
| HTML / CSS | Markup & Styling |
| Firebase Realtime Database | Backend / Datenpersistenz |

---

## Firebase

Die App kommuniziert direkt über die Firebase REST API — kein SDK, keine Konfigurationsdatei nötig. Die Datenbankadresse ist in `scripts/db.js` hinterlegt.

Folgende Operationen werden verwendet:

| Methode | Funktion |
|---|---|
| GET | `loadData(path)` |
| POST | `postData(path, data)` |
| PUT | `putData(path, data)` |
| DELETE | `deleteData(path)` |

---

## Projektstruktur

```
JoinMy/
├── scripts/          # JavaScript-Logik (Board, Tasks, Contacts, Login, ...)
├── templates/        # HTML-Templates als JS-Strings
├── styles/           # CSS-Dateien und Media Queries
├── assets/           # Bilder, Icons, Fonts
├── index.html        # Einstiegspunkt (Login)
├── summary.html
├── board.html
├── add-task.html
├── add-contact.html
└── register.html
```