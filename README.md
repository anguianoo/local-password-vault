🗝️ Local Password Vault

A lightweight, local-first password manager built with Electron.js.
All passwords are encrypted and stored on your machine only — no cloud, no external servers.

🚀 Features (Planned)

Master password to unlock the vault

AES-encrypted password storage

Save, view, and manage credentials

Clipboard auto-clear (optional)

Cross-platform: Windows, macOS, Linux

⚡ Getting Started

Clone the repo (or create project folder):
git clone https://github.com/yourusername/local-password-vault.git
cd local-password-vault

Install dependencies:
npm install

Run the app:
npm start

📦 Packaging the App

When you’re ready to distribute your app:

npm install electron-builder --save-dev
npx electron-builder


This generates .exe (Windows), .dmg (macOS), or .AppImage (Linux) installers in the dist/ folder.

🔐 Security Notes

Never hardcode your master password.
Use strong encryption (crypto module recommended).
Clear clipboard after use.
Consider locking the app after inactivity.

📚 Resources

Electron.js Docs
Node.js File System
Node.js Crypto

📂 Project Structure

local-password-vault/
│
├── package.json          # Project config (dependencies, scripts)
├── main.js               # Electron main process (creates the window)
├── index.html            # UI layout (inputs, buttons, display area)
│
├── src/                  # App logic and assets
│   ├── renderer.js       # Renderer process (handles UI events)
│   ├── crypto.js         # Encryption/decryption helpers
│   ├── storage.js        # File handling (read/write vault data)
│   └── styles.css        # CSS for UI styling
│
├── vault/                # Local data storage
│   └── vault.json        # Encrypted passwords saved here
│
└── assets/               # Icons, images (optional)
    └── icon.png

