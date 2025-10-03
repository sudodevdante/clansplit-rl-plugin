# ClanSplit RuneLite Plugin

**Automatically track and split PvP loot with your clan in real-time.**

ClanSplit is a web-based loot splitting tool designed for Old School RuneScape PvP clans. This official RuneLite plugin automatically detects when you open PvP Loot Keys and sends the values to your active ClanSplit session, making loot distribution fast, fair, and transparent.

---

## 🎯 What is ClanSplit?

ClanSplit ([app.clansplit.com](https://app.clansplit.com)) is a web application that helps PvP clans:
- **Track loot** from all clan members in real-time
- **Calculate fair splits** with configurable key reduction and clan tax
- **Manage sessions** with session leaders and late joiners
- **Checkout seamlessly** with automatic profit/debt calculations

The RuneLite plugin eliminates manual entry by automatically sending your loot key values to your session.

---

## ✨ Features

- **Automatic Detection**: Detects when you open PvP Loot Keys in-game
- **Instant Sync**: Sends loot values to your ClanSplit session in real-time
- **Secure**: Uses token-based authentication - only you can add keys to your session
- **Lightweight**: No overlay clutter, just three simple config options
- **Privacy-First**: Only tracks YOUR loot keys, never other players' keys
- **Works with Clan Chat**: Detects both direct messages and clan broadcast messages

---

## 📦 Installation

### Option 1: RuneLite Plugin Hub (Recommended)
1. Open RuneLite
2. Click the **Plugin Hub** button (puzzle piece icon)
3. Search for **"ClanSplit"**
4. Click **Install**

### Option 2: Manual Installation
1. Download the latest `.jar` from [Releases](https://github.com/sudodevdante/clansplit-rl-plugin/releases)
2. In RuneLite, go to **Configuration** → **Plugin Hub** → **Add External Plugin**
3. Select the downloaded `.jar` file
4. Enable the plugin

---

## ⚙️ Setup & Configuration

### 1. Create a ClanSplit Account
1. Visit [app.clansplit.com](https://app.clansplit.com)
2. Create an account or sign in
3. Go to **Account** → **RuneLite Plugin Settings**

### 2. Generate Your Plugin Token
1. Click **Generate Token** (or **Rotate Token** if you already have one)
2. Copy the token - you'll need it for the plugin configuration

### 3. Start or Join a Session
1. Go to the **Home** page
2. Either:
   - Click **Start New Session** to create a session
   - Join an existing session using a Session ID

### 4. Configure the RuneLite Plugin
1. In RuneLite, open **Configuration** (wrench icon)
2. Search for **"ClanSplit"** in the sidebar
3. Configure the following settings:

| Setting | Description |
|---------|-------------|
| **Enable** | Toggle the plugin on/off |
| **Session ID** | Paste your active session ID from the webapp |
| **Token** | Paste your plugin token from your account settings |

### 5. You're Ready!
Once configured:
- The plugin will automatically link your OSRS character to the session when you log in
- Every time you open a PvP Loot Key, it's automatically added to your session
- Check the webapp to see your loot, splits, and final checkout amounts in real-time

---

## 🔧 How It Works

### Loot Detection
The plugin listens for specific chat messages that indicate you've opened a loot key:

**Clan Broadcast Messages:**
```
[Clan] YourName has opened a loot key worth 187,036 coins!
```

**Direct Game Messages:**
```
You receive a PvP loot key worth 187,036 coins.
You open a loot key worth 187,036 coins.
```

### Data Sent to ClanSplit
When a loot key is detected, the plugin sends:
- **Your OSRS character name**
- **Loot key value** (in coins)
- **Session ID** (to know which session to update)
- **Unique nonce** (prevents duplicate entries)
- **Timestamp** (for accurate tracking)

### Security
- All data is sent over **HTTPS** (encrypted)
- **Token authentication** ensures only you can add keys to your session
- Tokens can be **rotated at any time** from your account settings
- The plugin **never** tracks other players' loot keys

---

## 🔒 Privacy & Security

### What the Plugin Tracks
✅ **YOUR loot keys only** - detected from your own chat messages  
✅ **Your OSRS character name** - to link you to your session  
✅ **Your session ID** - to know where to send the data

### What the Plugin Does NOT Track
❌ Other players' loot keys  
❌ Your inventory or bank  
❌ Your location or activities  
❌ Any personal information

### Data Usage
- Data is only sent when **you explicitly configure** the Session ID and Token
- You can **disable the plugin** at any time
- You can **rotate your token** if it's compromised
- You can **delete your account** and all associated data from the webapp

---

## 🛠️ Troubleshooting

### Plugin Not Sending Keys
1. **Check the configuration**: Ensure Enable is ON, Session ID and Token are correctly entered
2. **Verify the session**: Make sure the session is still active on the webapp
3. **Check your token**: Try rotating your token and updating it in the plugin config
4. **Restart the plugin**: Toggle it off and on in the config

### Keys Not Appearing in Webapp
1. **Hard refresh the webapp**: Press `Ctrl+Shift+R` (or `Cmd+Shift+R` on Mac)
2. **Check the session ID**: Make sure you're viewing the correct session
3. **Verify SSE connection**: The webapp uses Server-Sent Events for real-time updates

### Token Issues
- If you've rotated your token, update it in the plugin configuration immediately
- Old tokens are invalidated when you generate a new one
- Keep your token private - don't share it with anyone

---

## 📊 ClanSplit Web Features

The webapp provides:
- **Real-time session dashboard** with all member stats
- **Automatic split calculations** based on configurable settings
- **Late joiner support** with auto-join functionality
- **Session leader controls** for managing members and settings
- **Checkout tracking** to see who owes what
- **Session history** to review past sessions

---

## 🆘 Support

### Need Help?
- **Documentation**: [app.clansplit.com/how-it-works](https://app.clansplit.com/how-it-works)
- **GitHub Issues**: [github.com/sudodevdante/clansplit-rl-plugin/issues](https://github.com/sudodevdante/clansplit-rl-plugin/issues)
- **Contact**: Visit [app.clansplit.com](https://app.clansplit.com) for support

### Found a Bug?
Please report it on our [GitHub Issues](https://github.com/sudodevdante/clansplit-rl-plugin/issues) page with:
- Steps to reproduce
- Expected behavior
- Actual behavior
- Screenshots (if applicable)

---

## 📝 License

Proprietary - © 2025 ClanSplit

This plugin is the official companion to the ClanSplit web application. Use of this plugin is subject to the ClanSplit Terms of Service.

---

## 🚀 Version History

### v0.1.0 (Initial Release)
- Automatic PvP Loot Key detection
- Real-time sync with ClanSplit sessions
- Clan broadcast message support
- Secure token-based authentication
- Simple 3-option configuration

---

**Made with ⚔️ for the OSRS PvP community**

[Website](https://app.clansplit.com) • [GitHub](https://github.com/sudodevdante/clansplit-rl-plugin) • [Plugin Hub](https://runelite.net/plugin-hub)
