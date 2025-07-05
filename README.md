# Elite Motors - Premium Car Dealership Website

A modern, responsive car dealership website built with React, featuring a sleek dark theme, interactive inventory management, and professional design.

## 🚗 Features

### Core Functionality
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Interactive Navigation**: Smooth scrolling navigation with fixed header
- **Vehicle Inventory**: Advanced search and filtering system
- **Contact System**: Professional contact forms with validation
- **Modern UI**: Dark theme with red accent colors and smooth animations

### Sections
1. **Hero Section**: Eye-catching landing area with company stats
2. **Inventory**: Searchable car catalog with filtering options
3. **Services**: Comprehensive service offerings with testimonials
4. **About**: Company story, values, and team information
5. **Contact**: Multiple contact methods and location details
6. **Footer**: Links, newsletter signup, and certifications

### Interactive Features
- **Search Functionality**: Real-time vehicle search
- **Category Filtering**: Filter by Luxury, Sports, SUV categories
- **Price Filtering**: Filter by price ranges
- **Contact Form**: Validated form with success feedback
- **Smooth Animations**: Hover effects and transitions
- **Mobile Menu**: Responsive navigation for mobile devices

## 🛠️ Technology Stack

- **Frontend**: React 18 with JSX
- **Styling**: Tailwind CSS with custom design system
- **Icons**: Lucide React icons
- **UI Components**: shadcn/ui components
- **Build Tool**: Vite
- **Package Manager**: pnpm

## 📁 Project Structure

```
car-dealership/
├── public/                 # Static assets
├── src/
│   ├── assets/
│   │   └── cars/          # Car images
│   ├── components/        # React components
│   │   ├── ui/           # UI components (shadcn/ui)
│   │   ├── Header.jsx    # Navigation header
│   │   ├── Hero.jsx      # Hero section
│   │   ├── Inventory.jsx # Car inventory
│   │   ├── Services.jsx  # Services section
│   │   ├── About.jsx     # About section
│   │   ├── Contact.jsx   # Contact section
│   │   └── Footer.jsx    # Footer
│   ├── App.jsx           # Main app component
│   ├── App.css           # Global styles
│   └── main.jsx          # Entry point
├── package.json          # Dependencies
└── README.md            # This file
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- pnpm (recommended) or npm

### Installation

1. **Clone or extract the project**
   ```bash
   cd car-dealership
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   # or
   npm install
   ```

3. **Start development server**
   ```bash
   pnpm run dev
   # or
   npm run dev
   ```

4. **Open in browser**
   Navigate to `http://localhost:5173`

### Build for Production

```bash
pnpm run build
# or
npm run build
```

The built files will be in the `dist/` directory.

## 🎨 Design Features

### Color Scheme
- **Primary**: Black (#000000) and Dark Gray (#1F2937)
- **Accent**: Red (#DC2626) with gradients
- **Text**: White and Gray variants
- **Interactive**: Hover states with color transitions

### Typography
- **Headings**: Bold, large sizes with gradient text effects
- **Body**: Clean, readable fonts with proper contrast
- **UI Elements**: Consistent sizing and spacing

### Layout
- **Grid System**: Responsive CSS Grid and Flexbox
- **Spacing**: Consistent padding and margins
- **Breakpoints**: Mobile-first responsive design

## 🚗 Inventory Data

The website includes sample data for 6 premium vehicles:

1. **Ferrari 488 GTB** - $299,000 (Sports)
2. **Lamborghini Huracán** - $275,000 (Sports)
3. **Mercedes-Benz S-Class** - $125,000 (Luxury)
4. **BMW X7 M50i** - $98,000 (SUV)
5. **Porsche 911 Turbo S** - $230,000 (Sports)
6. **Range Rover Autobiography** - $145,000 (SUV)

Each vehicle includes:
- High-quality images
- Detailed specifications
- Pricing information
- Location details
- Feature highlights

## 📱 Responsive Design

The website is fully responsive with breakpoints for:
- **Mobile**: 320px - 768px
- **Tablet**: 768px - 1024px
- **Desktop**: 1024px and above

## 🔧 Customization

### Adding New Vehicles
Edit the `cars` array in `src/components/Inventory.jsx`:

```javascript
const cars = [
  {
    id: 7,
    name: 'Your Car Name',
    category: 'luxury', // 'luxury', 'sports', or 'suv'
    price: 150000,
    year: 2024,
    mileage: 100,
    fuel: 'Gasoline',
    transmission: 'Automatic',
    image: yourCarImage,
    features: ['Feature 1', 'Feature 2', 'Feature 3'],
    location: 'Your Location'
  }
  // ... add more cars
]
```

### Updating Company Information
- **Header**: Edit `src/components/Header.jsx`
- **About**: Edit `src/components/About.jsx`
- **Contact**: Edit `src/components/Contact.jsx`
- **Footer**: Edit `src/components/Footer.jsx`

### Styling Changes
- **Colors**: Modify CSS variables in `src/App.css`
- **Components**: Update Tailwind classes in component files
- **Layout**: Adjust grid and flexbox properties

## 🌐 Deployment Options

### Static Hosting (Recommended)
1. Build the project: `pnpm run build`
2. Deploy the `dist/` folder to:
   - Vercel
   - Netlify
   - GitHub Pages
   - AWS S3
   - Any static hosting service

### Server Deployment
The built files can be served by any web server (Apache, Nginx, etc.)

## 📞 Support

For questions or customization requests, contact the development team.

## 📄 License

This project is created for Elite Motors. All rights reserved.

---

**Elite Motors** - Premium Car Dealership Since 1995

