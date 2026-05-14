# Morinlab-presentation Quarto template

This is a Quarto extension to simplify preparation of the presentations in the Morin Lab.

## Installing

```bash
mkdir presentation
cd presentation
quarto use template morinlab/morinlab-presentation
```
While executing the last command, the prompt will ask you 3 questions:

- `? Do you trust the authors of this template (Y/n) ›`  Here, answer `Y` (or press Enter)
- `? Create a subdirectory for template? (y/N) ›` Here, answer `N` (or press Enter)
- `? Would you like to continue (Y/n) ›` Here, answer `Y` (or press Enter)

This will install the extension and create an example qmd file that you can use as a starting place for your presentation.

## Structure

After installation, the directory will be populated with required files and directories. The support files are placed in the directory `src/`, while the main required files are in the directory home.

```
.
├── _extensions
│   └── morinlab
├── presentation.qmd
├── _quarto.yml
└── src
    ├── bad_code.png
    ├── bl-abstract.png
    ├── common_problems.png
    ├── dlbcl_coo.jpg
    ├── dlbcl.jpg
    ├── gc.png
    ├── logos.png
    ├── note.png
    └── team.png

3 directories, 11 files
```

## How to use

Described below are several main components for the presentation:

### Presentation content

The main file `presentation.qmd` defines the main content of the presentation. Plese note that the file name of the file itself will be mirroring the name of the folder you created during the installation of the extension, and therefore can vary based on the specific use case. Here, we refer to it as `presentation.qmd` because in the installation instructions, we have created a directory "presentation" (`mkdir presentation`). Regardless of the name of the file, in will be the only file with extension `.qmd` in your folder.

The content follows the standard structure of the Quarto document, with preamble at the top and markdown-style content following it.

In the preamble, the title (`title`), author (`author`), and author's affiliations (`institute`) can be set. The template document contains example of how several affiliations can be attached to a specific author. Other main elements of the presentation can also be adjusted here as necessary following the [standard Quarto format](https://quarto.org/docs/presentations/revealjs/). The template already defines for you that images will be rendered in `svg` format (recommended for best compatibility with different projectors, preservation of color pallete, and overall quality) and centered on the slide. In the preamble, we also define the background image for the tile slide - you can modify it here by placing your image to the `src/` folder and changing the default value of `src/dlbcl.jpg` to the path for your file, as well as adjust the default opacity of the background image.

The main content in the file provided for you out of the box contains several sections with examples of how to paste images, animate slides, add speaker notes, modify slide title formatting, define different layout for the slide, use code-computated outputs, etc. Please run `quarto render` in order to see the representation of the markdown code.

This file should be adjusted accordingly to have your presentation content.

