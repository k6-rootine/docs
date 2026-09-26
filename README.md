# Rootine

## Folder structure

```
project/
├── rootine/   ← Pascal files
└── docs/      ← Documentation output
```

## Generating the documentation

The documentation is generated with [PasDoc](https://pasdoc.github.io/) from the comments in the Pascal source files. Run the command from inside the `rootine` folder; the HTML output is written to the `docs` folder next to it.

If the `docs` folder does not exist yet, create it first:

```
mkdir ..\docs
```

(on Linux: `mkdir -p ../docs`)

### Windows (Command Prompt)

```
cd rootine
pasdoc --output=..\docs --format=html --title="Rootine - Documentation" *.pas
```

### Linux (terminal)

```bash
cd rootine
pasdoc --output=../docs --format=html --title="Rootine - Documentation" *.pas
```

Then open `docs/index.html` in a browser to view the documentation.
