# PhotonicModulatorModels
Collection of python notebooks and analytic models.

## Website (MyST + GitHub Pages)

The notebook [`semiconductor.ipynb`](./semiconductor.ipynb) is published as a
[MyST](https://mystmd.org) website. Start page: [`index.md`](./index.md),
config: [`myst.yml`](./myst.yml).

Live URL after enabling Pages: `https://<org>.github.io/PhotonicModulatorModels/`

```bash
pip install -r requirements.txt
npm install -g mystmd
myst start               # preview (stored outputs)
myst start --execute     # preview with re-execution
myst build --html        # static build into _build/html
myst build --execute --html  # re-execute notebook, then build
```

Pushes to `main` deploy automatically via [`.github/workflows/deploy.yml`](./.github/workflows/deploy.yml).
First enable **Settings → Pages → Source: GitHub Actions** in the repo.
