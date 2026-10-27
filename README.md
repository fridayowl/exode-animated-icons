# ExodeUI Animated Icons

> **900+ free, interactive animated icons** powered by [ExodeUI](https://www.exodeui.com). Based on the open-source [Lucide](https://lucide.dev) icon set, enhanced with spring physics, hover, and press states.

🌐 **Live Demo & Interactive Customizer:**  
👉 **[https://fridayowl.github.io/exode-animated-icons/](https://fridayowl.github.io/exode-animated-icons/)**

---

## ✨ Features

- **900+ Icons**: Interface, media, navigation, weather, commerce, social, and system icons.
- **Physics-Based Spring Motion**: Natural bounce, squash, stretch, and ease curves computed in real time.
- **Multiple Triggers**: Preview and export with `hover`, `click`, or continuous `loop` triggers.
- **Interactive In-Browser Customizer**:
  - Stroke width, icon size, animation speed, and trigger adjustments.
  - Custom color selection with live preview on Canvas.
- **Multi-Framework Export**:
  - Copy ready-to-use components for **React**, **Vue 3**, **Svelte**, **Flutter**, **SwiftUI**, and vanilla **HTML/SVG**.
  - Download binary `.bexode` or JSON `.exode` files for instant import into the ExodeUI editor.
- **One-Command CLI Installation**: Install directly into your React / Next.js project with `npx exode add icon <name>`.

---

## 🚀 Quick Start

### 1. Install via Exode CLI

To add an icon directly to your React or Next.js project:

```bash
npx exode add icon heart
# or
npx exode add icon search
```

### 2. React / Next.js Usage

```tsx
import React, { useState } from 'react';
import { ExodeUICanvas } from 'exodeui';

export function HeartIcon({ size = 24, color = 'currentColor' }) {
  const [trigger, setTrigger] = useState(false);

  return (
    <div 
      onMouseEnter={() => setTrigger(true)} 
      onMouseLeave={() => setTrigger(false)}
      style={{ width: size, height: size }}
    >
      <ExodeUICanvas
        src="files/heart.bexode"
        active={trigger}
        style={{ width: '100%', height: '100%' }}
      />
    </div>
  );
}
```

---

## 🎨 Interactive Gallery

Visit the GitHub Pages deployment at **[https://fridayowl.github.io/exode-animated-icons/](https://fridayowl.github.io/exode-animated-icons/)** to:
1. Search all 900+ icons by name or category.
2. Adjust size, stroke width, and animation playback speed.
3. Test hover and click micro-interactions.
4. Copy generated framework code with a single click.

---

## 📁 Repository Structure

```text
.
├── index.html       # Standalone interactive gallery & customizer web app
├── files/           # Compiled .bexode binary and .exode JSON animation assets
├── .nojekyll        # Disables Jekyll processing for GitHub Pages
└── README.md        # Documentation and quick start guide
```

---

## 📄 License

- Icons are based on the [Lucide](https://github.com/lucide-icons/lucide) project, licensed under the [ISC License](https://opensource.org/licenses/ISC).
- Interactive animations and runtime definitions are provided by [ExodeUI](https://www.exodeui.com).
