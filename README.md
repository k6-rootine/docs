# Rootine -- Documentation

## Folder structure

```
project/
├── rootine/   ← Pascal files
└── docs/      ← Documentation output
```

## Generating the documentation

The documentation is generated with [PasDoc](https://pasdoc.github.io/). Run the command from inside the `rootine` folder; the HTML output is written to the `docs` folder next to it.

### Windows (Command Prompt)
If the `docs` folder does not exist yet, create it first:
```bash
mkdir ..\docs
```
Then, run the command to make the documentation:
```bash
pasdoc --output=..\docs --format=html --title="Rootine - Documentation" *.pas
```

### Linux (terminal)
If the `docs` folder does not exist yet, create it first:
```bash
mkdir -p ../docs
```
Then, run the command to make the documentation:
```bash
pasdoc --output=../docs --format=html --title="Rootine - Documentation" *.pas
```

In the end, open `docs/index.html` in a browser to view the documentation.
