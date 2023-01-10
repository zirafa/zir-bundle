# Zir-Bundle (Custom Textmate Bundle)

Trying to keep track of my textmate configuration and preferences as I try and migrate from Atom to Textmate.

## Installation
Download the zip file for this bundle or clone the repo and open zir-bundle.tmbundle in Textmate to install.

## Included macros (key bindings)
- Back Tab: shift + tab (same as ShiftLeft)
- Duplicate Line: ⌘D

## Included themes
- Zir Theme (custom theme based on Github Light)
- Monokai Light (https://github.com/rjfranco/monokai-light)
- Github Light & Dark (https://github.com/primer/github-textmate-theme)

## My setup notes
- Textmate > Preferences > Show Tab for single document
- Set font to Menlo 14 Regular: View > Font > Show Fonts
- Disable Soft Wrap: View > Disable Soft Wrap
- Set column width to 80: View > Wrap Column > 80
- Show wrap column: View > Show Wrap Column
- Soft tabs, 2 spaces: Click bottom toolbar to configure tab settings
- Enable shell support: Textmate > Preferences > Terminal (you can then open a file from terminal with ```mate filename.txt```)
- To disable autoclosing brackets, open up terminal and run ```defaults write com.macromates.TextMate disableTypingPairs YES```
- Set and use custom light theme (zir-theme): View > Theme > Theme for Light Appearance
- Modify or disable default Markdown font styles: Bundles > Edit Bundle > Themes > Settings (Defaults to giant Baskerville heading styles and courier)
- Enable Markdown: Github GFM Syntax Bundle (but do not enable GFM body styles bundle): Textmate > Preferences > Bundles
- Download [Typescript language bundle](https://github.com/stanger/TypeScript-TextMate)
- ShiftRight (Block Indent): option + tab or ⌘]
- ShiftLeft (Reverse Block Indent): shift + tab or ⌘[ 
- ctrl+shift+p: see what the descendent selector is for selection
- ctrl+shift+n: number of words for selection

## @@TODOS

Textmate is slightly quirky in some areas, mostly around Tab key behavior:

- Can't block indent multiple lines with the Tab key (instead it replaces the text with a tab character). It would be great if you could set a conditional command for the Tab key, i.e. "If there is nothing selected, insert tab character, else if multiple lines are selected do Block Indent (ShiftRight)".
- Inserting a tab in the middle of a line works as expected. Removing a tab (or doing a back tab) in the middle of a line doesn't seem to work. ShiftRight/ShiftLeft always shifts the line from the start of the line, not the position of the cursor. 
- Soft tabs are treated as virtual hard tabs. Soft tabs inserts 2 spaces but pressing the left arrow key or delete key I expect to be able to navigate back 1 space. Instead it always jumps back 2 spaces.
- Opening a new file from Finder or Terminal always opens in a new window instead of a new tab. Setting the File Browser Project directory to match your home directory may fix: View > Show File Browser > Navigate to your home directory, and then click the directory path at the top and select "Use as Project Folder"

## Alternatives

Other open source editors to check out:
- [Atom Community](https://github.com/atom-community/atom)
- [Pulsar Edit](https://github.com/pulsar-edit/pulsar)
- [VSCodium](https://github.com/VSCodium/vscodium)
- [Lapce](https://github.com/lapce/lapce)
- [Brackets](http://brackets.io/)
- [CotEditor](https://github.com/coteditor/CotEditor)
- [SubEthaEdit](https://github.com/subethaedit/SubEthaEdit/)
- [Emacs](https://emacsformacos.com/)


