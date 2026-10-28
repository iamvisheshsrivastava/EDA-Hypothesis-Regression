# Contributing

Thanks for your interest in improving this repo. It holds three R Markdown
statistical analysis projects (EDA, hypothesis testing, and regression) from
coursework at TU Dortmund University, plus a small GitHub Pages showcase in
`docs/`.

> **Note:** The `.Rmd` files under `Project_I/II/III` are currently known to
> be placeholders (scraped HTML rather than real R code — see
> [#1](https://github.com/iamvisheshsrivastava/EDA-Hypothesis-Regression/issues/1),
> [#4](https://github.com/iamvisheshsrivastava/EDA-Hypothesis-Regression/issues/4)),
> and the raw datasets they depend on aren't committed
> ([#5](https://github.com/iamvisheshsrivastava/EDA-Hypothesis-Regression/issues/5)).
> Fixing those requires the original project files from the repo owner, so
> external PRs touching the `.Rmd` sources or `data/` folders generally
> aren't actionable yet. Docs, tooling, CI, and the `docs/` showcase site are
> all fair game.

## Local setup

1. Install [R](https://www.r-project.org/) (this repo is pinned to **4.3.2**
   — see `renv.lock`) and [RStudio](https://posit.co/download/rstudio-desktop/)
   (optional but convenient).
2. Clone the repo and open it in RStudio, or `cd` into it from a terminal.
3. Restore the exact package versions pinned in `renv.lock`:

   ```r
   install.packages("renv")  # if you don't already have it
   renv::restore()
   ```

   If you'd rather not use `renv`, you can instead run:

   ```r
   install.packages(c(
     "dplyr", "tidyr", "ggplot2", "gridExtra", "corrplot",
     "cowplot", "ggpubr", "RColorBrewer", "car", "MASS", "lmtest", "leaps"
   ))
   ```

4. Make sure [Pandoc](https://pandoc.org/installing.html) is installed (RStudio
   ships its own copy, so this only matters if you're rendering from the
   command line).

## Rendering a report

Each project is self-contained in its own `Project_*/` folder:

```r
rmarkdown::render("Project_I/Vishesh_Srivastava_ICS_P1_code.Rmd")
```

or, from RStudio, open the `.Rmd` file and click **Knit**.

As noted above, this currently won't produce a real report for any of the
three projects until the corresponding issues are resolved — knitting will
either fail outright or just re-render the placeholder HTML. You can still
run individual chunks interactively once the real source is restored, or use
this to validate changes to the surrounding infrastructure (CI workflow,
`renv.lock`, etc.).

A GitHub Actions workflow (`.github/workflows/render-reports.yml`) re-knits
all three `.Rmd` files on every push/PR that touches a `.Rmd` file or
`renv.lock`, so CI will catch anything that breaks the build once the sources
are real R Markdown.

### Updating pinned package versions

If you add or upgrade a package used by one of the `.Rmd` files, regenerate
the lockfile from R:

```r
renv::snapshot()
```

and commit the resulting `renv.lock` diff.

### Working on the showcase site (`docs/`)

`docs/index.html` and `docs/style.css` are plain HTML/CSS served via GitHub
Pages — no build step. Open `docs/index.html` directly in a browser to
preview changes. A link-check workflow
(`.github/workflows/link-check.yml`) runs on every push/PR and weekly on a
schedule, so please check that any links you add or change resolve.

## Pull request process

1. Fork the repo and create a branch off `main` for your change.
2. Keep PRs focused — one logical change per PR is easier to review.
3. If your change affects rendering (`.Rmd` sources, `renv.lock`, or the CI
   workflow), make sure the "Render Reports" Action passes (or explain in the
   PR description why it still can't, e.g. because of the known placeholder
   `.Rmd` issue).
4. If your change affects `docs/`, make sure the "Link Check" Action passes.
5. Reference any related issue number in your PR description (e.g.
   `Fixes #5` or `Relates to #4`).
6. Open the PR against `main` and describe what you changed and why.

## Reporting issues

Please check [open issues](https://github.com/iamvisheshsrivastava/EDA-Hypothesis-Regression/issues)
first to avoid duplicates. When filing a new one, include:

- What you expected to happen vs. what actually happened
- Steps to reproduce (R version, OS, relevant package versions)
- Which project (`Project_I`, `Project_II`, or `Project_III`) it relates to,
  if applicable

Issues labeled [`good first issue`](https://github.com/iamvisheshsrivastava/EDA-Hypothesis-Regression/labels/good%20first%20issue)
are a good place to start if you're new to the repo.
