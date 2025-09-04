# 🗝️ Local Password Vault

A lightweight, local-first password manager built with Electron.js.
All passwords are encrypted and stored on your machine only — no cloud, no external servers.

# 🚀 Features (Planned)

- Master password to unlock the vault

- AES-encrypted password storage

- Save, view, and manage credentials

- Clipboard auto-clear (optional)

- Cross-platform: Windows, macOS, Linux

# ⚡ Getting Started

Clone the repo (or create project folder):
```
git clone https://github.com/yourusername/local-password-vault.git
cd local-password-vault
```

Install dependencies:
```
npm install
```

Run the app:
```
npm start
```
# 📦 Packaging the App

When you’re ready to distribute your app:
```
npm install electron-builder --save-dev
npx electron-builder
```

This generates .exe (Windows), .dmg (macOS), or .AppImage (Linux) installers in the dist/ folder.

# 🔐 Security Notes

- Never hardcode your master password.

- Use strong encryption (crypto module recommended).

- Clear clipboard after use.

- Consider locking the app after inactivity.

📚 Resources

- [Electron.js Docs](https://www.electronjs.org/docs/latest/)

- [Node.js File System](https://nodejs.org/api/documentation.html)
