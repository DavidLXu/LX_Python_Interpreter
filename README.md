# Lixin's Online Python Interpreter

A minimal Python interpreter that runs in the browser using Pyodide, with a terminal-style output panel.

## Features

- Run Python code directly in the browser
- Terminal-style output for `print()` and errors
- Built-in toy examples (FizzBuzz, recursion, classes, stdlib, traceback demo)
- No backend required (static site)

## Local Development

Run a local static server:

```bash
cd /home/lixin/LX_Python_Env
python3 -m http.server 8000
```

Open:

```text
http://localhost:8000/index.html
```

## GitHub Pages Deployment

This repo includes a GitHub Actions workflow for GitHub Pages:

- `.github/workflows/deploy-pages.yml`
- `.nojekyll`

To enable deployment:

1. Open your GitHub repository settings.
2. Go to `Pages`.
3. Set the source to `GitHub Actions`.
4. Push to `main`.

## Tech Stack

- HTML/CSS/JavaScript
- [Pyodide](https://pyodide.org/) (Python in WebAssembly)

## Notes

- This is a minimal environment focused on stdout/stderr output.
- Interactive `input()` is not implemented yet.
