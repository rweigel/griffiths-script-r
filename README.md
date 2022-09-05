**Griffiths-script-r**

This repository was created to store files mentioned in a [StackExchange Post](https://tex.stackexchange.com/a/626189).

This repository contains TrueType Font files for "script r" used for **r-r'** in *Introduction to Electrodynamics* by David Griffiths. It appears that the font used for "script r" is Kaufmann. 

In the files

```
ttf/U+0509-is-Kaufmann-r.ttf
ttf/U+0509-is-Bold-Kaufmann-r.ttf 
```

the symbol ԉ ([Cyrillic Small Letter Komi Lje](https://www.compart.com/en/unicode/U+0509)) has been replaced with lowercase *r* extracted from

```
ttf/Kaufmann.ttf
ttf/Kaufmann_Bold.ttf
```

These two files were downloaded from https://fontsov.com/family/kaufmann-font-family.html. The `U+0509-*` files have only a single glyph and were created by modifying the files downloaded from [fontsov.com](fontsov.com) using [FontForge](https://fontforge.org/en-US/).

When generating the `U+0509-*` files using [FontForge](https://fontforge.org/en-US/), I chose the option to include the TeX table. (According to the FontForge documentation, "The TeX table is an extension to the TrueType format and the various data you would expect to find in a ttf file (that isn't already stored elsewhere in the ttf file"). However, I have not tested these files using LaTeX. It is likely that the method described at https://tex.stackexchange.com/a/535744 could be used.

In the file `katex.html`, I demonstrate how "script r" can be used in KaTeX. `mathjax.html` shows an use in MathJaX. I have not tried using the `U+0509-*` files in LaTeX.

I attempted to extract the "script r" symbol from the pdf files [provided by Griffiths](http://academic.reed.edu/physics/faculty/griffiths/script_r.zip) using FontForge (the files in this zip archive are also in the directory `script-r`). Although the shapes and weights of the glyph appear identical, there is a rightward shift in the non-bold r that causes it to overlap with superscripts.

