# Archivo Font Setup Instructions

## Getting the Font Files

The GitHub repository at https://github.com/Omnibus-Type/Archivo is an excellent source for the Archivo font family.

### Option 1: Download Static Font Files (Recommended for specific weights)

1. Visit: https://github.com/Omnibus-Type/Archivo
2. Navigate to the `fonts` folder
3. Download the following files for Archivo SemiExpanded Bold:
   - `ArchivoSemiExpanded-Bold.woff2` (best format, smallest size)
   - `ArchivoSemiExpanded-Bold.woff` (fallback)
   - `ArchivoSemiExpanded-Bold.ttf` (fallback)

4. Place these files in the `fonts/` directory of this project

### Option 2: Use Variable Font (More flexible)

1. Download `Archivo-VariableFont_wdth,wght.woff2` from the fonts folder
2. Place it in the `fonts/` directory
3. The CSS will automatically use it with font-stretch and font-weight properties

### Quick Download Command

You can also use this command in your terminal (from the project root):

```bash
# Create fonts directory if it doesn't exist
mkdir -p fonts

# Download the SemiExpanded Bold font files
curl -L -o fonts/ArchivoSemiExpanded-Bold.woff2 "https://github.com/Omnibus-Type/Archivo/raw/master/fonts/static/ArchivoSemiExpanded-Bold.woff2"
curl -L -o fonts/ArchivoSemiExpanded-Bold.woff "https://github.com/Omnibus-Type/Archivo/raw/master/fonts/static/ArchivoSemiExpanded-Bold.woff"
curl -L -o fonts/ArchivoSemiExpanded-Bold.ttf "https://github.com/Omnibus-Type/Archivo/raw/master/fonts/static/ArchivoSemiExpanded-Bold.ttf"
```

Or download the variable font:

```bash
curl -L -o fonts/Archivo-VariableFont_wdth,wght.woff2 "https://github.com/Omnibus-Type/Archivo/raw/master/fonts/variable/Archivo-VariableFont_wdth,wght.woff2"
```

## Usage in CSS

After adding the font files, you can use:

- `font-family: 'Archivo SemiExpanded', 'Archivo', sans-serif;` for the SemiExpanded Bold variant
- `font-family: 'Archivo Variable', 'Archivo', sans-serif;` with `font-weight: 700; font-stretch: 75%;` for variable font

## License

Archivo is licensed under the SIL Open Font License 1.1, which allows free use for both personal and commercial projects.

