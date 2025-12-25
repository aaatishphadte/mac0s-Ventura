# Custom Fonts Folder

Place your custom font files here.

## Supported Formats
- `.ttf` (TrueType Font)
- `.otf` (OpenType Font)
- `.woff` (Web Open Font Format)
- `.woff2` (Web Open Font Format 2 - Recommended for best performance)

## How to Add Your Fonts

1. **Copy your font files** to this folder
   - Example: `MyFont-Regular.ttf`, `MyFont-Bold.ttf`

2. **Update** `/src/css/fonts.css` with your font names and file paths:
   ```css
   @font-face {
     font-family: 'MyCustomFont';
     src: url('/fonts/MyFont-Regular.ttf') format('truetype');
     font-weight: 400;
     font-style: normal;
     font-display: swap;
   }
   ```

3. **Use your fonts** in CSS:
   ```css
   body {
     font-family: 'MyCustomFont', sans-serif;
   }
   ```

## Tips
- Use `.woff2` format for best performance
- Include fallback fonts in your font-family declarations
- Use `font-display: swap` to prevent invisible text during loading
