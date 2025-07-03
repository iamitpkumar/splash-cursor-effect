# ✨ Splash Cursor Effect

<div align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white" alt="jQuery">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" alt="MIT License">
</div>

<div align="center">
  <h3>🌊 Create mesmerizing liquid splash effects that follow your cursor</h3>
  <p>A lightweight, customizable cursor effect that brings your website to life with beautiful gradient animations</p>
</div>

---

## 🎯 Features

- **🌈 Gradient Splash Effects** - Beautiful fluid gradients with cosmic colors
- **🎨 Multiple Splash Types** - Three different splash variations for dynamic visuals
- **⚡ Smooth Animations** - Optimized CSS keyframes with hardware acceleration
- **🖱️ Interactive Cursor** - Custom cursor with click feedback and smooth following
- **📱 Responsive Design** - Works seamlessly across all devices
- **🔧 Easy Integration** - Simple HTML, CSS, and jQuery implementation
- **🎭 Customizable** - Easy to modify colors, sizes, and animation timings

## 🚀 Demo

[**Live Demo**](https://iamitpkumar.github.io/splash-cursor-effect/) | [**CodePen**](https://codepen.io/your-username/pen/demo-link)

![Splash Cursor Effect Demo](demo.gif)

## 🛠️ Installation

### Option 1: Direct Download
```bash
git clone https://github.com/iamitpkumar/splash-cursor-effect.git
cd splash-cursor-effect
```

### Option 2: CDN Links
```html
<!-- Include jQuery -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>

<!-- Include the splash cursor CSS and JS -->
<link rel="stylesheet" href="path/to/splash-cursor.css">
<script src="path/to/splash-cursor.js"></script>
```

## 📋 Usage

### Basic Implementation

1. **HTML Structure**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Splash Cursor Effect</title>
    <link rel="stylesheet" href="splash-cursor.css">
</head>
<body>
    <div class="cursor"></div>
    
    <!-- Your content here -->
    <div class="container">
        <h1>Your Amazing Website</h1>
        <p>Move your cursor around!</p>
    </div>
    
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <script src="splash-cursor.js"></script>
</body>
</html>
```

2. **Initialize the Effect**
```javascript
$(document).ready(function() {
    // The effect initializes automatically!
    // Just include the script and CSS
});
```

### Custom Configuration

```javascript
// Customize splash frequency
const splashFrequency = 0.7; // 0.1 = rare, 0.9 = frequent

// Customize colors
const splashColors = {
    primary: '#3a86ff',
    secondary: '#8338ec', 
    accent: '#ff006e'
};

// Apply custom settings
initSplashCursor({
    frequency: splashFrequency,
    colors: splashColors,
    size: 'large' // 'small', 'medium', 'large'
});
```

## 🎨 Customization

### Color Themes

```css
/* Cosmic Theme (Default) */
--splash-primary: #3a86ff;
--splash-secondary: #8338ec;
--splash-accent: #ff006e;
--splash-dark: #120078;

/* Ocean Theme */
--splash-primary: #06ffa5;
--splash-secondary: #0077ff;
--splash-accent: #7209b7;
--splash-dark: #001122;

/* Sunset Theme */
--splash-primary: #ff6b35;
--splash-secondary: #f7931e;
--splash-accent: #ffcd3c;
--splash-dark: #2d1b69;
```

### Animation Timing

```css
/* Fast animations */
.splash-1 { animation-duration: 0.5s; }
.splash-2 { animation-duration: 0.7s; }
.splash-3 { animation-duration: 0.9s; }

/* Slow animations */
.splash-1 { animation-duration: 1.2s; }
.splash-2 { animation-duration: 1.5s; }
.splash-3 { animation-duration: 1.8s; }
```

### Splash Sizes

```css
/* Small splashes */
.splash-1 { width: 20px; height: 20px; }
.splash-2 { width: 35px; height: 35px; }
.splash-3 { width: 50px; height: 50px; }

/* Large splashes */
.splash-1 { width: 50px; height: 50px; }
.splash-2 { width: 80px; height: 80px; }
.splash-3 { width: 120px; height: 120px; }
```

## 🔧 API Reference

### Methods

| Method | Description | Parameters |
|--------|-------------|------------|
| `createSplash(x, y)` | Create a splash at coordinates | `x`: X position, `y`: Y position |
| `toggleEffect()` | Enable/disable the effect | None |
| `setTheme(theme)` | Change color theme | `theme`: 'cosmic', 'ocean', 'sunset' |

### Events

```javascript
// Listen for splash events
$(document).on('splash:created', function(e, data) {
    console.log('Splash created at:', data.x, data.y);
});

$(document).on('splash:destroyed', function(e, data) {
    console.log('Splash animation completed');
});
```

## 🌟 Examples

### E-commerce Landing Page
```html
<!-- Perfect for product showcases -->
<div class="product-hero">
    <h1>Discover Amazing Products</h1>
    <button class="cta-button">Shop Now</button>
</div>
```

### Portfolio Website
```html
<!-- Great for creative portfolios -->
<div class="portfolio-header">
    <h1>John Doe</h1>
    <p>Creative Developer</p>
</div>
```

### Gaming Website
```html
<!-- Ideal for gaming sites -->
<div class="game-banner">
    <h1>Epic Adventures Await</h1>
    <button class="play-button">Play Now</button>
</div>
```

## 🎯 Performance Tips

- **Throttle on mobile**: Reduce splash frequency on touch devices
- **Use will-change**: Add `will-change: transform` for better performance
- **Cleanup**: The effect automatically removes old splashes to prevent memory leaks
- **RAF optimization**: Uses `requestAnimationFrame` for smooth animations

## 📱 Browser Support

| Browser | Version |
|---------|---------|
| Chrome | 60+ |
| Firefox | 55+ |
| Safari | 12+ |
| Edge | 79+ |
| iOS Safari | 12+ |
| Android Chrome | 60+ |

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Commit your changes**: `git commit -m 'Add amazing feature'`
4. **Push to the branch**: `git push origin feature/amazing-feature`
5. **Open a Pull Request**

### Development Setup

```bash
# Clone the repo
git clone https://github.com/iamitpkumar/splash-cursor-effect.git
cd splash-cursor-effect

# Create a new feature
git checkout -b feature/your-feature-name

# Make your changes and test them
# Open index.html in your browser

# Commit and push
git add .
git commit -m "Add your feature description"
git push origin feature/your-feature-name
```

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by modern web design trends
- Built with love for the web development community
- Thanks to all contributors and users


---

<div align="center">
  <p>Made with ❤️ by <a href="https://github.com/iamitpkumar">Amit Kumar</a></p>
  <p>⭐ Star this repo if you found it helpful!</p>
</div>

## 🚀 What's Next?

- [ ] React/Vue component versions
- [ ] TypeScript support
- [ ] More animation presets
- [ ] Mobile touch optimizations
- [ ] Advanced theming system

---

**✨ Ready to make your website magical? Star this repo and let's create something amazing together!**
