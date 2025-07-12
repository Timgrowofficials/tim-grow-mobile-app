# Tim Grow Mobile App - Quick Commands

## Git Commands (Local PC)

### Initial Setup:
```bash
git init
git add .
git commit -m "Initial commit: Tim Grow mobile app"
git remote add origin https://github.com/YOUR_USERNAME/tim-grow-mobile-app.git
git push -u origin main
```

### Daily Development:
```bash
# Check what changed
git status

# Add changes
git add .

# Commit changes
git commit -m "Updated booking features"

# Push to GitHub (triggers APK build)
git push origin main
```

## Development Commands

### Start Development Server:
```bash
npm install
npm run dev
```

### Build for Production:
```bash
npm run build
```

### Mobile Development:
```bash
# Sync with Capacitor
npx cap sync android

# Open in Android Studio
npx cap open android

# Build APK locally
npx cap run android
```

## Codemagic Build

### Automatic Process:
1. **Push code** to GitHub
2. **Codemagic detects** changes
3. **Builds APK** automatically
4. **Download** from artifacts

### Build Time: 6-10 minutes

## File Structure

```
├── android/          # Native Android config
├── client/           # React frontend
├── server/           # Express backend
├── shared/           # TypeScript schemas
├── codemagic.yaml    # Build configuration
└── package.json      # Dependencies
```

Ready to develop your Tim Grow mobile app!