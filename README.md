# DRL Power Grid — Quarto GitHub Pages Version

This is the GitHub Pages-ready version of the Quarto research showcase.

For Chinese step-by-step publishing instructions, open:

`GITHUB_PAGES_GUIDE_CN.md`

## Quick workflow

1. Edit `index.qmd`
2. Preview locally
3. Run `quarto render`
4. Upload/push the project to GitHub
5. Set GitHub Pages to **main / docs**

The `docs/` folder is the published website output.


# Quarto DRL Power-Grid Research Showcase

This folder is a ready-to-edit Quarto website based on the supplied Word document
**DRL applied in power grid.docx**.

## Folder structure

```text
quarto_drl_grid_bundle/
├── _quarto.yml
├── index.qmd
├── styles.css
├── README.md
├── preview.bat
├── render.bat
└── images/
    ├── case14_topology.png
    └── performance_metrics.png
```

## Recommended editor

Use **Visual Studio Code** with the **Quarto** extension.

## First-time setup on Windows

1. Install Quarto.
2. Install Visual Studio Code.
3. In VS Code, install the extension named **Quarto**.
4. Open this entire folder in VS Code.
5. Open `index.qmd`.
6. Click **Preview** in VS Code.

Alternatively, double-click `preview.bat` after Quarto has been installed.

## Important files

- `_quarto.yml` controls the website format.
- `index.qmd` contains the research content.
- `styles.css` controls the page appearance.
- `images/` contains figures extracted from the original Word file.

## Page logic

The page is organized as:

**Research question → Test system → DRL framework → Action space → Methods →
Metrics → Results → Main findings**

## Render

In a terminal opened inside this folder:

```bash
quarto preview
```

or:

```bash
quarto render
```

The final HTML site will be written to `_site/`.

## Scope

The current page uses only information contained in the supplied Word document and its
embedded figures. Reward design, state representation, neural-network architecture,
training hyperparameters, and multi-seed uncertainty are not invented and are left for
later expansion when those materials are available.

## HTML indentation fix

Nested HTML used for the visual cards has been left-aligned so Quarto/Pandoc does not interpret it as an indented code block.
