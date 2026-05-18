# Live Demo Script — Claude Code × Navi

Small, hands-on script for the finale of the Knowledge Café. ~5–7 minutes on stage.

## Before you go on stage

- Navi backend running (`flask run` or your usual start command), browser open to the dashboard on a second monitor / projected window.
- Terminal open in `C:\Users\JoãoPedroSousa\OneDrive - Product League\Bureaublad\navi` with Claude Code launched.
- The target file is `market-oracle/templates/index.html` (single-file vanilla HTML/CSS/JS, no build step — saves hot-reload on refresh).
- Have this script open on your phone or a third screen so you can glance at it.

## The pitch (15 seconds, into the room)

"Navi is on screen. I'm going to ask Claude Code to change how it looks — live, no preview, no safety net. Watch what one prompt does."

## Primary prompt (the one you'll actually type)

```
In market-oracle/templates/index.html, give the logo gradient a bolder
look — switch the cyan-to-blue gradient to a purple-to-pink gradient.
Also change the "LIVE" label next to the green dot to "🚀 STREAMING"
and make the pulse animation 30% faster. Keep everything else intact.
```

Then refresh the browser. The audience sees: new gradient, new label, faster pulse. ~30 seconds of magic.

## Fallback prompt (if the first one doesn't land cleanly)

```
In market-oracle/templates/index.html, find the .pick-card hover state
and add a glowing box-shadow: 0 0 20px rgba(167,139,250,0.6). Make the
cards visibly pop when I hover them.
```

Refresh, hover over any "AI Pick" card on the dashboard — the cards now glow purple.

## If you have extra time (the "wow" closer)

```
Add a small toggle in the top-right of the navbar that switches the
entire dashboard between light and dark mode. Use the existing
CSS custom properties — there's already a theme system in place.
```

This shows Claude Code reading existing code and extending it, not just patching.

## What to say while Claude Code is working

- "I'm typing English. It's reading 2,000 lines of HTML and figuring out where to edit."
- "If you'd asked me a year ago how long this would take, I'd have said an hour."
- "This is the part where I would have googled and lost my flow."
- When the edits appear: "And… refresh."

## After the demo

Pivot straight into the closing slide ("what are you going to do with what you know?"). Don't linger.

## Risk plan

- **If Claude Code edits the wrong file**: just say "and here's the part where you stay in the loop" — show the diff, accept or reject, move on. Honest is better than slick.
- **If the browser doesn't reload**: hit Ctrl-Shift-R explicitly, narrate as "harder refresh."
- **If a prompt produces nothing visible**: use the fallback prompt — the hover-glow change is impossible to miss.
- **Last resort**: read the prompt aloud, paste it, and let Claude Code work while you talk. The "watching it think" is half the magic.
