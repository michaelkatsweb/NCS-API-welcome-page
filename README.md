[README.md](https://github.com/user-attachments/files/22986930/README.md)
# NCS-API Website

> **High-Performance Clustering API with Interactive Web Interface**

A modern, production-ready web application for the NCS (Neural Clustering System) API, featuring real-time clustering algorithms, interactive visualizations, and comprehensive documentation.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/michaelkatsweb/NCS-API-Website)
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/michaelkatsweb/NCS-API-Website)
[![Netlify Status](https://api.netlify.com/api/v1/badges/your-site-id/deploy-status)](https://app.netlify.com/sites/your-site/deploys)

## 🚀 **Live Demo**

- **🏠 Website**: [ncs-api.com](https://ncs-api.com)
- **🎮 Playground**: [ncs-api.com/playground](https://ncs-api.com/playground)
- **📚 Documentation**: [ncs-api.com/docs](https://ncs-api.com/docs)
- **📊 Benchmarks**: [ncs-api.com/benchmarks](https://ncs-api.com/benchmarks)
- **💡 Examples**: [ncs-api.com/examples](https://ncs-api.com/examples)

## ✨ **Features**

### 🎯 **Core Functionality**
- **Interactive Clustering Playground** - Upload data, run algorithms, visualize results in real-time
- **Multiple Algorithm Support** - K-Means, DBSCAN, Hierarchical, and proprietary NCS algorithm
- **Real-time Performance Monitoring** - Live metrics, benchmarks, and algorithm comparisons
- **Advanced Data Processing** - CSV/JSON/Excel upload with validation and preprocessing
- **Professional Visualizations** - 2D/3D scatter plots, heatmaps, dendrograms with smooth animations

### 🛠️ **Developer Experience**
- **Interactive API Documentation** - Live API explorer with code generation
- **Multi-language Examples** - JavaScript, Python, R, and cURL code samples
- **Code Generator** - Automatic client code generation in multiple languages
- **Real-time Collaboration** - Share clustering sessions and results
- **Comprehensive Testing Suite** - Unit, integration, and end-to-end tests

### 🎨 **User Interface**
- **Modern Responsive Design** - Works flawlessly on desktop, tablet, and mobile
- **Dark/Light Theme Support** - Automatic system preference detection
- **Progressive Web App (PWA)** - Offline capabilities and native app experience
- **Accessibility First** - WCAG 2.1 AA compliant with screen reader support
- **Smooth Animations** - 60fps animations and transitions throughout

### ⚡ **Performance**
- **Web Workers** - Background processing for large datasets without UI blocking
- **Smart Caching** - Intelligent caching strategies for optimal performance
- **Lazy Loading** - Progressive asset loading for faster initial page loads
- **Service Worker** - Offline functionality and background sync
- **Optimized Bundle** - Code splitting and tree shaking for minimal bundle size

## 📁 **Project Structure**

```
ncs-api-website/
│
├── 📄 index.html                       # Landing page with hero section
├── 📄 playground.html                  # Interactive clustering playground
├── 📄 docs.html                       # API documentation & explorer
├── 📄 benchmarks.html                 # Performance metrics & comparisons
├── 📄 examples.html                   # Use cases & sample implementations
├── 📄 manifest.json                   # PWA manifest
├── 📄 sw.js                           # Service worker for PWA
├── 📄 package.json                    # Project metadata & build scripts
├── 📄 .gitignore                      # Git ignore rules
├── 📄 README.md                       # Project documentation
│
├── 📁 assets/                         # Static assets
│   ├── 📁 data/                       # Sample datasets
│   │   ├── 📊 iris.csv                # Classic iris dataset
│   │   ├── 📊 customers.csv           # Customer segmentation sample
│   │   ├── 📊 ecommerce.csv           # E-commerce behavior data
│   │   ├── 📊 financial.csv           # Financial data clustering
│   │   └── 📊 socialmedia.csv         # Social media clustering
│   │
│   └── 📁 images/                     # Images & icons
│       ├── 🖼️ favicon.svg            # SVG favicon
│       ├── 🖼️ favicon.png            # PNG favicon fallback
│       └── 📁 icons/                 # UI icons
│
└── 📁 tests/                         # Test suite
    ├── 📁 unit/                       # Unit tests
    ├── 📁 integration/                # Integration tests
    └── 📁 e2e/                        # End-to-end tests
```

## 🚀 **Quick Start**

### Prerequisites

- **Node.js** 16.0.0 or higher
- **npm** 8.0.0 or higher
- Modern web browser (Chrome 80+, Firefox 75+, Safari 13+, Edge 80+)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/michaelkatsweb/NCS-API-Website.git
   cd NCS-API-Website
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   - Navigate to `http://localhost:3000`
   - The website should load with hot reload enabled

### Alternative Setup (Static Files)

If you prefer to serve static files without Node.js:

```bash
# Using Python (if you have Python installed)
python -m http.server 3000

# Using PHP (if you have PHP installed)
php -S localhost:3000

# Using any static file server
npx serve .
```

## 🛠️ **Development**

### Available Scripts

```bash
# Start development server with hot reload
npm run dev

# Build for production
npm run build

# Serve production build locally
npm run preview

# Run all tests
npm test

# Run only unit tests
npm run test:unit

# Run end-to-end tests
npm run test:e2e

# Lint and fix code
npm run lint:fix

# Format code with Prettier
npm run format

# Check accessibility
npm run accessibility

# Run performance audit with Lighthouse
npm run lighthouse

# Analyze bundle size
npm run analyze
```

### Development Workflow

1. **Feature Development**
   ```bash
   git checkout -b feature/your-feature-name
   npm run dev
   # Make your changes
   npm run test
   npm run lint:fix
   git commit -m "feat: add your feature"
   git push origin feature/your-feature-name
   ```

2. **Testing**
   ```bash
   # Run all tests
   npm test
   
   # Run tests in watch mode
   npm run test:watch
   
   # Generate coverage report
   npm run test:coverage
   ```

3. **Code Quality**
   ```bash
   # Lint JavaScript/CSS/HTML
   npm run lint
   
   # Auto-fix linting issues
   npm run lint:fix
   
   # Format all files
   npm run format
   
   # Validate HTML
   npm run validate
   ```

### Environment Variables

Create a `.env.local` file in the root directory:

```env
# API Configuration
NCS_API_BASE_URL=https://api.ncs-clustering.com/v1
NCS_API_KEY=your-development-api-key

# Development Settings
NODE_ENV=development
PORT=3000
HOST=localhost

# Feature Flags
ENABLE_DEBUG=true
ENABLE_HOT_RELOAD=true
ENABLE_ANALYTICS=false

# External Services
GOOGLE_ANALYTICS_ID=GA-XXXXXXXXX
HOTJAR_ID=your-hotjar-id
```

## 📊 **Sample Datasets**

The website includes several sample datasets for testing clustering algorithms:

### Iris Dataset (150 samples, 4 features)
- **File**: `assets/data/iris.csv`
- **Features**: sepal_length, sepal_width, petal_length, petal_width
- **Use Case**: Classic machine learning classification problem

### Customer Segmentation (200 samples, 9 features)
- **File**: `assets/data/customers.csv`
- **Features**: age, income, spending_score, gender, region, etc.
- **Use Case**: E-commerce customer behavior analysis

### E-commerce Analytics (200 samples, 16 features)
- **File**: `assets/data/ecommerce.csv`
- **Features**: session_duration, page_views, conversions, device_type, etc.
- **Use Case**: User behavior and conversion optimization

### Financial Data (108 samples, 15 features)
- **File**: `assets/data/financial.csv`
- **Features**: market_cap, pe_ratio, revenue_growth, volatility, etc.
- **Use Case**: Stock market analysis and portfolio optimization

### Social Media (180 samples, 13 features)
- **File**: `assets/data/socialmedia.csv`
- **Features**: followers_count, engagement_rate, activity_level, etc.
- **Use Case**: Influencer analysis and content strategy

## 🚀 **Deployment**

### Netlify Deployment (Recommended)

1. **Connect to Netlify**
   ```bash
   # Install Netlify CLI
   npm install -g netlify-cli
   
   # Login to Netlify
   netlify login
   
   # Initialize site
   netlify init
   ```

2. **Configure Build Settings**
   - Build command: `npm run build`
   - Publish directory: `build`
   - Environment variables: Add your API keys

3. **Deploy**
   ```bash
   # Deploy to production
   npm run deploy
   
   # Deploy preview
   netlify deploy
   ```

### Alternative Deployment Options

**Vercel**
```bash
npm install -g vercel
vercel --prod
```

**GitHub Pages**
```bash
npm run build
# Push build folder to gh-pages branch
```

**AWS S3 + CloudFront**
```bash
aws s3 sync build/ s3://your-bucket-name
aws cloudfront create-invalidation --distribution-id YOUR_ID --paths "/*"
```

### Production Environment Variables

```env
NODE_ENV=production
NCS_API_BASE_URL=https://api.ncs-clustering.com/v1
NCS_API_KEY=your-production-api-key
ENABLE_ANALYTICS=true
GOOGLE_ANALYTICS_ID=GA-XXXXXXXXX
```

## 🧪 **Testing**

### Test Strategy

- **Unit Tests**: Individual functions and components
- **Integration Tests**: API interactions and data flow
- **End-to-End Tests**: Complete user journeys
- **Performance Tests**: Lighthouse audits and load testing
- **Accessibility Tests**: WCAG compliance validation

### Running Tests

```bash
# Run all tests
npm test

# Unit tests with Jest
npm run test:unit

# E2E tests with Playwright
npm run test:e2e

# Visual regression tests
npm run test:visual

# Performance tests
npm run test:performance

# Accessibility tests
npm run test:a11y
```

### Test Coverage

Current test coverage targets:
- **Unit Tests**: >90%
- **Integration Tests**: >80%
- **E2E Tests**: Critical user paths
- **Performance**: Lighthouse score >90
- **Accessibility**: WCAG 2.1 AA compliance

## 📈 **Performance**

### Optimization Techniques

- **Code Splitting**: Dynamic imports for route-based splitting
- **Tree Shaking**: Remove unused code from bundles
- **Image Optimization**: WebP format with fallbacks
- **Caching**: Service worker with smart caching strategies
- **Compression**: Gzip/Brotli compression for all assets
- **CDN**: Static assets served from global CDN

### Performance Metrics

- **First Contentful Paint**: <1.5s
- **Largest Contentful Paint**: <2.5s
- **Cumulative Layout Shift**: <0.1
- **First Input Delay**: <100ms
- **Time to Interactive**: <3.5s

### Bundle Analysis

```bash
# Analyze bundle size
npm run analyze

# Check bundle composition
npm run bundle-analyzer

# Monitor performance
npm run lighthouse
```

## ♿ **Accessibility**

### Compliance Standards

- **WCAG 2.1 Level AA** compliance
- **Section 508** federal accessibility requirements
- **ADA** Americans with Disabilities Act compliance
- **EN 301 549** European accessibility standard

### Accessibility Features

- **Semantic HTML**: Proper heading structure and landmarks
- **ARIA Labels**: Comprehensive ARIA implementation
- **Keyboard Navigation**: Full keyboard accessibility
- **Screen Reader Support**: Optimized for assistive technologies
- **Color Contrast**: WCAG AA compliant color ratios
- **Focus Management**: Visible focus indicators
- **Alternative Text**: Descriptive alt text for all images

### Testing Accessibility

```bash
# Run accessibility audit
npm run accessibility

# Test with screen reader
npm run test:screen-reader

# Validate ARIA implementation
npm run test:aria

# Check color contrast
npm run test:contrast
```

## 🔒 **Security**

### Security Measures

- **Content Security Policy (CSP)**: Strict CSP headers
- **HTTPS Enforcement**: All traffic encrypted
- **Input Validation**: Client-side and server-side validation
- **XSS Protection**: Protection against cross-site scripting
- **CSRF Protection**: Cross-site request forgery prevention
- **Secure Headers**: Security-focused HTTP headers

### Environment Security

```bash
# Security audit
npm audit

# Fix vulnerabilities
npm audit fix

# Check for security issues
npm run security-check
```

## 🤝 **Contributing**

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Quick Contribution Guide

1. **Fork the repository**
2. **Create your feature branch**: `git checkout -b feature/amazing-feature`
3. **Make your changes**: Follow our coding standards
4. **Add tests**: Ensure your changes are tested
5. **Commit your changes**: `git commit -m 'feat: add amazing feature'`
6. **Push to the branch**: `git push origin feature/amazing-feature`
7. **Open a Pull Request**: Describe your changes clearly

### Development Standards

- **Code Style**: ESLint + Prettier configuration
- **Commit Messages**: Conventional Commits specification
- **Testing**: Maintain >90% test coverage
- **Documentation**: Update README and inline comments
- **Accessibility**: Ensure WCAG 2.1 AA compliance

## 📝 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 **Team**

- **Project Lead**: [Michael Kats](https://github.com/michaelkatsweb)
- **Frontend Development**: NCS-API Team
- **UI/UX Design**: Design Team
- **API Development**: Backend Team

## 🙏 **Acknowledgments**

- **Chart.js** - Beautiful, responsive charts
- **Three.js** - 3D visualization capabilities
- **Prism.js** - Syntax highlighting for code examples
- **Inter Font** - Modern, readable typography
- **Netlify** - Reliable hosting and deployment
- **Open Source Community** - For the amazing tools and libraries

## 📞 **Support**

- **Documentation**: [ncs-api.com/docs](https://ncs-api.com/docs)
- **Issues**: [GitHub Issues](https://github.com/michaelkatsweb/NCS-API-Website/issues)
- **Discussions**: [GitHub Discussions](https://github.com/michaelkatsweb/NCS-API-Website/discussions)
- **Email**: support@ncs-api.com
- **Twitter**: [@NCS_API](https://twitter.com/NCS_API)

## 🗺️ **Roadmap**

### Version 1.1 (Q2 2025)
- [ ] Real-time collaborative clustering
- [ ] Advanced data preprocessing tools
- [ ] Custom algorithm support
- [ ] Mobile app companion

### Version 1.2 (Q3 2025)
- [ ] Machine learning model integration
- [ ] Advanced visualization options
- [ ] Enterprise SSO integration
- [ ] Multi-language support

### Version 2.0 (Q4 2025)
- [ ] AI-powered clustering recommendations
- [ ] Advanced analytics dashboard
- [ ] Enterprise deployment options
- [ ] Full API v2 integration

---

<div align="center">

**[⭐ Star this repo](https://github.com/michaelkatsweb/NCS-API-Website) if you find it helpful!**

Made with ❤️ by the NCS-API Team

</div>
