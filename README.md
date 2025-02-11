# RPG-LaTeX Collection

This is a LaTeX class collection for building thematic RPG documents. The 
original file is based on 
[anoderay's DND-5E-LaTeX-Template](https://github.com/anoderay/DND-5e-LaTeX-Template).

### Changes made
 - Would not compile in TeXLive 2021 due to use of a font that TeXLive was
   not finding. I changed the default font to something suitable.
 - Made tables more flexible by passing column styles as a parameter.
 - Added a custom caption for putting titles on tables etc.
 - Added a spellbox option based on the monsterbox type.
 - Cleaned up monsterbox to match more thematically with choices so far.
 - Gave tables color options and removed itemtable.
 - Gave all three box types color options.
 - Removed dnd-specific naming from files.
 - Original quotebox style just wasn't satisfying; I made it better.
 - Built two better hline options for monsterbox or anywhere desired with color options.
 
### Plans for the future
 - Add framing options to tables
 - Generalize themeing to beyond D&D
 - Create package options to choose theme (fantasy, scifi, steampunk, etc.)
 - Make full-width boxes and tables possible
 - Look into the original to-dos listed below

The template compiles with pdflatex.

![Preview](https://github.com/InfernalBullfrog/RPG-LaTeX/raw/master/scrot.png)


### Installation

Just clone the repo. From terminal:

```sh
$ git clone https://github.com/InfernalBullfrog/RPG-LaTeX.git
$ cd RPG-LaTeX
$ pdflatex example.tex
```

If you don't have LaTeX installed, the following should help you out:
#### Ubuntu
```sh
sudo apt-get install texlive-full
```
#### Arch
```sh
sudo pacman -S texlive-bin texlive-core texlive-latexextra
```
It's a bit unclear exactly what subset of features this module needs. As a 
general rule, we'd recommend installing one of larger ones.

### Package Options
- bg-letter: Loads a letter-sized background-image
- bg-a4: Loads an A4-sized background-image
- bg-print: Loads a printer-friendly background-image (only decal at the bottom)
- bg-full: Loads the full background-image

Per default "bg-letter" and "bg-full" are loaded.

### Todo's

 - Consider implementing more complex tables for monsters, etc.
 - Clean up the table-preset
 - Create more elegant solution for spacing before and after boxes (using \vspace is rather rigid when two boxes follow in a row)
 - Add subtitle option for boxes
 - Sort out box-decals when boxes break column or page
 - Look into adding the ability to add large images to the document. There are some documents made with InDesign out there that accomplish this quite well.


### Image Credit

 - Credit for the background image goes to http://lostandtaken.com/

### Version
2021.1

### License
The MIT License (MIT)

Copyright (c) 2016 InfernalBullfrog

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
