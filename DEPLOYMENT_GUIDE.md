# Portfolio Website Deployment Guide

This guide will help you deploy your portfolio website to various platforms.

## Option 1: GitHub Pages (Recommended - Free & Easy)

GitHub Pages is perfect for hosting static websites directly from your GitHub repository.

### Steps to Deploy:

1. **Ensure your files are in the repository root or in a `docs` folder**
   - Current setup has files in the root (index.html, styles.css, script.js) ✓

2. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click on "Settings" tab
   - Scroll down to "Pages" section in the left sidebar
   - Under "Source", select the branch (e.g., `main`)
   - Select the folder: `/ (root)` or `/docs` depending on where your files are
   - Click "Save"

3. **Wait for deployment**
   - GitHub will automatically build and deploy your site
   - This usually takes 1-2 minutes
   - You'll see a green checkmark when it's ready

4. **Access your website**
   - Your site will be available at: `https://isandeep06.github.io/Tata-s-GenAI-Powered-Data-Analytics-on-Forage/`
   - GitHub will show you the URL in the Pages settings

### Custom Domain (Optional)
- You can add a custom domain in the GitHub Pages settings
- Add a `CNAME` file with your domain name
- Configure DNS settings with your domain provider

---

## Option 2: Netlify (Easy Drag & Drop)

Netlify offers free hosting with continuous deployment.

### Steps to Deploy:

1. **Sign up for Netlify**
   - Go to [netlify.com](https://netlify.com)
   - Sign up using your GitHub account

2. **Deploy your site**
   - Click "Add new site" → "Import an existing project"
   - Connect to GitHub and select your repository
   - Build settings:
     - Build command: (leave empty)
     - Publish directory: `/` (root)
   - Click "Deploy site"

3. **Access your website**
   - Netlify will provide a random URL (e.g., `random-name-123.netlify.app`)
   - You can change this to a custom subdomain in site settings

### Benefits:
- Automatic deployments on every push
- Free SSL certificate
- Custom domains
- Form handling (if you add contact forms later)

---

## Option 3: Vercel (Modern Platform)

Vercel is a modern deployment platform with excellent performance.

### Steps to Deploy:

1. **Sign up for Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Sign up using your GitHub account

2. **Import your project**
   - Click "Add New Project"
   - Select your GitHub repository
   - Vercel will auto-detect it's a static site
   - Click "Deploy"

3. **Access your website**
   - Vercel will provide a URL (e.g., `your-repo.vercel.app`)
   - Custom domains are available in settings

### Benefits:
- Lightning-fast CDN
- Automatic HTTPS
- Instant rollbacks
- Real-time collaboration

---

## Option 4: Traditional Web Hosting

If you have traditional web hosting (cPanel, FTP, etc.):

### Steps to Deploy:

1. **Prepare your files**
   - Download or export these files:
     - `index.html`
     - `styles.css`
     - `script.js`

2. **Upload via FTP**
   - Use an FTP client (FileZilla, Cyberduck, etc.)
   - Connect to your hosting server
   - Upload all three files to the `public_html` or `www` directory

3. **Access your website**
   - Visit your domain (e.g., `www.yourdomain.com`)

---

## Updating Your Website

After making changes to your portfolio:

### For GitHub Pages:
1. Commit and push changes to GitHub
2. GitHub Pages will automatically rebuild your site

### For Netlify/Vercel:
1. Commit and push changes to GitHub
2. Automatic deployment triggers
3. Changes go live in 1-2 minutes

### For Traditional Hosting:
1. Re-upload the modified files via FTP
2. Clear browser cache to see changes

---

## Testing Before Deployment

Always test your website locally before deploying:

```bash
# Start a local server
python3 -m http.server 8000

# Open browser to:
http://localhost:8000
```

---

## Troubleshooting

### Issue: Website not showing properly
- **Solution**: Clear browser cache or try incognito mode
- Check if all files (HTML, CSS, JS) are uploaded

### Issue: Fonts/Icons not loading
- **Solution**: Ensure you have internet connection (CDN resources need internet)
- Check browser console for errors

### Issue: GitHub Pages not updating
- **Solution**: Wait 5-10 minutes, GitHub Pages can be slow
- Check Actions tab for build status
- Try clearing GitHub cache: Settings → Pages → Change source and change back

---

## Performance Tips

1. **Optimize images** (if you add any):
   - Use WebP format
   - Compress images before uploading

2. **Enable caching**:
   - GitHub Pages and Netlify/Vercel handle this automatically

3. **Use a CDN**:
   - GitHub Pages uses GitHub's CDN
   - Netlify and Vercel have global CDNs

---

## Security

- GitHub Pages provides free HTTPS
- Netlify and Vercel provide free SSL certificates
- No sensitive data should be in your public repository

---

## Recommended: GitHub Pages

For this portfolio website, **GitHub Pages is recommended** because:
✓ It's free
✓ Integrated with your GitHub repository
✓ Automatic deployments on push
✓ Free HTTPS
✓ Good performance
✓ No additional account needed

Just enable it in Settings → Pages and your portfolio will be live!

---

## Next Steps After Deployment

1. Share your portfolio URL on LinkedIn
2. Add the URL to your GitHub profile
3. Include it in your resume
4. Test on different devices (mobile, tablet, desktop)
5. Share with friends for feedback

---

**Happy Deploying! 🚀**
