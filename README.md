# Artograph

**Live: [art.sala.company](https://art.sala.company)** · part of [go.sala.company](https://go.sala.company)

A Spirograph in your browser. Pick a ring and a wheel, put the pen in a hole, and let it roll. Everything runs in one HTML file, with nothing to install and no sign-up.

[![Artograph](https://go.sala.company/img/artograph.jpg)](https://art.sala.company)

## How to use it

The controls are numbered steps that make a first drawing easy. You don't have to follow them in order: you can come back to any step at any time.

1. **Start with blank paper**, white or black.
2. **Choose how the wheel rolls:** inside a ring, or around a centre gear.
3. **Pick a ring:** 96, 105, 144 or 150 teeth, as in the classic set. Around a gear, pick a centre gear of 24 to 84 teeth.
4. **Pick a wheel:** 17 wheels from 24 to 84 teeth. Each one previews the pattern it makes with your ring and pen hole, and shows how many points that pattern has. A gold dot marks a good match: 5 to 24 points, quick to draw. Very busy patterns are marked *dense*. Wheels that would run off the paper are greyed out.
5. **Put the pen in a hole:** near the centre gives gentle waves, the middle gives rounded petals, and near the edge gives sharp points. *Start at tooth* turns the pattern. **Fit between the points** turns the next layer by half a point, so it lands in the gaps of the last one.
6. **Choose a pen:** ten gel-pen colors (including gold and white for black paper) or any color you like, and a line width. A sample stroke shows the result, with a suggested width for the pattern.
7. **Draw:** press Draw and the page scrolls back to the paper. Tap the paper to pause. Drag clockwise around the paper to turn the wheel by hand instead. The step also shows how long the pattern will take at the current speed.
8. **Add a rosette:** repeat the pattern 3, 4, 6, 8 or 12 times, evenly turned, optionally with a new pen color for each copy.
9. **Keep it:** save a 3000 × 3000 PNG or an SVG for printing and pen plotters, or copy a share link that carries the whole drawing.

Changing the pen mid-drawing switches pens. Changing a gear, hole or start tooth lifts the wheel, so the next drawing starts a new layer on top.

## The maths

A pattern closes when the wheel's teeth line up with the ring's again. With a ring of *R* teeth and a wheel of *r* teeth, and *g* the largest number that divides both:

- the pattern has **R ÷ g points**
- the wheel goes round the ring **r ÷ g times** before it closes

That's why a 105-tooth ring and a 63-tooth wheel (g = 21) make a quick 5-point star, while 105 and 52 (g = 1) make a dense 105-point pattern. The wheel ratings, the time estimate and the width suggestion all come from these two numbers.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app: markup, styles and script |
| `artograph/`, `spirograph/` | Redirects from earlier addresses; they keep share-link drawings |
| `CNAME` | The custom domain, `art.sala.company` |

GitHub Pages serves the `main` branch at [art.sala.company](https://art.sala.company), and every push goes live in about a minute.

Fonts come from Google Fonts: Monoton for the title and step numbers, IM Fell English for step headings, Instrument Sans and JetBrains Mono for everything else.
