# 900+ Free Animated Icons (Interactive & Open Source)

<p align="center">
  <a href="https://fridayowl.github.io/exode-animated-icons/"><img src="https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-ff5a36.svg?style=for-the-badge&logo=github" alt="Live Demo" /></a>
  <a href="https://github.com/fridayowl/exode-animated-icons/stargazers"><img src="https://img.shields.io/github/stars/fridayowl/exode-animated-icons?style=for-the-badge&logo=star&color=f59e0b" alt="GitHub Stars" /></a>
  <a href="https://github.com/fridayowl/exode-animated-icons/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT%20%2F%20ISC-10b981.svg?style=for-the-badge" alt="License" /></a>
  <img src="https://img.shields.io/badge/Icons-900%2B%20Free-6366f1.svg?style=for-the-badge" alt="900+ Icons" />
  <img src="https://img.shields.io/badge/Commercial%20Use-100%25%20Free-0ea5e9.svg?style=for-the-badge" alt="Free for Commercial Use" />
</p>

<p align="center">
  <strong>A comprehensive library of 900+ free, open-source animated interactive icons for modern web and mobile apps.</strong><br>
  Built with real-time spring physics, micro-interactions on hover & click, and one-click export for <strong>React, Vue 3, Svelte, Flutter, SwiftUI, and SVG</strong>.
</p>

<p align="center">
  <a href="https://fridayowl.github.io/exode-animated-icons/"><strong>Explore 900+ Icons Live Customizer &rarr;</strong></a> |
  <a href="https://www.exodeui.com"><strong>ExodeUI Home</strong></a> |
  <a href="https://app.exodeui.com"><strong>Open Exode Studio</strong></a>
</p>

---

## ⭐ If you find this project useful, please give it a star on GitHub! It helps more developers discover free open-source animations.

---

## 🌟 Why Exode Animated Icons?

| Feature | Static SVGs / Lucide | Heavy Lottie JSONs | **Exode Animated Icons** |
| :--- | :--- | :--- | :--- |
| **Animation** | ❌ None (Static) | ⚠️ Pre-baked keyframes | ✅ **Real-time spring physics & momentum** |
| **Interactivity** | ❌ None | ⚠️ Clunky JS listeners | ✅ **Native Hover, Click, & Loop triggers** |
| **File Size** | ~1 KB | ~30 KB - 100 KB+ | ✅ **Compact binary (`.bexode`) & JSON** |
| **Customization** | Color / Stroke only | Difficult to modify | ✅ **Live size, stroke, color, speed mixer** |
| **Frameworks** | React / Vue / Svelte | Lottie web player | ✅ **React, Vue 3, Svelte, Flutter, SwiftUI, SVG** |
| **Licensing** | Open Source | Mixed / Paid | ✅ **100% Free & Open Source for Commercial Use** |

---

## ✨ Features

- **900+ Free Interactive Icons**: Complete coverage across UI, arrows, media, navigation, commerce, social, editor, weather, and system controls.
- **Physics-Based Spring Dynamics**: Natural bounce, squash, stretch, and momentum curves computed on the fly.
- **Micro-Interaction Triggers**: Switch seamlessly between `hover`, `click` (press bounce), and `continuous loop`.
- **Live In-Browser Customizer**:
  - Live adjustment of stroke width (1px - 3px), icon size (16px - 128px), and playback speed.
  - Interactive color picker with real-time canvas rendering.
  - Multi-trigger tester (hover, active press, idle state).
- **Multi-Framework Export**:
  - Copy ready-to-paste components for **React**, **Vue 3**, **Svelte**, **Flutter**, **SwiftUI**, and vanilla **HTML / SVG**.
  - Download `.bexode` binary or `.exode` JSON files for editing in [ExodeUI Studio](https://app.exodeui.com).
- **One-Command CLI**: Quick-scaffold icons directly into React or Next.js apps with `npx exode add icon <name>`.

---

## 🚀 Quick Start

### Option 1: Install via Exode CLI

Add any animated icon to your React or Next.js project with a single command:

```bash
npx exode add icon heart
# or
npx exode add icon bell
# or
npx exode add icon check
```

### Option 2: React / Next.js Component

```tsx
import React, { useState } from 'react';
import { ExodeUICanvas } from 'exodeui';

export function InteractiveHeartIcon({ size = 28, color = '#ff5a36' }) {
  const [active, setActive] = useState(false);

  return (
    <button
      onMouseEnter={() => setActive(true)}
      onMouseLeave={() => setActive(false)}
      onClick={() => setActive(!active)}
      style={{
        width: size,
        height: size,
        background: 'transparent',
        border: 'none',
        cursor: 'pointer',
        padding: 0,
      }}
      aria-label="Favorite"
    >
      <ExodeUICanvas
        src="https://raw.githubusercontent.com/fridayowl/exode-animated-icons/main/files/heart.bexode"
        active={active}
        color={color}
        style={{ width: '100%', height: '100%' }}
      />
    </button>
  );
}
```

### Option 3: Vue 3 / Nuxt

```vue
<template>
  <div 
    @mouseenter="active = true" 
    @mouseleave="active = false"
    :style="{ width: `${size}px`, height: `${size}px` }"
  >
    <ExodeUICanvas
      src="/icons/heart.bexode"
      :active="active"
    />
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { ExodeUICanvas } from 'exodeui-vue';

defineProps({
  size: { type: Number, default: 28 }
});
const active = ref(false);
</script>
```

---

## 🎨 Online Interactive Gallery & Customizer

Visit the live gallery at **[https://fridayowl.github.io/exode-animated-icons/](https://fridayowl.github.io/exode-animated-icons/)** to:
1. **Search & Filter**: Search 900+ icons instantly with real-time keyword matching and category filters.
2. **Tune Parameters**: Adjust stroke width, icon scale, animation speed, and color in real time.
3. **Test Micro-Interactions**: Hover, click, and inspect micro-interactions with immediate visual feedback.
4. **Copy Code**: One-click copy for React, Vue, Svelte, Flutter, SwiftUI, and SVG.

---

## 🏷️ Keywords & Topics

`animated-icons` • `interactive-icons` • `free-icons` • `open-source` • `react-icons` • `svg-icons` • `lucide-animated` • `lottie-alternative` • `motion-ui` • `micro-interactions` • `spring-physics` • `ui-components` • `vector-animation` • `vue-icons` • `svelte-icons` • `web-components` • `exodeui`

---

## 📄 Open Source License

- Icon base vectors derived from the open-source [Lucide](https://github.com/lucide-icons/lucide) project under the [ISC License](https://opensource.org/licenses/ISC).
- Interactive physics definitions and animations powered by [ExodeUI](https://www.exodeui.com).
- **100% Free for both Personal and Commercial Use.** No attribution required, though a ⭐ star on GitHub is always appreciated!

---

<p align="center">
  Crafted with care by the <a href="https://www.exodeui.com">ExodeUI</a> team &bull; <a href="https://github.com/fridayowl/exode-animated-icons">GitHub Repository</a>
</p>
