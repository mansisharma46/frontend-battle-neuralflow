# NeuralFlow — Data Automation Platform

**Frontend Battle 3.0 Official Submission — IIT Bhubaneswar**

---

## Project Overview

NeuralFlow is a responsive, high-performance SaaS landing page developed exclusively for Frontend Battle 3.0. The architecture and user interface were engineered with strict adherence to the competition's technical constraints and scoring rubrics, specifically optimizing for Architecture, UI/UX Usability, and Motion Matching criteria.

## Rule Compliance & Constraints

This submission guarantees strict adherence to all mandated project rules:

- **Zero-Build Architecture**: The entire application is delivered as a single `index.html` file to ensure maximum portability.
- **Native Implementation**: Developed exclusively using Vanilla HTML5, CSS3, and JavaScript (ES2020+). No external frameworks (e.g., React, TailwindCSS) or animation libraries (e.g., GSAP, Framer Motion) were utilized.
- **Performance Budget**: All UI/UX animations and interactivity execute strictly within the required 500ms entry budget.
- **Local Portability**: Designed to render instantly via the `file://` protocol without CORS errors or the need for a local development server.
- **Design System Fidelity**: Implements the exact typography (JetBrains Mono, Inter) and hexadecimal color palette provided in the competition assets.

## Architecture Highlights

- **DOM-Isolated State Management**: The pricing matrix logic dynamically computes values based on multi-dimensional configurations (currency tariffs, billing cycles). State updates are strictly isolated to target text nodes, ensuring zero parent component reflows for maximum performance.
- **Responsive Context Transfer**: The desktop Bento Grid seamlessly transitions into a mobile accordion pattern, gracefully retaining the active panel's state context across viewport resizes.
- **Embedded Asset Mapping**: To ensure zero-configuration local execution, all required SVGs are embedded synchronously via a JavaScript object map (`SVG_MAP`), bypassing local network fetch limitations.

## UI/UX & Motion Innovations

To maximize scoring in the UI/UX Usability and Motion Matching categories, the following native innovations were implemented from scratch:

1. **Typewriter Effect**: A recursive algorithm driving an infinitely looping hero headline.
2. **Particle Canvas Background**: A lightweight, 60 FPS HTML5 `<canvas>` rendering engine for dynamic background motion using `requestAnimationFrame`.
3. **Cursor-Aware Spotlight**: Dynamic CSS `radial-gradient` mouse tracking across the feature grid.
4. **3D Tilt Transformations**: Real-time perspective transformations (`rotateX`, `rotateY`) on pricing cards reacting to mouse coordinates.
5. **Infinite Marquee**: A continuous, CSS-driven scrolling trust bar.
6. **Scroll-Triggered Reveals**: `IntersectionObserver`-based fade and transform animations for sections entering the viewport.
7. **Scroll Tracking**: A fixed gradient progress bar mapping to document scroll depth.
8. **Active Navigation Context**: Dynamic navigation highlighting based on viewport intersection state.

## Setup Instructions

The project requires no dependency installation or server configuration.

1. Extract the project repository.
2. Locate the `index.html` file in the root directory.
3. Open `index.html` directly in any modern web browser (Chrome, Firefox, Safari, Edge).
