# Nuqta Site Block - Chrome Extension

A beautiful, modern, and smart website blocking Chrome Extension designed to help you stay focused and distraction-free.

🔗 **Chrome Web Store:**  
https://chromewebstore.google.com/detail/nuqta-site-blocker/lngcogdoddheoaakfgcaadbgjhgflhcj
📄 **Privacy Policy:**  
See `PRIVACY.md` for full details about data handling and privacy.
## 🎨 Features

### ✨ Modern Design
- Beautiful gradient UI with smooth animations
- Clean, minimalist interface
- Dark mode support
- Responsive and user-friendly

### 🚀 Smart Features
- **Quick Site Blocking**: Add sites directly from the popup
- **Block Current Site**: Instantly block the website you're viewing
- **Focus Sessions**: 25/50/90 minute presets + custom duration
- **Keyword Blocking**: Automatically blur pages with blocked keywords
- **Password Protection**: Secure your settings with a password
- **Live Timer**: Real-time countdown during focus sessions

### 🔒 Security
- SHA-256 password hashing
- Settings locked during focus mode
- Cannot bypass blocking during active sessions

## 📦 Installation

### Step 1: Prepare Icons
You'll need icon files in the `icons/` folder:
- `icon16.png` (16x16 pixels)
- `icon48.png` (48x48 pixels)
- `icon128.png` (128x128 pixels)

You can use placeholder images or create custom icons.

### Step 2: Load Extension
1. Open Chrome and go to `chrome://extensions/`
2. Enable **Developer mode** (toggle in top-right)
3. Click **Load unpacked**
4. Select the folder containing all extension files
5. Pin the extension to your toolbar for easy access

## 🎯 How to Use

### Adding Sites to Block

**Method 1: Quick Add (Fastest)**
1. Click the Nuqta icon
2. Type any website in the input field (e.g., `facebook.com`, `twitter.com`, `instagram.com`, `reddit.com`)
3. Click **+** or press Enter

**Method 2: Block Current Site**
1. Visit any website
2. Click Nuqta icon
3. Click **🚫 Block Current Site**

**Method 3: Settings Page**
1. Click **Settings** in popup
2. Enter password
3. Add sites in "Blocked Websites" section

### Starting a Focus Session
1. Click the Nuqta icon
2. Choose duration: **25m**, **50m**, **90m**, or enter custom minutes
3. Click **Start Focus**
4. All blocked sites are now inaccessible!

### Managing Settings
1. Click **Settings** button
2. Enter your password (or set one on first use)
3. Manage blocked sites, keywords, and password

## 🎨 Design Highlights

- **Poppins Font**: Modern, clean typography
- **Gradient Themes**: Beautiful purple/blue gradients
- **Smooth Animations**: Subtle transitions throughout
- **Glass-morphism**: Modern UI effects
- **Responsive**: Works on all screen sizes

## 🛠️ Technical Details

- **Manifest V3** compliant
- **Service Worker** for background tasks
- **Declarative Net Request** for fast blocking
- **Chrome Alarms API** for reliable timers
- **Chrome Storage Sync** for data persistence

## 📝 Files Structure

```
Nuqta Site Block/
├── manifest.json       # Extension configuration
├── background.js       # Service worker
├── popup.html/css/js   # Main popup interface
├── options.html/css/js # Settings page
├── blocked.html/css/js # Blocked page UI
├── content.js          # Keyword blocking script
└── icons/              # Extension icons
```

## 🔧 Features Explained

### Focus Mode
- Blocks all listed websites automatically
- Prevents settings changes during session
- Shows live countdown timer
- Auto-unlocks when timer ends

### Keyword Blocking
- Scans page content for blocked keywords
- Blurs entire page if keyword found
- Shows warning message with timer
- Optimized for performance

### Password Protection
- All settings locked behind password
- SHA-256 hashed (never stored in plaintext)
- Cannot disable during focus mode

## 💡 Tips

- Start with short focus sessions (25 min)
- Use "Block Current Site" for quick additions
- Set a strong password for settings
- Review blocked sites regularly

## 🐛 Troubleshooting

**Sites not blocking?**
- Make sure focus mode is active
- Check if domain is correct (e.g., `youtube.com` not `www.youtube.com`)

**Can't access settings?**
- End your focus session first
- Settings are locked during active focus

**Timer not updating?**
- Refresh the popup
- Check if focus mode is still active

## 📄 License

This extension is provided as-is for personal and educational use.

---

**Built with ❤️ for productivity and focus**
