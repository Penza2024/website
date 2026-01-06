# Node.js Installation Guide for macOS

The Node.js installer has been downloaded to `/tmp/node-installer.pkg`

## Option 1: Double-click Installation (Easiest)

1. Open Finder
2. Press `Cmd + Shift + G` to open "Go to Folder"
3. Type: `/tmp`
4. Find and double-click `node-installer.pkg`
5. Follow the installation wizard
6. Enter your password when prompted

## Option 2: Command Line Installation

Run this command in your terminal:
```bash
sudo installer -pkg /tmp/node-installer.pkg -target /
```

You'll be prompted for your password.

## After Installation

Once installed, close and reopen your terminal, then verify the installation:

```bash
node --version
npm --version
```

You should see version numbers like:
- Node: v20.11.0
- npm: 10.x.x

## Next Steps

After Node.js is installed, we'll:
1. Install Wrangler CLI: `npm install -g wrangler`
2. Login to Cloudflare: `wrangler login`
3. Deploy your website: `wrangler pages deploy . --project-name=mapalo-portfolio`

---

Let me know once Node.js is installed and I'll help you with the deployment!
