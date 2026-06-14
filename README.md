# Mustang - Standard Notes theme

A dark warm-gray Standard Notes theme ported from the Mustang color scheme,
originally created for Vim by Henrique C. Alves and later ported to Emacs.

## Color palette

| Role | Color | Hex |
|---|---|---|
| Background | Dark warm gray | `#202020` |
| Panels / sidebars | Slightly lighter gray | `#232323` |
| Primary text | Warm light gray | `#e2e2e5` |
| Secondary text | Muted gray | `#808080` |
| Accent / highlights | Orange | `#ff9800` |
| Success | Green | `#b1d631` |
| Warning | Gold | `#df9f2d` |
| Danger | Red | `#f34a4a` |
| Borders | Dark gray | `#303030` |
| Selection bg | Warm gray-blue | `#3c414c` |
| Selection fg | Light cream | `#faf4c6` |

## Installation

1. Open Standard Notes and go to **Preferences -> Plugins -> Install Custom Plugin**.
2. Paste the raw CSS URL and confirm:

```
https://cdn.jsdelivr.net/gh/netromdk/sn-theme-mustang@master/ext.json
```

After publishing a new release, purge the jsDelivr cache so the update checker
picks up the latest `ext.json`:

- https://purge.jsdelivr.net/gh/netromdk/sn-theme-mustang@master/ext.json

(The CSS is served from an immutable version tag and does not need purging.)

## Building from source

The source lives in `src/main.scss`. Compile it to `dist/dist.css` with:

```sh
./build.sh
```

The script requires `npm` (Node.js). On first run it installs `sass` locally into `node_modules/`
(no global install needed). Subsequent runs skip the install step.

To run the build step directly after `npm install`:

```sh
npm run build
```
