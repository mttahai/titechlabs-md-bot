<div align="center">

<img src="https://i.imgur.com/placeholder.png" width="150" height="150" style="border-radius:50%" alt="TiTech Bot Logo"/>

# TiTechLabs MD Bot

> A powerful, feature-rich WhatsApp MD bot with 90+ commands. AI integration, media tools, group management, and themed responses — built on Node.js and the Baileys library.

[![Stars](https://img.shields.io/github/stars/mttahai/titechlabs-md-bot?style=flat-square&color=yellow)](https://github.com/mttahai/titechlabs-md-bot/stargazers)
[![Forks](https://img.shields.io/github/forks/mttahai/titechlabs-md-bot?style=flat-square&color=blue)](https://github.com/mttahai/titechlabs-md-bot/network/members)
[![License](https://img.shields.io/github/license/mttahai/titechlabs-md-bot?style=flat-square&color=green)](LICENSE)
[![Node](https://img.shields.io/badge/Node.js-18%2B-brightgreen?style=flat-square)](https://nodejs.org)
[![Last Commit](https://img.shields.io/github/last-commit/mttahai/titechlabs-md-bot?style=flat-square)](https://github.com/mttahai/titechlabs-md-bot/commits)
[![Issues](https://img.shields.io/github/issues/mttahai/titechlabs-md-bot?style=flat-square&color=red)](https://github.com/mttahai/titechlabs-md-bot/issues)

</div>

---

## 🚀 Deploy TiTech Bot

### Before you deploy — Get your Session ID first

> [![Get Session ID](https://img.shields.io/badge/GET%20SESSION%20ID-Click%20Here-blueviolet?style=for-the-badge)](https://session.silvatechb.tech)

---

### Choose your hosting platform

| | Heroku | Railway | Koyeb |
|---|---|---|---|
| **Deploy** | [![Deploy to Heroku](https://img.shields.io/badge/Deploy-Heroku-430098?style=flat-square&logo=heroku)](https://heroku.com/deploy?template=https://github.com/mttahai/titechlabs-md-bot) | [![Deploy to Railway](https://img.shields.io/badge/Deploy-Railway-0B0D0E?style=flat-square&logo=railway)](https://railway.app/new/template?template=https://github.com/mttahai/titechlabs-md-bot) | [![Deploy to Koyeb](https://img.shields.io/badge/Deploy-Koyeb-121212?style=flat-square)](https://app.koyeb.com/deploy?type=git&repository=github.com/mttahai/titechlabs-md-bot) |
| **Speed** | ⚡ Recommended | ⚡ Fast | 🌐 Global edge |
| **Free?** | GitHub EDU Credits | $5 free/month | Always free tier |
| **24/7** | ✅ Yes | ✅ Yes | ✅ Yes |

> **Heroku** — Recommended · 24/7 uptime · Auto-restart on crash
>
> **Railway** — $5 free credits monthly · Fast cold-starts · Global edge
>
> **Koyeb** — Always-on free tier · Zero cold-starts · No config needed

---

## 🔑 How to Get a Session ID

You need a Session ID so the bot can connect to your WhatsApp account without scanning a QR code every time.

> 📱 **[Session ID Setup Guide →](https://session.silvatechb.tech)**

1. Open the session generator link above
2. Enter your WhatsApp number (with country code e.g. `923XXXXXXXXX`)
3. A pairing code will appear — enter it in WhatsApp → **Linked Devices → Link a Device → Link with phone number**
4. Copy the `SESSION_ID` shown on screen
5. Paste it in your platform's **Environment Variables** as `SESSION_ID`

> ⚠️ Keep your Session ID **private**. It gives full access to your WhatsApp account. Never share it publicly.

---

## ✨ Features

- 📥 **Media & Downloads** — YouTube, TikTok, Instagram, Facebook
- 🤖 **AI & Smart Tools** — AI chat, image generation
- 👥 **Group Management** — warn, ban, kick, mute, welcome, anti-spam
- 🛡️ **Protection Suite** — anti-fake, anti-link, anti-bad words
- 🎮 **Fun & Games** — stickers, polls, truth & dare
- 👑 **Owner Tools** — broadcast, sudo, settings panel

---

## ⚙️ Environment Variables

<details>
<summary>View all variables</summary>

| Variable | Description | Default |
|---|---|---|
| `SESSION_ID` | Your WhatsApp session ID | **Required** |
| `OWNER_NUMBER` | Your number e.g. `923XXXXXXXXX` | **Required** |
| `BOT_NAME` | Bot display name | `TiTech Bot` |
| `PREFIX` | Command prefix | `.` |
| `AUTO_STATUS_VIEW` | Auto view statuses | `true` |
| `AUTO_REACT_STATUS` | React to statuses | `true` |
| `ALWAYS_ONLINE` | Always show online | `false` |
| `REJECT_CALL` | Auto reject calls | `false` |
| `WARN_LIMIT` | Warns before kick | `3` |
| `TZ` | Timezone | `Asia/Karachi` |

</details>

---

## 🎨 Themes

Available themes — change with `.settheme` `.theme`:

`default` · `dark` · `light` · `minimal` · `neon`

---

## 📁 Project Structure

<details>
<summary>Expand file layout</summary>

```
titechlabs-md-bot/
├── silva.js          # WhatsApp connection, auto-status, event loop
├── handler.js        # Message routing, permissions, plugin dispatch
├── config.js         # All environment variables in one place
├── app.json          # Heroku deploy config + variable definitions
│
├── plugins/          # 90+ command plugins (one file per feature)
│   ├── menu.js       # Help menu
│   ├── settings.js   # Bot settings panel
│   ├── greet.js      # Daily auto-greeting
│   ├── warn.js       # Warning system (auto-kick at 3)
│   ├── sticker.js    # Sticker creator
│   ├── ai.js         # AI chat
│   ├── music.js      # YouTube audio
│   ├── tiktok.js     # TikTok downloader
│   ├── welcome.js    # Welcome / goodbye system
│   └── ...
```

</details>

---

## 📋 Full Command List

> All 90+ commands by category

<details>
<summary>🛡️ Group Management</summary>

`.kick` `.ban` `.unban` `.promote` `.demote` `.mute` `.unmute` `.warn` `.resetwarn` `.warnlist` `.tagall` `.hidetag` `.welcome` `.goodbye` `.setwelcome` `.setgoodbye` `.antilink` `.antifake` `.antispam`

</details>

<details>
<summary>📥 Downloaders</summary>

`.ytmp3` `.ytmp4` `.tiktok` `.instagram` `.facebook` `.twitter` `.pinterest` `.spotify`

</details>

<details>
<summary>🎨 Media Tools</summary>

`.sticker` `.toimg` `.crop` `.enhance` `.blur` `.sharpen` `.grayscale` `.mirror`

</details>

<details>
<summary>🤖 AI Tools</summary>

`.ai` `.gpt` `.imagine` `.describe` `.translate` `.tts` `.stt`

</details>

<details>
<summary>🎮 Fun & Games</summary>

`.dare` `.truth` `.wyr` `.poll` `.quiz` `.riddle` `.joke` `.meme`

</details>

<details>
<summary>👑 Owner Commands</summary>

`.broadcast` `.sudo` `.addsudo` `.delsudo` `.ban` `.unban` `.restart` `.shutdown` `.settings`

</details>

---

## 🛠️ Built With

[![Node.js](https://img.shields.io/badge/Node.js-18+-339933?style=flat-square&logo=node.js)](https://nodejs.org)
[![Baileys](https://img.shields.io/badge/Baileys-Latest-blueviolet?style=flat-square)](https://github.com/WhiskeySockets/Baileys)
[![Express](https://img.shields.io/badge/Express-4.x-000000?style=flat-square&logo=express)](https://expressjs.com)
[![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-47A248?style=flat-square&logo=mongodb)](https://mongodb.com)
[![Axios](https://img.shields.io/badge/Axios-1.x-5A29E4?style=flat-square)](https://axios-http.com)

---

## 🔗 Connect With TiTechLabs

[![Website](https://img.shields.io/badge/Website-titechlabs.dev-blue?style=flat-square)](https://titechlabs.dev)
[![GitHub](https://img.shields.io/badge/GitHub-mttahai-181717?style=flat-square&logo=github)](https://github.com/mttahai)
[![Portfolio](https://img.shields.io/badge/Portfolio-tahaislam.me-orange?style=flat-square)](https://tahaislam.me)
[![Fiverr](https://img.shields.io/badge/Fiverr-Hire%20Me-1DBF73?style=flat-square&logo=fiverr)](https://fiverr.com)

---

## 👥 Contributors

<a href="https://github.com/mttahai/titechlabs-md-bot/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=mttahai/titechlabs-md-bot" />
</a>

---

## 🌐 Community

> [![WhatsApp Group](https://img.shields.io/badge/Join-WhatsApp%20Group-25D366?style=for-the-badge&logo=whatsapp)](https://wa.me/923XXXXXXXXX)

---

## 📄 License

MIT License — free to use, modify, and distribute with attribution.

> TiTechLabs MD Bot — 90+ commands · Built with ❤️ by [Muhammad Taha Islam](https://tahaislam.me)
>
> *Based on [Silva MD Bot](https://github.com/SilvaTechB/silva-md-bot) — MIT License*

---

<div align="center">

**⭐ Star this repo if you found it useful!**

*TiTechLabs · Pakistan 🇵🇰*

</div>
