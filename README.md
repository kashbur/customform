# Big Reveal Generator

This repository contains the HTML form used to create custom URL links for the Big Reveal page hosted at **https://bigreveal.joyjotstudio.store/**. The generator lets you choose fonts and colors, then produces a shareable link with all of the settings encoded as query parameters.

## Using the form

1. Open `index.html` in your browser.
2. Enter the access code from your purchase PDF to unlock the form.
3. Fill out each section:
   - **Background Theme** – pick one of the preset colors or choose a custom hex value.
   - **Text Color** – sets the color of all text.
   - **Text Outline Color** – optional outline around each letter.
   - **Default Font** – base font used when per‑line fonts are not specified.
   - **Main Headline** – first line on page 1. Displayed in ALL CAPS by default.
   - **Message 1** – first line on page 2. Also uppercased by default.
   - **Message 2** – optional second line on page 2.
   - **Photo URL** – optional image shown on page 2.
   - **Ending Message** – optional closing line on page 2.
   - **Per‑line Fonts** – use the dropdowns to pick a specific font for the main headline, message 1, message 2, and ending message.
4. Click **Generate My Reveal URL**. A shareable link will appear. Copy this link or preview the page.

## URL parameters

The generated link encodes all options as query parameters. Any of these can be adjusted manually:

- `color` – background theme or `#RRGGBB` hex color.
- `textColor` – main text color.
- `outlineColor` – color of the optional text outline (`transparent` for none).
- `font` – default font family.
- `fontMain` – font for the main headline.
- `fontSub` – font for message 1.
- `fontDate` – font for message 2.
- `fontFrom` – font for the ending message.
- `main` – main headline text.
- `sub` – message 1 text.
- `date` – message 2 text.
- `photo` – URL to an image displayed on page 2.
- `from` – ending message text.
- `mainCaps` – set to `0` to disable automatic uppercasing of the main headline.
- `subCaps` – set to `0` to disable uppercasing of message 1.

### Defaults

If a parameter is omitted the reveal page falls back to sensible defaults:

- Background defaults to beige (`#f3ddbb`).
- Text defaults to black with no outline.
- The chosen default font is used for all lines if a per‑line font is not provided.
- The main headline and message 1 are converted to uppercase unless `mainCaps=0` or `subCaps=0` are supplied.

## Example

```
https://bigreveal.joyjotstudio.store/?main=WE%27RE%20EXPECTING&sub=Baby%20Smith&date=Arriving%20Feb%202024&from=Love%20The%20Smiths&color=pink&textColor=%232563eb&outlineColor=%23ffffff&font=Poppins&fontMain=Playfair%20Display&fontSub=Dancing%20Script&fontDate=Montserrat&fontFrom=Sacramento
```

Opening the above URL will render the reveal page with a pink background, blue text, white outline, and individual fonts for each line.

