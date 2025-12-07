# Cositas Corona - Project Reference

## Services Used

- **Hosting**: Netlify (automatic deployments from GitHub)
- **Version Control**: GitHub
- **Payment Methods**: Venmo, Zelle, Cash, Bitcoin
- **Forms**: Netlify Forms (built-in form handling)

## Color Palette

### Primary Colors
- `#9a4513` - Dark brown (primary text, borders)
- `#b56324` - Medium brown
- `#d08030` - Golden brown (buttons, accents)
- `#cfa982` - Light tan (button gradients)
- `#8b6f47` - Wood brown (chalkboard border)

### Background Colors
- `#faf3e8` - Light cream (gradient start)
- `#f7e8c8` - Light yellow-cream (gradient end)
- Dark mode: `#9a4513` to `#b56324` gradient

### Text Colors
- `#f5f1e8` - Off-white (primary text on dark backgrounds)
- `#f0f0f0` - Light gray (chalkboard text)
- `#ffc107` - Amber/Gold (accents, Limited Time badge, location text)

### Chalkboard Sign Colors
- Background: `#2d3436` to `#1e272e` gradient
- Border: `#8b6f47` (wood brown)
- Inner border: `#654321` (dark wood)

### Opacity Variants
- `rgba(181, 99, 36, 0.96)` - Container background
- `rgba(154, 69, 19, 0.97)` - Container background gradient
- `rgba(208, 128, 48, 0.3)` - Input backgrounds, badges
- `rgba(207, 169, 130, 0.5)` - Borders, shadows

## Typography

### Fonts
- **Headings (h1)**: 'Brush Script MT', 'Lucida Handwriting', cursive
- **Body Text**: 'Georgia', serif
- **Form Elements**: 'Arial', sans-serif
- **Chalkboard**: 'Comic Sans MS', 'Chalkboard SE', 'Bradley Hand', 'Marker Felt', cursive

### Font Sizes
- h1: 5.5em (desktop), 4em (tablet), 3em (mobile)
- h2: 1.8em (desktop), 1.4em (mobile)
- h3 (location): 1.1em (desktop), 1em (mobile)
- Body: 1em - 1.1em
- Chalkboard text: 1.6em (desktop), 1.3em (mobile)

## Pricing

- 🍯 (1 jar) = $12
- 🍯🍯 (2 jars) = $20
- 🍯🍯🍯 (3 jars) = $32* (Limited Time)
- 🍯🍯🍯🍯 (4 jars) = $38* (Limited Time)

## Business Details

- **Service Areas**: Chula Vista and Tijuana
- **Order Timeline**: Up to 7 business days
- **Product**: Handmade, gourmet cajeta (goat's milk caramel)

## Ingredients

- Goat's milk
- Brown sugar* (organic)
- Cinnamon sticks* (organic)
- Vanilla extract* (organic)
- Baking soda
- Spiced rum

## Key Files

- `index.html` - English main page
- `index-es.html` - Spanish main page
- `thank-you.html` - English confirmation page
- `thank-you-es.html` - Spanish confirmation page

## Development Best Practices

### TODO: Recommended Improvements for Scaling

#### 1. Code Organization
- [ ] Extract CSS into separate stylesheet (`styles.css`)
- [ ] Create shared components for bilingual content
- [ ] Set up CSS variables for color palette
- [ ] Consider using a CSS preprocessor (SASS/LESS) for better organization

#### 2. Asset Management
- [ ] Create `/assets` folder structure:
  - `/assets/css/` - stylesheets
  - `/assets/js/` - JavaScript files
  - `/assets/images/` - images and icons
  - `/assets/fonts/` - custom fonts if needed

#### 3. Bilingual Support
- [x] **ALWAYS update both English and Spanish pages together**
- [x] Use proper Spanish accents (á, é, í, ó, ú, ñ, ¿, ¡)
- [x] Maintain formal register in Spanish (usted instead of tú)
- [ ] Consider using a templating system or static site generator
- [ ] Create a translation file/system for easier content management
- [ ] Ensure all new pages have both English and Spanish versions

**Current Bilingual Parity:**
- Location text: ✓ "Now serving Chula Vista and Tijuana" / "Ahora sirviendo Chula Vista y Tijuana"
- Styling: ✓ Both pages use same h3 golden italic styling
- Forms: ✓ Both have Netlify form integration

#### 4. Performance Optimization
- [ ] Minify CSS and JavaScript for production
- [ ] Optimize images (compress, use WebP format)
- [ ] Implement lazy loading for images
- [ ] Add caching headers via Netlify config

#### 5. SEO & Accessibility
- [ ] Add meta descriptions to all pages
- [ ] Implement Open Graph tags for social sharing
- [ ] Add favicon
- [ ] Ensure proper heading hierarchy (h1, h2, h3)
- [ ] Add alt text to images
- [ ] Test with screen readers

#### 6. Configuration Files
- [ ] Create `netlify.toml` for deployment configuration
- [ ] Add `.gitignore` for excluding unnecessary files
- [ ] Consider adding `robots.txt` and `sitemap.xml`

#### 7. Testing
- [ ] Test forms on multiple browsers
- [ ] Test mobile responsiveness on actual devices
- [ ] Validate HTML/CSS with W3C validators
- [ ] Test payment flow end-to-end

#### 8. Documentation
- [ ] Document form submission workflow
- [ ] Create style guide for future pages
- [ ] Document deployment process
- [ ] Keep component library/pattern reference

## Git Workflow

### Branch Strategy
- `main` - Production branch (auto-deploys to Netlify)
- Consider using feature branches for major changes

### Commit Message Format
- Use descriptive commit messages
- Format: `[Type] Brief description`
  - Types: Feature, Fix, Style, Docs, Refactor

## Netlify Configuration

### Current Setup
- Auto-deploy from GitHub main branch
- Forms enabled (Netlify Forms)
- Custom domain: (add when configured)

### Recommended Settings
- Enable HTTPS (should be default)
- Set up branch deploys for testing
- Configure custom headers for security
- Set up form notifications

## File Structure (Current)

```
cositas/
├── index.html              # English main page
├── index-es.html           # Spanish main page
├── thank-you.html          # English confirmation
├── thank-you-es.html       # Spanish confirmation
├── project-reference.md    # This file
└── .git/                   # Git repository
```

## File Structure (Recommended Future)

```
cositas/
├── index.html
├── index-es.html
├── thank-you.html
├── thank-you-es.html
├── assets/
│   ├── css/
│   │   └── styles.css
│   ├── js/
│   │   └── main.js
│   └── images/
│       └── favicon.ico
├── docs/
│   ├── project-reference.md
│   └── style-guide.md
├── netlify.toml
├── .gitignore
└── README.md
```

## Environment Variables (if needed later)

Document any API keys or sensitive data here:
- Payment gateway credentials (keep in Netlify environment variables)
- Analytics tracking IDs
- Email service API keys

## Browser Support

Target browsers:
- Chrome (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Edge (latest 2 versions)
- Mobile: iOS Safari, Chrome Mobile

## Recent Changes Log

### 2024-12-07
- Added "Now serving Chula Vista and Tijuana" location text
- Styled location text with golden italic styling (#ffc107)
- Added mobile responsive styling for location text
- Created project reference documentation

### Previous
- Improved Limited Time badge spacing (margin-top: 10px)
- Restored Spanish accents: envíe, información, hábiles, más
- Updated Spanish formality (tu → su, permite → permita)
- Restored chalkboard pricing section
- Added Spanish page (index-es.html)
