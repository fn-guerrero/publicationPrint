# publicationPrint

Script to generate publication-ready figures in Matlab

```Matlab
publicationPrint(fig, fig_width, fig_height, file_name, file_type, font_size, font_name)
```
Assigns a size in cm to the figure, changes the font to Times New Roman 11, and exports an image of the requested type. Optionally, fsz and fName can be modified to change the font style.

### ARGUMENTS:

 - fig: Handle to the figure (h1 = handle(1), gcf retrieves the current handle).
 - fig_width: Desired width in cm.
 - fig_height: Desired height in cm, or an empty array [] for a 1.6 aspect ratio.
 - file_name: Filename.
 - file_type: File type to generate: 'png', 'eps', 'pdf'.

### OPTIONAL:

 - font_size: Font size (default: 11).
 - font_name: Font type (default: Times New Roman).

### TYPICAL EXAMPLE:

```Matlab
publicationPrint(gcf,8.6,[],'Figure1','pdf')
```
Saves the current figure in the current directory with a width of 8.6 cm and a height of 8.6/1.6 cm.
