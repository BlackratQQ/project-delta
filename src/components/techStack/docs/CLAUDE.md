# Claude Code - TechStack Components Technical Documentation

## Architecture

```
/components/techStack/
├── TechStack.astro        # Main tech stack section
├── About.astro            # Technology information section
└── docs/
    ├── README.md
    └── CLAUDE.md          # This file
```

## Implementation

### TechStack.astro

- Container for technology showcase section
- Integration with LogoLoop React component from /react/techStack/
- Animated headings using BlurText
- Responsive layout system

### About.astro

- Detailed information about technology choices
- Philosophy and approach to technology selection
- Integration with broader site design system

## React Integration

### LogoLoop Component

Located in `/react/techStack/LogoLoop.tsx`:

```typescript
interface LogoLoopProps {
  logos: LogoItem[]; // Array of technology logos
  speed?: number; // Animation speed (120 px/s default)
  direction?: 'left' | 'right'; // Scroll direction
  pauseOnHover?: boolean; // Pause on mouse hover
  scaleOnHover?: boolean; // Scale effect on hover
}
```

**Features:**

- Infinite horizontal scrolling
- Smooth velocity transitions
- ResizeObserver for responsive behavior
- Copy management for seamless looping
- Performance optimizations (requestAnimationFrame)

### Technology Logos

Pre-configured logos include:

- OpenAI, Claude AI
- React, Next.js, Astro
- TypeScript, JavaScript
- Tailwind CSS, CSS3
- HTML5, PHP
- WordPress, Figma

## Technical Features

- **Infinite Scroll**: Seamless logo carousel using requestAnimationFrame
- **3D Background**: Threads component for visual depth
- **Performance**: Copy management, throttled animations
- **Responsive**: Mobile-first design with breakpoint optimization
- **Accessibility**: ARIA labels, keyboard navigation support

---

_Technical Documentation v1.0.0 - TechStack Components_
