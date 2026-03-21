# Partida Fría · Pastelería
 
A mobile-first web app to manage the cold station and pastry section of a fine dining kitchen (50–100 covers). Built as a single HTML file — no dependencies, no build step.
 
## What it does
 
The app acts as a daily operations dashboard for a professional kitchen's cold and pastry sections. It covers:
 
- **Daily checklists** — opening, cold mise en place, pastry mise en place, service, and closing tasks, each with a progress bar and individual reset buttons
- **Timbre (pass) loading** — separate checklists for the sweet (left) and savory (right) sides of the pass, with a warning banner to load before first cover
- **Cámaras (cold storage)** — minimum stock checklist for the front fridge, plus reference lists for the back fridge and freezer
- **Recipes** — collapsible recipe cards for the section's key preparations (mantequilla ahumada, mejillones en escabeche, tartare, flanes, sabayón, etc.)
- **Orders (Pedidos)** — weekly order composer per supplier with checkable item lists, quantity inputs, notes, and a WhatsApp send button
- **Weekly schedule** — day-by-day production and delivery calendar with alerts for key deadlines
- **Supplier info** — contact details and order frequency for each provider
 
## Tech
 
- Pure HTML, CSS, and vanilla JavaScript — a single self-contained file
- No framework, no backend, no build tooling required
- Designed for mobile (PWA-ready meta tags, safe area insets, sticky nav, large touch targets)
- State is persisted to `localStorage` so checked items survive a page reload
- Typography: Cormorant Garamond (labels) + DM Mono (UI/data), loaded from Google Fonts
- Color palette: warm linen, terracotta, aged teal — tuned for readability in a kitchen environment
 
## File structure
 
```
Tramo-Frio-Pasteleria/
├── index.html      # Current production version
├── index1.0.html   # Previous version / backup
└── README.md
```
 
## Usage
 
Open `index.html` in any modern mobile browser — no server needed. To use it across devices, host it anywhere that serves static files (GitHub Pages, Netlify, etc.) and add it to the home screen as a PWA.
 
For local use:
 
```bash
# Clone the repo
git clone https://github.com/mch-codes/Tramo-Frio-Pasteleria.git
 
# Open in browser
open https://mch-codes.github.io/Tramo-Frio-Pasteleria/
```
 
## Context
 
*Tramo Frío* is the cold section of a fine dining restaurant kitchen. This tool was built to replace paper checklists and WhatsApp message chains for daily mise en place, stock control, and supplier orders — keeping everything in one place on a phone during service.
 
## License
 
MIT
