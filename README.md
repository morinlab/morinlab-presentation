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

## Using

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

Described below are several main components for the presentation:

