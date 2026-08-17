# Phoenix Mockups

Standalone HTML/CSS/JS prototypes for Doodle's Phoenix product, iterated on outside the main app codebase for fast design exploration.

## Files

- `index.html` (+ `index_files/`) — The Doodle marketing homepage, saved as the entry point for this prototype. Its "Create a Doodle" / "Try Doodle" buttons link to `meeting-creation-v3_4.html` instead of the live site.
- `meeting-creation-v3_4.html` — New-event creation flow, reached from the homepage above. Infers the event type (Group Poll / 1:1 / Sign-up Sheet / Booking Page) from two plain-language questions instead of a flat type picker, with a live status readout, auto-suggested capacity, an always-on shareable link, a calendar-grid time picker, and custom time rows with real date/time pickers. Opens with "Your name" / "Your email" fields since this flow runs for signed-out visitors, and the primary action always reads "Sign up and share".

## Running locally

Serve the folder and start from the homepage:

```bash
python3 -m http.server 8931
```

Then visit `http://localhost:8931/index.html`.
