# 🧪 Local Testing Guide

This guide will help you test your website locally before pushing changes to GitHub.

## 🚀 Quick Start - Local Testing

### Method 1: Using the Start Server Script (Recommended)

1. Open Terminal
2. Navigate to the project directory:
   ```bash
   cd "/Users/tim.chowdary/cursor/Professional Website"
   ```

3. Run the server script:
   ```bash
   ./start-server.sh
   ```

4. Open your browser and go to:
   ```
   http://localhost:8000
   ```

5. To stop the server, press `Ctrl + C` in the terminal

### Method 2: Direct Python Command

If you prefer to run the command directly:

```bash
cd "/Users/tim.chowdary/cursor/Professional Website"
python3 -m http.server 8000
```

Then open: http://localhost:8000

---

## 📋 Complete Workflow: Edit → Test → Deploy

### Step 1: Make Your Changes
Edit your files (`index.html`, `css/style.css`, `js/script.js`, etc.)

### Step 2: Test Locally
```bash
# Start local server
./start-server.sh

# Open in browser: http://localhost:8000
```

**Test everything:**
- ✅ Click all buttons (Email, Mobile, GitHub, LinkedIn)
- ✅ Test navigation links
- ✅ Check responsive design (resize browser window)
- ✅ Verify all sections display correctly
- ✅ Check browser console for errors (F12 → Console tab)

### Step 3: If Everything Works, Deploy to GitHub

```bash
# Stop the local server (Ctrl + C)

# Check what files changed
git status

# Add all changes
git add .

# Commit with a descriptive message
git commit -m "Your descriptive commit message here"

# Push to GitHub
git push origin main
```

### Step 4: Verify Live Site
Wait 1-2 minutes for GitHub Pages to deploy, then visit:
https://tc-personal.github.io/timchowdary.github.io/

---

## 🐛 Debugging Tips

### Check JavaScript Console
1. Press `F12` or `Cmd + Option + I` to open Developer Tools
2. Go to **Console** tab
3. Look for error messages (red text)
4. Errors will help identify issues

### Common Issues & Solutions

**Issue: Buttons don't work**
- Check console for JavaScript errors
- Verify button IDs match in HTML and JS
- Make sure `script.js` is loading (check Network tab in DevTools)

**Issue: Styles not showing**
- Check console for CSS loading errors
- Verify `style.css` path is correct
- Try hard refresh: `Cmd + Shift + R` (Mac) or `Ctrl + F5` (Windows)

**Issue: Changes not visible**
- Clear browser cache
- Use incognito/private mode for testing
- Do a hard refresh

---

## 📱 Testing Responsive Design

### Test Different Screen Sizes

**In Chrome/Edge:**
1. Press `F12` to open DevTools
2. Click the device toggle icon (📱) or press `Cmd + Shift + M`
3. Select different devices from dropdown:
   - iPhone 12/13 Pro
   - iPad
   - Desktop (1920x1080)

**Or resize browser window manually**

---

## ✅ Pre-Deployment Checklist

Before pushing to GitHub, verify:

- [ ] All buttons work (Email, Mobile, GitHub, LinkedIn)
- [ ] Navigation links scroll smoothly
- [ ] No console errors (check F12 console)
- [ ] Layout looks good on desktop
- [ ] Layout looks good on mobile (responsive)
- [ ] All images load properly
- [ ] All external links work
- [ ] Text is readable and properly formatted

---

## 🔧 Advanced Testing

### Test in Multiple Browsers
- Chrome
- Safari
- Firefox
- Edge

### Test on Real Devices (if available)
- iPhone
- iPad
- Android phone/tablet

---

## 💡 Pro Tips

1. **Keep the server running** while editing - just refresh the browser to see changes
2. **Use incognito mode** for testing to avoid cache issues
3. **Check mobile view** before deploying (most visitors use mobile)
4. **Test all interactive elements** before pushing
5. **Read console messages** - they often explain what's wrong

---

## 🆘 Need Help?

If something doesn't work:
1. Check the browser console for errors (F12)
2. Verify file paths are correct
3. Make sure the local server is running
4. Try a different browser
5. Clear browser cache completely

---

## 📚 Additional Resources

- [MDN Web Docs](https://developer.mozilla.org/) - Web development documentation
- [Chrome DevTools Guide](https://developer.chrome.com/docs/devtools/) - Debugging guide
- [GitHub Pages Documentation](https://docs.github.com/en/pages) - Deployment guide

---

**Happy Testing! 🎉**

