# Asthra

A modern, responsive demo page built with Next.js 15, TypeScript, and Tailwind CSS. This project demonstrates how to create beautiful static sites that can be easily deployed to GitHub Pages.

## 🚀 Features

- **Next.js 15** - Latest version with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **Static Export** - Optimized for GitHub Pages deployment
- **Responsive Design** - Looks great on all devices
- **Modern UI** - Gradient backgrounds, glassmorphism effects, and smooth animations
- **GitHub Actions** - Automated deployment workflow

## 🛠️ Tech Stack

- [Next.js 15](https://nextjs.org/) - React framework
- [TypeScript](https://www.typescriptlang.org/) - Type safety
- [Tailwind CSS](https://tailwindcss.com/) - Styling
- [GitHub Pages](https://pages.github.com/) - Hosting
- [GitHub Actions](https://github.com/features/actions) - CI/CD

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/your-username/asthra.git
cd asthra
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🏗️ Build for Production

To build the static site for GitHub Pages:

```bash
npm run build:static
```

This will create an `out` directory with the static files ready for deployment.

## 🚀 Deployment to GitHub Pages

### Automatic Deployment (Recommended)

1. Push your code to the `main` branch
2. Go to your repository settings
3. Navigate to "Pages" in the left sidebar
4. Under "Source", select "GitHub Actions"
5. The site will automatically deploy when you push to the main branch

### Manual Deployment

1. Build the static site:
```bash
npm run build:static
```

2. Push the `out` directory to the `gh-pages` branch:
```bash
npx gh-pages -d out
```

## 📁 Project Structure

```
asthra/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions workflow
├── src/
│   └── app/
│       ├── page.tsx            # Main page component
│       ├── layout.tsx          # Root layout
│       └── globals.css         # Global styles
├── next.config.ts              # Next.js configuration
├── package.json                # Dependencies and scripts
├── tailwind.config.ts          # Tailwind CSS configuration
└── README.md                   # This file
```

## 🎨 Customization

### Colors and Styling

The design uses a purple and pink gradient theme. You can customize the colors by modifying the Tailwind classes in `src/app/page.tsx`:

- Primary gradient: `from-purple-500 to-pink-500`
- Background gradient: `from-slate-900 via-purple-900 to-slate-900`
- Accent colors: Various purple, pink, blue, and green shades

### Content

Edit `src/app/page.tsx` to customize:
- Hero section text
- Features section
- About section
- Contact information
- Navigation links

### Configuration

- **Next.js config**: `next.config.ts` - Configure static export and GitHub Pages settings
- **Tailwind config**: `tailwind.config.ts` - Customize design system
- **Package.json**: Add or modify build scripts

## 🔧 Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production (with Turbopack)
- `npm run build:static` - Build static site for GitHub Pages
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

### Adding New Pages

1. Create a new file in `src/app/` directory
2. Export a default React component
3. The page will be automatically available at the corresponding route

### Adding Components

1. Create components in `src/components/` directory
2. Import and use them in your pages
3. Use TypeScript for type safety

## 📱 Responsive Design

The site is fully responsive and includes:
- Mobile-first design approach
- Flexible grid layouts
- Responsive typography
- Touch-friendly interactive elements
- Optimized images and assets

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## 📞 Support

If you have any questions or need help, please:
- Open an issue on GitHub
- Check the documentation
- Review the code examples

---

Built with ❤️ using Next.js 15, TypeScript, and Tailwind CSS.