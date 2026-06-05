# 👋 Waving Hand CSS Animation

A tiny, pure-CSS waving hand emoji animation. No JavaScript, no dependencies — just copy two CSS rules and you're done.

---

## ✨ Live Demo

<p align="center">
  <a href="https://emre-the-enthusiastic-coder.github.io/waving-hand-animation/">
    <img src="https://img.shields.io/badge/▶%20View%20Live%20Demo-0d1117?style=for-the-badge&logo=github&logoColor=white" alt="Live Demo" />
  </a>
</p>

<p align="center">
  <a href="https://emre-the-enthusiastic-coder.github.io/waving-hand-animation/">
    <img src="https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen?style=flat-square&logo=github" alt="GitHub Pages" />
  </a>
  <a href="https://codepen.io/einargudnig/pen/YzNeZOG">
    <img src="https://img.shields.io/badge/Original-CodePen-black?style=flat-square&logo=codepen" alt="CodePen" />
  </a>
  <img src="https://img.shields.io/badge/CSS-Only-264de4?style=flat-square&logo=css3" alt="CSS Only" />
  <img src="https://img.shields.io/badge/No%20JS-required-success?style=flat-square" alt="No JS" />
</p>

---

## 👀 Preview

<p align="center">
  <iframe
    src="https://emre-the-enthusiastic-coder.github.io/waving-hand-animation/"
    width="700"
    height="400"
    style="border: 1px solid #30363d; border-radius: 12px;"
    title="Waving Hand CSS Animation Demo">
  </iframe>
</p>

> **Note:** GitHub's README renderer blocks iframes. [Click here to see the live demo](https://emre-the-enthusiastic-coder.github.io/waving-hand-animation/) 👆

---

## 🚀 Usage

**Step 1 — Add the CSS:**

```css
.waving-hand {
  animation-name: wave-animation;
  animation-duration: 2.5s;
  animation-iteration-count: infinite;
  transform-origin: 70% 70%;
  display: inline-block;
}

@keyframes wave-animation {
  0%   { transform: rotate(  0.0deg) }
  15%  { transform: rotate( 14.0deg) }  /* tweak these to change intensity */
  30%  { transform: rotate( -8.0deg) }
  40%  { transform: rotate( 14.0deg) }
  50%  { transform: rotate( -4.0deg) }
  60%  { transform: rotate( 10.0deg) }
  70%  { transform: rotate(  0.0deg) }  /* pause for the last 30% */
  100% { transform: rotate(  0.0deg) }
}
```

**Step 2 — Add the class to any emoji or element:**

```html
<!-- Standalone -->
<span class="waving-hand">👋</span>

<!-- Inline inside a heading -->
<h1>Hello there <span class="waving-hand">👋</span> welcome!</h1>

<!-- Works with other emojis too -->
<span class="waving-hand">🌟</span>
<span class="waving-hand">🎉</span>
```

That's it! ✅

---

## 🔧 How it works

| Property | Value | Why |
|---|---|---|
| `transform-origin: 70% 70%` | wrist pivot point | makes the rotation feel like a real wrist movement |
| `animation-iteration-count: infinite` | loops forever | keeps waving |
| `display: inline-block` | required | `transform` doesn't apply to pure `inline` elements |
| keyframes 70% → 100% | stays at 0° | creates a natural pause between waves |

---

## 🎨 Customisation

| What | How |
|---|---|
| **Speed** | Change `animation-duration` (e.g. `1.5s` faster, `4s` slower) |
| **Intensity** | Adjust the `deg` values in the keyframes |
| **One-time wave** | Change `infinite` to `1` |
| **Delayed start** | Add `animation-delay: 1s` |
| **Any element** | Works on any HTML element, not just emojis |

---

## 📁 Files

```
waving-hand-animation/
└── index.html   ← standalone demo page (open in any browser)
```

---

## 🙏 Credits

Original pen by **[@einargudnig](https://codepen.io/einargudnig/pen/YzNeZOG)** on CodePen.  
Saved and shared here to make it easy to find, copy, and use.

---

<sub>Pure CSS · No JS · No dependencies · Works in all modern browsers · MIT</sub>
