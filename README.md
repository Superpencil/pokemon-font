# pokemon-font v1.8.2

This font is an extended clone of the original font shipped with Pokemon R/G/B/Y for the GAME BOY in the 90's. It was made into a proper, modern, Unicode font and was extended with more language support and ligatures because it was needed for Pokemon-Mini.

_Install_ `npm install pokemon-font`

## Donate

- BTC ₿ 32xrhaLRJ7DWgAc5umnkVqa5PFqcDhUisK
- ETH Ξ 0x132F77Ab366A30614cD08405aC5F10F260525332

## Usage

This is a 'pixel' font, but modern font formats are actually vector based, so the font uses vector calculations to create little squares. This brings all the same issues as old-fashioned pixel fonts in terms of rendering it properly.

The font is 10px high, so to properly render it you'll need to use increments of 10px

You'll also need to turn off anti-aliasing for fonts if the browser supports it to avoid blurry fonts.

Displaying the font in flexbox layouts will make it blurry too.

### CSS example

```css
body {
  font-size: 10px;
  font-smooth: never;
  -webkit-font-smoothing: none;
  font-family: "pokemon-font", monospace;
}
h1 {
  font-size: 40px;
}
```

## Latin

The latin character set has been extended to support the first three Unicode blocks, Basic Latin, Latin-1 Supplement and Latin Extended-A. This covers most West European languages. Some of the original glyphs have been changed for harmony with the added new glyphs.

For all my nerdy trainers out there, these characters are extended as well to support common programming languages. So go ahead and load this up in your favorite editor.

![Alt text](/img/Latin.png?raw=true "pokemon-font Latin Glyphs")

## Unown

To type Unown, you must use one of the formats that supports ligatures. These little living glyphs might attack though. So be ready.

To write in Unown, prepend each basic A-z alphabet character with the word unown. If you write unowna and unownz the a and z Unown will be shown.

![Alt text](/img/Unown.png?raw=true "pokemon-font Font Unown Glyphs")
This:

```
unownyunownounownu unowncunownaunownuunowngunownhunownt unownaunownlunownl unowntunownhunowne unownuunownnunownounownwunownn unownvunownaunownrunowniunownaunowntunowniunownounownnunowns, unowntunownhunownaunownt unowniunowns unowna unowngunownrunowneunownaunownt unownaunowncunownhunowniunowneunownvunowneunownmunowneunownnunownt!
```

Becomes this:

```
You caught all the Unown variations, that is a great achievement!
```

## Ligatures

There is a ligature to get the original PKMN glyph, plainly write this string: PKMN in capitals without spaces and it will be replaced with PKMN.
There are also the original games' ligatures for 'd, 'l, 'm, 'r, 's, 'v and 't. Sadly, 'n isn't supported, so you can't write cap'n.

## MissingNo

If the font doesn't support a certain character, � is displayed, in this font that is a MissingNo, because a tiny MissingNo is sugoi kawaii.

![Alt text](/img/MissingNo.png?raw=true "pokemon-font Font MissingNo Glyph")

## Japanese

I extended support to cover the full Unicode blocks for Hiragana and Katakana, which holds a few obscure characters that aren't used anymore, but gotta catch 'em all right?

![Alt text](/img/Japanese.png?raw=true "pokemon-font Font Japanese Glyphs")

## What we learned

While making this font I learned how to create SVG shapes with raw code, how modern fonts are encoded, how to convert between font formats, how to deal with size, kerning, ligatures, etc. This is also the first time I'm publishing a package to npm and bower.

We used [Glyphs App](https://glyphsapp.com) in the end to manage the `.ufo` master 'file'/folder.

## License

Copyright (c) 2016-2017, Superpencil (https://superpencil.com | support@superpencil.com>),
with pokemon-font.

This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is included in the repository, and is also available with a FAQ at:
http://scripts.sil.org/OFL
