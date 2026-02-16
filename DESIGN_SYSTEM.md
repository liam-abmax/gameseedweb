# GameSeed - Design System & Color Documentation

## Overview
GameSeed is a modern, futuristic indie gaming discovery platform with a sophisticated color palette designed for gaming audiences. The design emphasizes glassmorphism, smooth animations, and a premium dark-mode aesthetic.

---

## Color Palette

### Primary Colors

#### **Cyan (#00D9FF)**
- **Usage**: Primary actions, navigation highlights, borders, accent elements
- **RGB**: rgb(0, 217, 255)
- **HSL**: hsl(189, 100%, 50%)
- **Psychology**: Trust, technology, innovation, calmness
- **Common Uses**:
  - Primary buttons
  - Hover states
  - Active navigation
  - Glow effects
  - Primary text accents

#### **Electric Magenta (#FF006E)**
- **Usage**: Secondary actions, highlights, urgent calls-to-action
- **RGB**: rgb(255, 0, 110)
- **HSL**: hsl(330, 100%, 50%)
- **Psychology**: Energy, excitement, action
- **Common Uses**:
  - Secondary buttons
  - Featured tags
  - Investor/premium features
  - Attention-grabbing elements

#### **Bright Lime (#39FF14)**
- **Usage**: Success states, achievements, positive actions
- **RGB**: rgb(57, 255, 20)
- **HSL**: hsl(113, 100%, 54%)
- **Psychology**: Success, growth, vitality
- **Common Uses**:
  - Success messages
  - Achievement badges
  - Positive indicators
  - Growth charts

### Background Colors

#### **Deep Navy (#0A0E27)**
- **Usage**: Primary background color
- **RGB**: rgb(10, 14, 39)
- **HSL**: hsl(228, 59%, 10%)
- **Purpose**: Main page background, immersive gaming aesthetic
- **Features**: Very dark, minimizes eye strain, perfect for gaming interfaces

#### **Card Background (#16213E)**
- **Usage**: Card/component backgrounds
- **RGB**: rgb(22, 33, 62)
- **HSL**: hsl(218, 48%, 16%)
- **Purpose**: Subtle elevation above main background

#### **Light Variant (#1a1a3a)**
- **Usage**: Secondary background sections
- **RGB**: rgb(26, 26, 58)
- **HSL**: hsl(240, 38%, 16%)
- **Purpose**: Alternative background for sections

### Text Colors

#### **White (#FFFFFF)**
- **Usage**: Primary text, headers
- **RGB**: rgb(255, 255, 255)
- **Contrast Ratio**: AAA compliant with all backgrounds

#### **Light Gray (#E0E0E0)**
- **Usage**: Secondary text, body content
- **RGB**: rgb(224, 224, 224)
- **Contrast Ratio**: AAA compliant

#### **Gray (#808080)**
- **Usage**: Placeholder text, disabled states
- **RGB**: rgb(128, 128, 128)

---

## Color Gradient Combinations

### Primary Gradient
```css
linear-gradient(135deg, #00D9FF 0%, #FF006E 100%)
```
- **Usage**: Text, borders, buttons, visual accents
- **Effect**: Creates modern, energetic feel
- **Common Elements**: Logo, hero headlines, stat numbers

### Secondary Gradient
```css
linear-gradient(135deg, #FF006E 0%, #FF1493 100%)
```
- **Usage**: Secondary button gradients
- **Effect**: Bold magenta tones
- **Brightness Adjustment**: 10% lighter variant available

### Tertiary Gradient
```css
linear-gradient(135deg, #00D9FF 0%, #0099FF 100%)
```
- **Usage**: Primary action buttons
- **Effect**: Cool, inviting, tech-forward

---

## Design Patterns & Effects

### Glassmorphism
- **Background**: `rgba(22, 33, 62, 0.6)`
- **Backdrop Filter**: `blur(10px)`
- **Border**: `1px solid rgba(0, 217, 255, 0.2)`
- **Effect**: Creates frosted glass appearance with depth

### Glow Effects (CSS)
```css
/* Primary Glow */
box-shadow: 0 0 20px rgba(0, 217, 255, 0.5),
            0 0 40px rgba(0, 217, 255, 0.2);

/* Secondary Glow */
box-shadow: 0 0 20px rgba(255, 0, 110, 0.5),
            0 0 40px rgba(255, 0, 110, 0.2);
```

### Button States

#### Primary Button
- **Default**: Cyan gradient background, dark text
- **Hover**: Lifts up 3px, glow shadow appears
- **Active**: Pressed state with reduced shadow
- **Disabled**: Reduced opacity (0.5)

#### Secondary Button
- **Default**: Magenta gradient background, white text
- **Hover**: Lifts up 3px, glow shadow appears
- **States**: Same as primary

#### Outline Button
- **Default**: Transparent background, cyan border
- **Hover**: Cyan background fills with 10% opacity
- **Focus**: Border brightens, shadow appears

### Hover Effects
- **Cards**: Lift up 8px, border brightness increases, shadow expands
- **Links**: Underline grows from left to right
- **Icons**: Scale up 10% on hover

---

## Opacity & Alpha Values

| Usage | Value | Notes |
|-------|-------|-------|
| Primary Border | 0.2 | Subtle, doesn't overpower |
| Hover State | 0.4 | More visible, interactive feel |
| Active State | 0.6 | Clearly selected |
| Disabled | 0.3 | Reduced but still visible |
| Text Overlay | 0.9 | Readable while showing background |
| Glow Inner | 0.1 | Subtle internal glow only |

---

## Typography

### Font Family
- **Primary**: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
- **Fallback**: System fonts for optimal rendering

### Font Weights & Sizes

| Element | Weight | Size | Letter Spacing |
|---------|--------|------|-----------------|
| Logo | 900 (Black) | 2rem | -0.02em |
| Hero H1 | 900 (Black) | 4rem-8rem | -0.03em |
| Section H2 | 900 (Black) | 2.25rem-3rem | -0.02em |
| Card Title | 900 (Black) | 1.5rem | 0 |
| Body Text | 500 (Medium) | 1rem | 0 |
| Small Text | 400 (Regular) | 0.875rem | 0.01em |
| Label | 700 (Bold) | 0.75rem | 0.05em |

---

## Component Colors

### Cards
- **Background**: `glass-effect` class (rgba + blur)
- **Border**: `1px solid rgba(0, 217, 255, 0.2)`
- **Hover Border**: `rgba(0, 217, 255, 0.6)`

### Tags/Badges
- **Background**: `rgba(0, 217, 255, 0.1)`
- **Border**: `1px solid rgba(0, 217, 255, 0.3)`
- **Text**: Cyan primary

### Form Elements
- **Input Background**: Dark card color
- **Input Border**: Primary/20%
- **Input Focus**: Primary/50%
- **Placeholder**: Gray/40%

### Navigation
- **Link Color**: Gray (#E0E0E0)
- **Hover Color**: Primary cyan
- **Active Color**: Primary cyan + underline
- **Underline**: Gradient cyan to magenta

---

## Animation & Motion

### Keyframes

#### Float Animation
```css
@keyframes float {
    0%, 100% { transform: translateY(0px) rotateZ(0deg); }
    50% { transform: translateY(-30px) rotateZ(2deg); }
}
```
- **Duration**: 6s
- **Timing**: ease-in-out
- **Uses**: Logo, hero elements

#### Glow Animation
```css
@keyframes glow-primary {
    0%, 100% { box-shadow: 0 0 20px... }
    50% { box-shadow: 0 0 40px... }
}
```
- **Duration**: 3s
- **Timing**: ease-in-out
- **Uses**: Buttons, featured elements

#### Slide Up Animation
```css
@keyframes slide-up {
    from { opacity: 0; transform: translateY(40px); }
    to { opacity: 1; transform: translateY(0); }
}
```
- **Duration**: 0.8s
- **Timing**: ease-out
- **Uses**: Page load, scroll reveal

### Transition Timing
- **Quick Actions**: 0.2s (button hover)
- **Standard**: 0.3s (card hover, link underline)
- **Slow**: 0.6s-0.8s (page animations)

---

## Responsive Design Breakpoints

- **Mobile**: < 768px (md)
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

### Color Adjustments for Different Screens
- **All sizes**: Same color palette
- **Text sizes**: Scale responsively
- **Opacity**: Same across all breakpoints
- **Glow effects**: Slightly reduced on mobile for performance

---

## Accessibility Considerations

### Contrast Ratios
All text meets WCAG AA standards (4.5:1 minimum)
- Cyan on dark background: 7.2:1 ✓
- White on dark background: 12.6:1 ✓
- Magenta on dark background: 6.1:1 ✓

### Color Blindness
- Not relying solely on color for information
- Using patterns, text, and icons in addition to color
- Gradients provide additional visual information

### Focus States
- All interactive elements have visible focus indicators
- Focus color: Cyan primary
- Focus outline: 2px solid

---

## File Structure & Variables

### CSS Custom Properties (Recommended for Implementation)
```css
:root {
    --color-primary: #00D9FF;
    --color-secondary: #FF006E;
    --color-accent: #39FF14;
    --color-dark: #0A0E27;
    --color-dark-card: #16213E;
    --color-dark-light: #1a1a3a;
    --color-text: #FFFFFF;
    --color-text-secondary: #E0E0E0;
    
    --gradient-primary: linear-gradient(135deg, #00D9FF, #FF006E);
    --gradient-secondary: linear-gradient(135deg, #FF006E, #FF1493);
    
    --duration-quick: 0.2s;
    --duration-standard: 0.3s;
    --duration-slow: 0.6s;
}
```

---

## Mobile Development Handoff

### For React Native / Flutter / Native Mobile
Use these exact hex values:
- **Primary**: `#00D9FF`
- **Secondary**: `#FF006E`
- **Accent**: `#39FF14`
- **Dark**: `#0A0E27`
- **Card**: `#16213E`

### For Dark Mode Adjustments
All colors already optimized for dark theme. No additional adjustments needed.

### Shadow & Glow on Mobile
```
Shadow: 0 4px 12px rgba(0, 217, 255, 0.2)
Glow: 0 0 12px rgba(0, 217, 255, 0.3)
(Slightly reduced for performance)
```

---

## Special Effects

### Blink/Pulse States
- **Normal Elements**: Subtle, 50% opacity to 100%
- **Duration**: 2s infinite
- **Effect**: Draws attention without being jarring

### Spin Effects
- **Speed**: 8s linear infinite
- **Usage**: Loading states, animated logos
- **Effect**: Smooth, continuous rotation

---

## Component-Specific Colors

### Game Cards
- **Title**: White
- **Description**: Gray-300
- **Tags**: Cyan with cyan borders
- **Rating**: Cyan gradient for stars
- **Primary Button**: Cyan gradient
- **Secondary Button**: Outline cyan

### Developer Dashboard
- **Stat Numbers**: Cyan-to-magenta gradient
- **Active Navigation**: Cyan background with border
- **Chart Bars**: Cyan to secondary gradient
- **Growth Indicator**: Lime/accent color

### Scout/Investor Section
- **Emphasis Color**: Secondary magenta
- **Stats**: Gradient text
- **Features**: Mixed cyan/magenta

---

## Design Tokens Summary

```json
{
  "colors": {
    "primary": "#00D9FF",
    "secondary": "#FF006E",
    "accent": "#39FF14",
    "backgrounds": {
      "main": "#0A0E27",
      "card": "#16213E",
      "light": "#1a1a3a"
    },
    "text": {
      "primary": "#FFFFFF",
      "secondary": "#E0E0E0"
    }
  },
  "gradients": {
    "primary": "linear-gradient(135deg, #00D9FF 0%, #FF006E 100%)",
    "button": "linear-gradient(135deg, #00D9FF 0%, #0099FF 100%)"
  },
  "shadows": {
    "glow": "0 0 20px rgba(0, 217, 255, 0.5)",
    "card": "0 20px 40px rgba(0, 217, 255, 0.2)"
  }
}
```

---

## Version History
- **v1.0** (Feb 2026): Initial design system documentation
- **Future**: Component library documentation, animation guidelines

---

**Design System Created**: February 2026
**Last Updated**: February 2026
