# 💌 Happy Boyfriend's Day

An interactive, one-screen-at-a-time love page built with vanilla HTML, CSS and JavaScript. Open the envelope, read the letter, spin the wheel, scratch open the truths, and redeem a coupon.

Fully responsive on mobile and laptop. No frameworks, no build step, no dependencies.

## ✨ Flow

| Step | Screen | What happens |
|------|--------|--------------|
| 1 | **Envelope** | Tap anywhere to begin |
| 2 | **Letter** | A short note and a mini collage |
| 3 | **Spin the wheel** | 8 emoji date-night options; the next button unlocks after the first spin |
| 4 | **Scratch cards** | 4 cards to scratch open; the next button unlocks once all are uncovered |
| 5 | **Coupon** | Tap the coupon and a "REDEEMED" stamp animates on. Includes a "watch it again" replay button |

Progress dots at the top track where you are.

## 🚀 Run it

No setup needed.

1. Download `boyfriends-day.html`
2. Open it in any browser

To host it, drop the file on GitHub Pages, Netlify or Vercel.

## 🎨 Customize

Everything lives in the one HTML file.

**Letter text**
Edit the content inside the `#s-letter` section.

**Scratch card messages** (keep it at 4, or update the `of 4` counter too)
```js
const truths = [
  "you make ordinary days feel special",
  "i still get a little nervous around you",
  "you're my favourite notification",
  "i'd choose you again, every time"
];
```

**Wheel options** (icons show on the wheel, labels show in the result)
```js
const optionLabels = ["Movie Night", "His Fav Meal", ...];
const optionIcons  = ["🎬", "🍝", ...];
```
Keep both arrays the same length.

**Coupon text**
Edit the `.coupon` block in the `#s-coupon` section.

**Colors**
Change the CSS variables at the top of the file:
```css
:root{
  --teal:#b3261e;   /* main red */
  --coral:#e2574a;  /* accent */
  --mint:#fdecea;   /* background */
}
```
The variable names are legacy from the first green version, but the values are the red theme.

## 🧱 Tech

- HTML5, CSS3, vanilla JS
- Canvas API for the scratch cards
- Inline SVG for the wheel and envelope
- Google Fonts: Fraunces, Caveat, Quicksand

## 📱 Responsive

Full-bleed on every screen size. Cards, wheel and buttons scale up on screens wider than 700px.

## 📁 Structure

```
index.html   # the whole project
README.md
```

## 🙌 Credits

First draft generated with AI, customized and crafted by **Storymint Studio**.

Follow for a new UI drop every week: [@storymint.studio](https://instagram.com/storymint.studio)
