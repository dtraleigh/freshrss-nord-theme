# Nord Compact

A FreshRSS theme based on Nord's color scheme, with a tidier mobile layout.

Nord Compact is a fork of the [Nord theme](https://github.com/FreshRSS/FreshRSS/tree/1.30.0/p/themes/Nord)
bundled with FreshRSS 1.30.0, originally created by [joelchrono12](https://github.com/joelchrono12/freshrss-nord-theme).
It installs alongside the bundled Nord, so you can switch between them in FreshRSS' display options.

![Example](./thumbs/original.png)

## Changes from Nord

On narrow screens (840px and below):
- The navigation toolbar is centered, with even spacing between button groups.
- Category boxes in the global view are evenly inset from both screen edges.

On all screen sizes:
- The article subtitle line (feed, author, date) wraps instead of overflowing horizontally,
  and the date stays on one line when there's room.
- The reading view card has less empty space at the top and a small gap at its sides.

## Installation

Clone the repository into your FreshRSS theme directory as `NordCompact`.
Where that is depends on where you installed FreshRSS, but it's usually in:
```shell
FRESHRSS_INSTALL_DIR="/var/www/freshrss"
```

```shell
cd "$FRESHRSS_INSTALL_DIR/p/themes"
git clone https://github.com/dtraleigh/freshrss-nord-theme.git NordCompact
```
Clear your browser's cache, then select **Nord Compact** in FreshRSS' display options.

To update later, run `git pull` inside the `NordCompact` folder.

## Compatibility

Built against FreshRSS 1.30.0. The theme relies on FreshRSS' base stylesheet (`_frss.css`),
which changes between releases, so check the theme after upgrading FreshRSS.
If something looks off, compare it with the bundled Nord theme.
