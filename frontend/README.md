# TrustLens Frontend

This is the frontend application for the TrustLens AI Analyst platform, providing an intuitive web interface for financial analysis and fraud detection.

## 🏗️ Frontend Structure

```
frontend/
├── index.html          # Main landing page with AI Analyst dashboard
├── fraudcheck.html     # Dedicated fraud detection interface  
├── styles.css          # Complete styling for both pages
└── script.js           # Frontend JavaScript functionality
```

## 🎨 Features

### Main Website (index.html)
- **Hero Section**: Financial intelligence platform overview
- **Feature Showcase**: Real-time analytics, security, India-first approach
- **Pricing Plans**: Basic, Professional, and Enterprise tiers
- **AI Analyst Demo**: Live transaction processing simulation
- **Contact Form**: Lead generation and customer inquiries

### Fraud Detection Interface (fraudcheck.html)
- **Transaction Submission**: Submit transactions for real-time fraud analysis
- **Results Display**: Visual fraud detection results with detailed indicators
- **Transaction History**: View all processed transactions with statistics
- **API Testing**: Built-in tools to test backend API endpoints
- **Mobile Responsive**: Works seamlessly on all devices

## 🎯 Technology Stack

- **HTML5**: Semantic markup with accessibility features
- **CSS3**: Modern styling with gradients, animations, and responsive design
- **JavaScript (ES6+)**: Interactive functionality and API integration
- **TailwindCSS**: Utility-first CSS framework (loaded via CDN)
- **Responsive Design**: Mobile-first approach

## 🚀 Getting Started

### 1. Simple Setup
Just open the HTML files in your web browser:
- Double-click `index.html` for the main website
- Double-click `fraudcheck.html` for fraud detection

### 2. With Local Server (Recommended)
For full functionality, serve the files through a local web server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (if you have live-server installed)
npx live-server

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

### 3. Backend Connection
The fraud detection interface requires the backend API to be running:
- Start the backend server first (see backend/README.md)
- The frontend will connect to `http://localhost:3001` by default

## 🔧 Configuration

### API Connection
The fraud detection API endpoint is configured in `fraudcheck.html`:
```javascript
const API_BASE = 'http://localhost:3001';
```

To change the backend URL, update this variable.

### Styling Customization
Main styling is in `styles.css` with these key sections:
- **Variables**: CSS custom properties for colors and spacing
- **Hero Section**: Landing page styling
- **Dashboard Components**: Financial dashboard cards and animations
- **Fraud Interface**: Fraud detection specific styling
- **Responsive**: Mobile and tablet breakpoints

## 🎨 Design System

### Color Palette
- **Primary Blue**: `#0084ff` - Main brand color
- **Secondary Blue**: `#00c6ff` - Accent and gradients
- **Dark Background**: `#050a24` - Primary background
- **Success Green**: `#10b981` - Safe transactions
- **Danger Red**: `#ef4444` - Fraud alerts
- **Warning Orange**: `#ff6b00` - Alerts and notifications

### Typography
- **Main Font**: Segoe UI, Tahoma, Geneva, Verdana, sans-serif
- **Headers**: Bold weights with gradient text effects
- **Body**: Regular weight with good line spacing
- **Monospace**: For API responses and technical data

## 📱 Responsive Breakpoints

```css
/* Mobile First Approach */
/* Small phones: default styles */
/* Large phones: 480px+ */
/* Tablets: 768px+ */
/* Desktop: 1024px+ */
/* Large desktop: 1200px+ */
```

## ⚡ Performance Features

- **Optimized Images**: SVG icons and optimized assets
- **Minimal Dependencies**: Only TailwindCSS via CDN
- **Efficient Animations**: CSS transforms and transitions
- **Lazy Loading**: Progressive feature loading
- **Caching**: Browser caching for static assets

## 🔒 Security Considerations

- **Input Validation**: Client-side validation for forms
- **HTTPS Ready**: Designed to work with HTTPS in production
- **No Secrets**: No API keys or sensitive data in frontend code
- **CORS Compliant**: Works with backend CORS configuration

## 🧪 Testing the Interface

### Fraud Detection Testing
1. **Safe Transaction**: Use normal amounts and valid Indian locations
2. **Trigger Fraud**: Use account `9876543210` as recipient
3. **High Amount**: Try amounts over ₹100,000
4. **Geographic Test**: Submit from different cities quickly
5. **API Test**: Use built-in API testing buttons

### Browser Compatibility
Tested on:
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ✅ Mobile browsers (iOS/Android)

## 🔄 Development Workflow

### File Organization
- `index.html` - Main website structure and content
- `fraudcheck.html` - Fraud detection app structure
- `styles.css` - All styling (shared between pages)
- `script.js` - Shared JavaScript functionality

### Making Changes
1. Edit HTML for structural changes
2. Update CSS for styling modifications  
3. Modify JavaScript for functionality changes
4. Test in multiple browsers and devices
5. Check mobile responsiveness

## 🌟 Advanced Features

### Animation System
- **Logo Animations**: SVG path drawing and hover effects
- **Counter Animations**: Number counting for statistics
- **Scroll Animations**: Elements animate on scroll
- **Loading States**: Smooth loading indicators

### Interactive Elements
- **Smart Navigation**: Active link highlighting
- **Mobile Menu**: Responsive hamburger menu
- **Form Validation**: Real-time input validation
- **API Integration**: Dynamic content loading

### Accessibility
- **Semantic HTML**: Proper heading structure and ARIA labels
- **Keyboard Navigation**: Full keyboard accessibility
- **High Contrast**: Good color contrast ratios
- **Screen Reader**: Compatible with assistive technologies

## 🚀 Production Deployment

### Optimization Checklist
- [ ] Minify CSS and JavaScript
- [ ] Optimize images and assets
- [ ] Enable gzip compression
- [ ] Set up CDN for static files
- [ ] Configure caching headers
- [ ] Test on various devices and browsers

### Environment Configuration
Update API endpoints for production:
```javascript
const API_BASE = 'https://your-api-domain.com';
```

---

**🎨 Beautifully designed, 🚀 lightning fast, and 🇮🇳 built for India!**
