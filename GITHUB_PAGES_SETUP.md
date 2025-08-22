# GitHub Pages Setup Guide

This guide will help you set up GitHub Pages for your Madrid Parks app landing page.

## Step 1: Enable GitHub Pages

1. Go to your GitHub repository
2. Click on **Settings** tab
3. Scroll down to **Pages** section (in the left sidebar)
4. Under **Source**, select **Deploy from a branch**
5. Choose **gh-pages** branch
6. Click **Save**

## Step 2: Push Your Changes

The GitHub Actions workflow will automatically deploy your site when you push to the main branch:

```bash
git add .
git commit -m "Add landing page for GitHub Pages"
git push origin main
```

## Step 3: Wait for Deployment

1. Go to **Actions** tab in your repository
2. You should see the "Deploy to GitHub Pages" workflow running
3. Wait for it to complete (usually takes 2-3 minutes)
4. Your site will be available at: `https://yourusername.github.io/retiropark_app`

## Step 4: Add Screenshots

To make the landing page complete, add your app screenshots to the `assets/` folder:

- `assets/screenshot-main.png` - Main app interface
- `assets/screenshot-settings.png` - Settings screen  
- `assets/screenshot-map.png` - Map view

## Step 5: Customize

- Update the GitHub link in the footer with your actual username
- Modify colors, text, or layout as needed
- Add more features or sections

## Troubleshooting

- If the site doesn't appear, check the Actions tab for any errors
- Make sure the `gh-pages` branch was created automatically
- Verify that GitHub Pages is enabled in repository settings
- Check that the workflow has the necessary permissions

## Next Steps

Once your site is live, you can:
- Use the URL in your App Store submission
- Share it on social media
- Include it in your portfolio/CV
- Customize it further for your needs

Your landing page will automatically update whenever you push changes to the main branch!
