# Media Queries - notatki

## Skladnia

```css
@media not|only mediatype and (media-feature: value) {
    /* CSS */
}
```

W HTML:

```html
<link rel="stylesheet" media="mediatype and|not|only (media-feature)" href="styles.css" />
```

Alternatywa (OR) w regule to przecinek `,`:

```css
@media (max-width: 900px), (min-resolution: 192dpi), (min-device-pixel-ratio: 2) {
    /* CSS */
}
```

## Lista `mediatype`

- `all` (domyslne)
- `print`
- `screen`
- `speech`

## Najczęściej używane `media feature`

- `width`, `height`
- powyższe z dodatkowymi prefiksami: `min-`, `max-`
- `aspect-ratio`, `device-aspect-ratio` (np. `16/9`, `4/3`, `2`)
- `orientation`
- `resolution` (jednostki: `dpi`, `dpcm`, `dppx`)

## Możliwe architektury

1. Mobile first
2. Ostre limity przedziałów vs kaskada oparta o `max-width`.
3. Przykładowe breakpointy graniczne: `480`, `600`, `760`, `980`, `1200`.

## Debug

- Chrome DevTools.
