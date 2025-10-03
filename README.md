# ClanSplit RuneLite Plugin

Official RuneLite plugin for ClanSplit - automatically sends your PvP Loot Keys to shared clan sessions.

## Build

```bash
./gradlew clean build
```

The JAR will be in `build/libs/clansplit-rl-plugin-0.1.0.jar`.

## Install

### External Plugin (Manual)
1. Open RuneLite → Plugins → External Plugins → Add plugin
2. Select the built JAR
3. Enable the plugin

### Plugin Hub (Coming Soon)
The plugin will be available on the RuneLite Plugin Hub.

## Configure

1. **Enable**: Toggle the plugin on/off
2. **Session ID**: Paste your session ID from the ClanSplit webapp
3. **Plugin Token**: Generate from My Account → RuneLite Plugin → Generate/Rotate

## Features

- Automatically links your OSRS name to your ClanSplit session
- Detects when you open PvP Loot Keys
- Sends loot values to your active ClanSplit session in real-time
- Works with clan broadcast messages
- Secure token-based authentication

## How It Works

1. When you log in, the plugin links your OSRS character name to your ClanSplit session
2. When you open a PvP Loot Key, the plugin detects the value from chat messages
3. The key value is automatically posted to your session with a unique nonce to prevent duplicates

## Privacy & Security

- Only sends data when you explicitly configure Session ID and Token
- Only tracks YOUR OWN loot keys - never other players' keys
- All data is sent over HTTPS
- Tokens can be rotated at any time from your account settings

## Support

Visit [app.clansplit.com](https://app.clansplit.com) for support and documentation.

## License

Proprietary - © 2025 ClanSplit

