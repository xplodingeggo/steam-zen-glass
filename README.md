# Zen Glass for Steam

A frosted glass theme for the Steam client, based on the transparent look of [Zen Browser](https://zen-browser.app). Steam's backgrounds are cleared so the Windows 11 acrylic blur shows through, with a dark navy tint on top.

## What you need

- Windows 11 with **Transparency effects** turned on (Settings → Personalization → Colors)
- [Millennium](https://steambrew.app)
- The [Window Styler (DWMX)](https://steambrew.app/plugin/b4c58634419b) plugin. It provides the actual blur. Without it the theme just looks dark.

If DWMX doesn't blur anything on your setup (common on 64-bit Millennium), see [ejalxndr/dwmx#18](https://github.com/ejalxndr/dwmx/pull/18) for a fix.

## Install

1. Download or clone this repo into `Steam\millennium\themes\zen-glass`
2. In Steam, open Millennium → Themes and pick **Zen Glass**
3. Make sure DWMX is enabled under Millennium → Plugins

## Tweaking

Colors are CSS variables at the top of each file:

- `css/glass.css`: the Steam client (library, game pages, downloads, menus, dialogs, friends)
- `css/webkit.css`: the store and community pages

The main one is `--zg-tint`. Raise its last number to make the window darker, or lower it to see more of what's behind.

## Known issues

- Steam's class names change with updates, so a panel might turn solid again after a Steam update. Open an issue with a screenshot and I'll take a look.
- Only covers the desktop client. Big Picture isn't themed.

## License

[MIT](LICENSE). Use it, change it, and share your own versions, just keep the credit.
