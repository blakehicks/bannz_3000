# bannz_3000

## HTML Banner Package for the Yeare of Oure Lourde Three Thousande

_Dap to [@crigger](https://github.com/crigger) for the OG package this is based on._

---

## Installation

- Open Terminal, `cd` to desired location, then `git clone https://github.com/blakehicks/bannz_3000.git` to grab repo.
- Switch to directory with `cd bannz_3000` (feel free to change name first to be more descriptive if desired).
- `npm install` or `yarn install` to get dependencies.
- `npm link` or `yarn link` to set up commands (temp fix, not ideal right yet—may screw up client names).

## Commands

### bannz setup

**Perform initial setup.**

- Set client name.
- Choose animation library ([GSAP](https://greensock.com/docs/v3) or [Anime.js](https://animejs.com/documentation/)) and insert CDN link into template HTML.
- Initialize your first ad creative based on whatever size you feel like starting with.

### bannz watch

**Choose creative to watch for changes and show in browser.**

- Lists all existing ad creatives in `src/banners/` that are properly denoted with size names.
- Loads chosen creative in default browser tab at `localhost:3000`.
- Monitors for changes in directory and reloads tab via [Browsersync](https://browsersync.io/).
- Minifies CSS from `src/banners/<creative>/assets/css/source.css` to `style.css` in same folder.
- Minifies JS from `src/banners/<creative>/assets/js/main.js` to `main.min.js` in same folder.
- Add arg `--folder <creative name here>` to skip selection process and target specific ad.
- Use `CTRL + C` to stop process.

### bannz deploy

**Zip up vendor-ready files in `src/banners/` and output to `/dist` for sending along to vendor.**

- Grabs only minified and otherwise necessary files before zip to cut file size down as much as possible.

### bannz help

**See most of the above information in your terminal.**
