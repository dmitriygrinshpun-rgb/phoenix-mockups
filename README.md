# Phoenix Mockups

Standalone HTML/CSS/JS prototypes for Doodle's Phoenix product, iterated on outside the main app codebase for fast design exploration.

## Files

- `meeting-creation-v3_4.html` — New-event creation flow. Infers the event type (Group Poll / 1:1 / Sign-up Sheet / Booking Page) from two plain-language questions instead of a flat type picker, with a live status readout, auto-suggested capacity, an always-on shareable link, a calendar-grid time picker, and custom time rows with real date/time pickers.

## Running locally

Each file is self-contained — open it directly in a browser, or serve the folder:

```bash
python3 -m http.server 8931
```

Then visit `http://localhost:8931/<file>.html`.
