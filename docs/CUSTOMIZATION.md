# Customization Guide — Portfolio V5

This guide explains how to adapt this portfolio to your own brand and content.  
All changes are made in a single file: `moe-kyaw-aung-portfolio-v5.html`

---

## Table of Contents

- [Profile Photo](#1-profile-photo)
- [Personal Info](#2-personal-info)
- [Color Theme](#3-color-theme)
- [Hero Content](#4-hero-content)
- [Skills](#5-skills)
- [Projects](#6-projects)
- [Certificates](#7-certificates)
- [Social Links](#8-social-links)
- [Contact Details](#9-contact-details)
- [Pricing](#10-pricing)
- [Google Map](#11-google-map)
- [Testimonials](#12-testimonials)
- [Footer](#13-footer)

---

## 1. Profile Photo

Find and replace the Gravatar URL (appears ~6 times in the file):

```html
<!-- Current (Moe Kyaw Aung's Gravatar) -->
https://0.gravatar.com/avatar/a2dae9a29fbf7c72552047efc744be54a018938aacd9009e7500f93d72eb0f2e?size=400

<!-- Replace with your own Gravatar URL -->
<!-- How to get yours:
     1. Create a Gravatar account at gravatar.com
     2. MD5 hash your email: https://www.md5hashgenerator.com/
     3. URL = https://0.gravatar.com/avatar/YOUR_MD5_HASH?size=400
-->
```

Or use any direct image URL:
```html
<img src="https://your-domain.com/your-photo.jpg" alt="Your Name">
```

---

## 2. Personal Info

### Name & Role
```html
<!-- Sidebar logo -->
<div class="sb-logo">YNA<span>.</span>DEV</div>
<div class="sb-name">YOUR NAME HERE</div>
<div class="sb-role">Your Role</div>

<!-- Hero subtitle -->
<p class="hero-sub">Your Name — Full Stack Developer</p>

<!-- About heading -->
<h3>Senior Android Developer & Full Stack Engineer</h3>
```

### Bio
```html
<!-- About section, two paragraphs -->
<p>Your bio paragraph 1...</p>
<p>Your bio paragraph 2...</p>
```

### Info Grid
```html
<div class="info-row"><i class="fas fa-map-marker-alt"></i> Your City, Country</div>
<div class="info-row"><i class="fas fa-envelope"></i> your@email.com</div>
<div class="info-row"><i class="fas fa-phone"></i> +1 234 567 890</div>
```

---

## 3. Color Theme

Edit the `:root` CSS custom properties (top of `<style>` block):

```css
:root {
  /* === CHANGE THESE === */
  --primary:   #9b8ec4;   /* Main brand color (lavender) */
  --secondary: #7c6daa;   /* Darker brand color */
  --accent:    #c084fc;   /* Highlight / label color */
  --accent2:   #818cf8;   /* Second highlight */
  --bg:        #F5F3FF;   /* Light background */
  --bg-alt:    #ede9fe;   /* Alternate section background */
}

[data-theme="dark"] {
  /* === CHANGE THESE FOR DARK MODE === */
  --primary:   #b5a8d9;
  --secondary: #9b8ec4;
  --accent:    #d8b4fe;
  --bg:        #0d0a1c;
  --bg-alt:    #140f28;
}
```

**Tip:** Use [coolors.co](https://coolors.co) to generate matching palettes.

---

## 4. Hero Content

```html
<!-- Tech chips below the subtitle -->
<div class="hero-chips">
  <span class="chip"><i class="fab fa-android"></i> Kotlin</span>
  <span class="chip">Your Tech Stack</span>
  <!-- Add / remove chips as needed -->
</div>

<!-- Hero description paragraph -->
<p class="hero-desc">
  Your compelling bio paragraph here. Mention your experience,
  specializations, and what makes you unique.
</p>
```

---

## 5. Skills

Find the `.skills-grid` section and edit each skill card:

```html
<div class="skill-card gc fi d1">
  <div class="sk-icon"><i class="fab fa-android"></i></div>
  <div class="sk-name">Skill Name</div>
  <div class="sk-track">
    <div class="sk-fill" data-pct="95"></div>  <!-- 0–100 -->
  </div>
  <div class="sk-pct">95%</div>
</div>
```

**Icon classes:** Use any Font Awesome icon class.  
`fab fa-android` · `fas fa-fire` · `fab fa-react` · `fas fa-database` · etc.

---

## 6. Projects

Each project card in `.proj-g`:

```html
<div class="proj-c gc fi d1">
  <div class="proj-tag-top"><i class="fas fa-star"></i> Featured</div>
  <div class="proj-title">Your Project Name</div>
  <div class="proj-desc">Project description goes here. 2–3 sentences.</div>
  <div class="proj-chips">
    <span class="p-chip">Kotlin</span>
    <span class="p-chip">Firebase</span>
  </div>
  <div class="proj-links">
    <a href="https://github.com/your-repo" class="p-link">
      <i class="fab fa-github"></i> GitHub
    </a>
    <a href="https://demo-url.com" class="p-link">
      <i class="fas fa-external-link-alt"></i> Demo
    </a>
  </div>
</div>
```

---

## 7. Certificates

Edit the `CERTS` JavaScript array:

```javascript
const CERTS = [
  {
    nm:  'Certificate Name',     // Display name
    cat: 'mobile',               // Category: mobile | web | security | cloud | other
    url: 'https://your-cert.jpg' // Direct image URL to certificate
  },
  // ... add all your certificates
];
```

**Getting Programming Hub certificate URLs:**
1. Log in at programminghub.io
2. Open your certificate
3. Right-click → "Copy image address"

---

## 8. Social Links

Find the `.soc-g` grid in the social section and edit each link:

```html
<a href="https://github.com/YOUR-USERNAME" target="_blank" rel="noopener" class="soc-c fi d1">
  <div class="soc-ico" style="background:#24292e">
    <i class="fab fa-github"></i>
  </div>
  <div>
    <div class="soc-pl">GitHub</div>
    <div class="soc-hl">@YOUR-USERNAME</div>
  </div>
</a>
```

Remove any platforms you don't use. Add new ones by copying the pattern.

---

## 9. Contact Details

```html
<!-- Contact info cards -->
<div class="ci-val">your@email.com</div>
<div class="ci-val">+1 234 567 890</div>
<div class="ci-val">Your City, Country (GMT+XX:00)</div>
```

---

## 10. Pricing

Edit the three price cards in the `.price-g` grid.  
Change amounts, feature lists, and button links as needed.

```html
<div class="price-amt"><sup>$</sup>800</div>  <!-- Change price -->
<div class="price-per">/ project</div>         <!-- Change period -->
```

---

## 11. Google Map

Replace the `src` URL in the map iframe:

```html
<!-- Get your embed URL from:
     maps.google.com → Search your location →
     Share → Embed a map → Copy HTML → extract src="..." -->

<iframe
  src="YOUR_GOOGLE_MAPS_EMBED_URL"
  ...></iframe>
```

---

## 12. Testimonials

Each slide in `.slider-track`:

```html
<div class="slide">
  <div class="testi-c">
    <div class="stars">★★★★★</div>
    <p class="testi-q">"Your testimonial text here..."</p>
    <div class="testi-auth">
      <img src="https://picsum.photos/seed/client1/48/48" alt="Client Name">
      <div>
        <div class="auth-nm">Client Name</div>
        <div class="auth-role">Role, Company</div>
      </div>
    </div>
  </div>
</div>
```

Add or remove `.slide` divs. The JS auto-detects the count.

---

## 13. Footer

```html
<!-- Brand name -->
<div class="ft-brand-name">YOUR<span>.</span>DEV</div>

<!-- Tagline -->
<p class="ft-desc">Your footer description...</p>

<!-- Copyright -->
<div class="ft-copy">© 2026 Your Name. Made with ❤️ from Your City.</div>

<!-- Version -->
<div class="ft-ver">PORTFOLIO V5.0.0</div>
```

---

## 💡 Pro Tips

1. **Keep all colors as CSS variables** — never hardcode `#hex` in the HTML body
2. **Use Font Awesome icons** — browse at [fontawesome.com/icons](https://fontawesome.com/icons)
3. **Test dark mode** — every color change must work in both light and dark
4. **Validate HTML** — use [validator.w3.org](https://validator.w3.org/) before deploying
5. **Check mobile** — open DevTools → Toggle device toolbar → 375px width minimum

---

*Questions? Open an issue or contact: moekyawaung@fastmail.com*
