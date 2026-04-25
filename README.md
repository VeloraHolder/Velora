# Velora

Velora is a Windows optimization and gaming tweak utility focused on performance, cleanup, diagnostics, restore workflows, and profile-based system tuning.

## Download

Official download page:

https://getvelora.netlify.app

Latest installer:

https://www.dropbox.com/scl/fi/i7dse40zkrc4mnf0or3cm/Velora-Installer-2.4.0.exe?rlkey=p39vo4u3ris4za2jfpbpki1ab&st=7sv300jh&dl=1

Community and support:

https://discord.gg/FjB27cjSPp

## Project Structure

```txt
site/             Public download website
src/              React app source
electron/         Electron main/preload code
installer-app/    Installer UI app
build/            Installer resources
scripts/          Build and release scripts
public/           Static app assets
```

## Local Development

Install dependencies:

```bash
npm install
```

Run the Electron development app:

```bash
npm run dev
```

Build the web renderer:

```bash
npm run build
```

Build the Windows installer:

```bash
npm run build:win
```

## Website

The public website lives in `site/`.

For GitHub Pages, the included workflow publishes the `site` folder automatically when changes are pushed to `main`.

If you use GitHub Pages, set the repository Pages source to:

```txt
GitHub Actions
```

## Release Notes

Current version:

```txt
2.4.0
```

Recommended release flow:

```bash
npm run build:win
```

Then upload the generated installer to your release host and update:

```txt
site/index.html
site/updates/latest.json
README.md
```

## Safety

Velora changes Windows settings only when users choose actions inside the app. Keep restore and review flows visible for any system-level optimization feature.

## License

Copyright Velora Team. All rights reserved unless a separate license is added.
