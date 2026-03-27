# 🏋️ IRONFORGE GYM — Website

**WHERE LIMITS BREAK**  
High-converting single-page gym website. Built with vanilla HTML, CSS, and JavaScript. No frameworks. No dependencies (except Google Fonts).

---

## 🚀 Quick Start

1. Download `ironforge-gym.html`
2. Open it in any browser
3. That's it — fully functional, no build step required

---

## 📐 Site Structure

| Section | Description |
|---|---|
| **Navigation** | Sticky bar, transparent → frosted glass on scroll, mobile hamburger |
| **Hero** | Full-viewport, animated hex shape, dual CTA buttons |
| **Social Proof Bar** | Animated count-up stats: members, retention, coaches, rating |
| **About / USP** | Two-column layout with feature cards and member quote |
| **Programs** | 3-card grid: Strength, Fat Loss (highlighted), Functional Fitness |
| **Pricing** | 3 tiers with monthly/annual toggle (20% discount), Most Popular badge |
| **Testimonials** | Horizontal scroll carousel with dot navigation |
| **FAQ** | Sticky intro + animated accordion |
| **Footer** | Final email capture CTA + links + social |

---

## 🎨 Design System

### Colors
```css
--black:       #0A0A0A   /* Page background */
--charcoal:    #141414   /* Cards */
--iron:        #1E1E1E   /* Secondary surfaces */
--accent:      #E8FF00   /* Electric yellow-green — primary CTA */
--accent-hot:  #FF3C00   /* Hot orange — urgency, badges */
--white:       #F5F5F0   /* Body text */
--gray:        #7A7A72   /* Secondary text */
```

### Fonts (Google Fonts)
| Role | Font | Usage |
|---|---|---|
| Display / Headlines | `Bebas Neue` | H1, H2, logo, stats |
| Body / UI | `DM Sans` | Body copy, buttons, cards |
| Labels / Mono | `Space Mono` | Labels, badges, micro-copy |

---

## ⚡ JavaScript Behaviors

1. **Sticky Nav** — adds `.scrolled` class (blur + bg) after 80px scroll
2. **Mobile Menu** — full-screen overlay, closes on link click
3. **Smooth Scroll** — all anchor links scroll with 80px header offset
4. **Scroll Reveal** — `IntersectionObserver` fades sections up on entry
5. **Stat Counter** — animated count-up triggered when social proof bar enters viewport
6. **Pricing Toggle** — monthly/annual switch with fade transition on price numbers
7. **FAQ Accordion** — single-open, `max-height` animation, icon rotates 45°
8. **Testimonial Dots** — click to scroll + auto-update active dot on scroll
9. **Form Submit** — swaps form for success message on submit (no backend needed)

---

## 💰 Pricing Tiers

| Plan | Monthly | Annual |
|---|---|---|
| Basic | $39/mo | $31/mo |
| **IRONFORGE PRO** ⭐ | $69/mo | $55/mo |
| Elite | $119/mo | $95/mo |

---

## 📱 Responsive Breakpoints

| Breakpoint | Changes |
|---|---|
| `> 1024px` | Full layout, hex shape visible, 3-column grids |
| `≤ 1024px` | Tighter gaps, reduced pricing card padding |
| `≤ 768px` | Single column, hidden hex shape, hamburger nav, stacked form |

---

## 🔧 Customization

### Change gym name/location
Search and replace `IRONFORGE` and `CABUDARE, VENEZUELA` throughout the file.

### Update prices
Find `data-monthly` and `data-annual` attributes on `.price-amount` elements:
```html
<span class="price-amount" data-monthly="69" data-annual="55">69</span>
```

### Update stats
Find `data-target` attributes on `.stat-number` elements:
```html
<div class="stat-number" data-target="1400">0</div>
```

### Connect form to a real backend
Replace the mock submit handler in the `<script>` block:
```javascript
leadForm.addEventListener('submit', (e) => {
  e.preventDefault();
  // Replace with your fetch() call to Mailchimp, ConvertKit, etc.
});
```

---

## 🗂️ File Structure

```
ironforge-gym.html     ← Everything. One file.
README.md              ← This file
```

---

## 🛠️ Built With

- **HTML5** — semantic structure
- **CSS3** — custom properties, Grid, Flexbox, clip-path, animations
- **Vanilla JS** — IntersectionObserver, requestAnimationFrame, DOM manipulation
- **Google Fonts** — Bebas Neue, DM Sans, Space Mono

---

## ✅ Conversion Features

- CTA appears **5+ times** across the page
- "Free trial" framing removes financial friction
- Social proof numbers visible within first scroll
- "Most Popular" badge on mid-tier to anchor decisions
- Trust signals (no contract, cancel anytime, money-back) near every CTA
- Annual billing toggle increases perceived value
- Mobile-first — all buttons minimum 48px tap height

---

*IRONFORGE GYM · Where Limits Break · © 2025*
