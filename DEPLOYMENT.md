# Deployment Guide for GitHub Pages

This guide will help you deploy your Asthra demo page to GitHub Pages.

## Prerequisites

- A GitHub account
- Git installed on your local machine
- Node.js and npm installed

## Step 1: Push to GitHub

1. Create a new repository on GitHub (or use an existing one)
2. Initialize git in your project directory:
```bash
git init
git add .
git commit -m "Initial commit: Asthra demo page"
```

3. Add your GitHub repository as remote:
```bash
git remote add origin https://github.com/your-username/asthra.git
```

4. Push to GitHub:
```bash
git push -u origin main
```

## Step 2: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" section in the left sidebar
4. Under "Source", select "GitHub Actions"
5. Save the settings

## Step 3: Automatic Deployment

The GitHub Actions workflow (`.github/workflows/deploy.yml`) will automatically:
- Build your Next.js app
- Generate static files
- Deploy to GitHub Pages

Every time you push to the `main` branch, the site will be automatically updated.

## Step 4: Access Your Site

Your site will be available at:
```
https://your-username.github.io/asthra
```

## Manual Deployment (Alternative)

If you prefer manual deployment:

1. Build the static site:
```bash
npm run build:static
```

2. Install gh-pages:
```bash
npm install --save-dev gh-pages
```

3. Add deploy script to package.json:
```json
"scripts": {
  "deploy": "gh-pages -d out"
}
```

4. Deploy:
```bash
npm run deploy
```

## Troubleshooting

### Build Fails
- Check that all dependencies are installed: `npm install`
- Ensure there are no TypeScript or ESLint errors
- Verify Next.js configuration in `next.config.ts`

### Site Not Loading
- Check GitHub Pages settings
- Verify the repository is public (required for free GitHub Pages)
- Wait a few minutes for the deployment to complete

### Styling Issues
- Ensure Tailwind CSS is properly configured
- Check that all CSS classes are valid
- Verify the build output includes CSS files

## Custom Domain (Optional)

To use a custom domain:

1. Add a `CNAME` file to the `public` directory with your domain
2. Configure DNS settings with your domain provider
3. Update GitHub Pages settings to use your custom domain

## Performance Tips

- Images are automatically optimized by Next.js
- Static export ensures fast loading times
- Tailwind CSS is purged in production builds
- All assets are minified and compressed

## Support

If you encounter issues:
1. Check the GitHub Actions logs
2. Review the build output
3. Ensure all files are committed and pushed
4. Verify GitHub Pages settings

---

Your Asthra demo page is now ready to showcase your projects! 🚀
