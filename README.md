# Servermutescheduler
A Vencord plugin that automatically mutes all your Discord servers outside your active hours and sets them to @mentions only during active hours. Features a toggle slider in the server list and the ability to exclude specific servers from being affected.

# ServerMuteScheduler

A Vencord plugin that automatically mutes all your Discord servers outside your active hours and sets them to @mentions only during active hours. Features a toggle slider in the server list and the ability to exclude specific servers from being affected.

---

## 📋 Requirements

- **Node.js** → [nodejs.org](https://nodejs.org) (pick LTS version)
- **Git** → [git-scm.com](https://git-scm.com)

---

## 🔧 Step 1 — Install Vencord from source

Open CMD and run these commands one by one:
```bash
git clone https://github.com/Vendicated/Vencord
cd Vencord
pnpm install --frozen-lockfile
pnpm run build
pnpm run inject
```

When `pnpm run inject` asks for your Discord location, enter:
C:\Users\YOURNAME\AppData\Local\Discord
Then fully restart Discord.

---

## 📁 Step 2 — Install the plugin

1. Download `ServerMuteScheduler.tsx` from this page
2. Go to this folder on your PC:
C:\Users\YOURNAME\Vencord\src\userplugins
3. If the `userplugins` folder doesn't exist, create it
4. Drop `ServerMuteScheduler.tsx` inside it

---

## ⚙️ Step 3 — Build and launch

Run in CMD:
```bash
cd C:\Users\YOURNAME\Vencord
pnpm run build
```
Then open Discord → **Settings → Vencord → Settings** → click **Relaunch Discord**

---

## ✅ Step 4 — Enable the plugin

1. Go to **Settings → Plugins**
2. Search **ServerMuteScheduler**
3. Toggle it **on**
4. Click the ⚙️ icon to configure your active hours and excluded servers

---

## 🕐 Step 5 — Configure

| Setting | Description |
|---|---|
| Active Start | UTC hour when servers unmute (default: 16) |
| Active End | UTC hour when servers mute (default: 0) |
| Excluded Servers | Comma separated server IDs to never touch |

To get a server ID: enable **Developer Mode** in Discord (Settings → Advanced → Developer Mode) then right-click a server icon → **Copy Server ID**

---

## 🎚️ Usage

A green/red slider will appear at the top of your server list:

- 🟢 **ON** → scheduler is running
- 🔴 **OFF** → scheduler is paused

Click it anytime to pause or resume without going into settings.

---

> ⚠️ Replace `YOURNAME` with your actual Windows username in all folder paths above.
>
> ⚠️ This plugin is PC only. Vencord does not work on mobile.
