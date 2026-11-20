# hello-static

A simple **static site** built with HTML, CSS, and JavaScript — automatically deployed to **GitHub Pages**.

## Live site

🌐 **[https://tegor1212.github.io/hello-static/](https://tegor1212.github.io/hello-static/)**

## What's inside

| File          | Purpose                         |
|---------------|---------------------------------|
| `public/index.html` | Main page with interactive counter |
| `public/style.css`  | Page styling                    |
| `public/script.js`  | Counter logic                   |
| `public/favicon.svg`| Site favicon                    |

## Run locally

```bash
# Open in browser
open public/index.html

# Or serve with any HTTP server
python3 -m http.server -d public -p 8000
```

## CI/CD pipeline

The [workflow](.github/workflows/ci-cd.yml) on every push to `main`:

1. **CI** — validates HTML, CSS, and JavaScript via linters (`html-validate`, `stylelint`, `eslint`)
2. **Deploy** — uploads the `public/` folder to **GitHub Pages**

The site goes live at the URL above within minutes of merging.