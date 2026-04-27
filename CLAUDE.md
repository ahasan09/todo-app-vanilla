# Hasan-ToDo-App

Vanilla JavaScript to-do application supporting create, edit, delete, search, and status filtering, with data persisted to localStorage.

## Tech Stack
- Vanilla JavaScript (ES5)
- HTML5 / CSS3
- No frameworks or build tools

## Project Structure
```
Hasan-ToDo-App/
  index.html          # Main entry point
  app.js              # All application logic (single-file IIFE)
  app.css             # Styles
  modified-index.html # Alternate/experimental HTML version
  img/                # Logo images
```

## Development
No dependencies to install. Open `index.html` directly in a browser:
```bash
open Hasan-ToDo-App/index.html
# or serve with:
python3 -m http.server 8080
```

## Key Notes
- All logic is in a single `app.js` file using an IIFE pattern.
- Tasks are stored in `localStorage` — no backend required.
