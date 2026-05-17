# Conan SRD

A fan-made system reference document for running games in the Hyborian Age using the 2d20 system. Built as a Jekyll site, deployable to GitHub Pages.

This is a personal reference for the GM and a small group of players. It summarizes mechanics in original prose; it is not a reproduction of the published rulebook, and the rulebook remains the authority where the two disagree. Setting material, flavor text, named characters, and adventures are intentionally **not** included — those belong to the source.

## What's here

```
conan-srd/
├── _config.yml          # Jekyll configuration + sidebar nav
├── Gemfile              # Locked to github-pages so local matches deploy
├── _layouts/
│   └── default.html     # The single layout — header, sidebar, content, pager
├── assets/
│   └── css/
│       └── style.scss   # Conan/Hyborian theme: dark parchment, oxblood, brass
├── _pages/              # All chapter content (Jekyll collection)
│   ├── getting-started.md
│   ├── core-mechanic.md
│   ├── attributes.md
│   ├── skills.md
│   ├── talents.md
│   ├── character-creation.md
│   ├── momentum-and-doom.md
│   ├── action-scenes.md
│   ├── combat.md
│   ├── damage-and-recovery.md
│   ├── equipment.md
│   ├── sorcery.md
│   ├── gamemastering.md
│   ├── encounters.md
│   └── appendix-tables.md
├── index.md             # The foreword / landing page
├── .github/workflows/
│   └── pages.yml        # GitHub Actions: build + deploy on push to main
└── README.md
```

## Running it locally

You need Ruby 3.1+ and Bundler.

```bash
cd conan-srd
bundle install
bundle exec jekyll serve --livereload
```

Then open <http://127.0.0.1:4000>.

If `bundle install` fails on Windows, install RubyInstaller-Devkit and re-run; the `wdm` and `tzinfo-data` gems are listed in the Gemfile for Windows.

## Deploying to GitHub Pages

Two options. Pick one.

### Option 1 — GitHub Actions (recommended)

1. Push the `conan-srd/` folder to a new GitHub repository. The repo can be either the contents of `conan-srd/` at the root, or this whole `Splatbook` repo with the workflow's `working-directory` pointed at `conan-srd/`.
2. In the repo settings, **Pages → Build and deployment → Source**: select **GitHub Actions**.
3. Push to `main`. The workflow in `.github/workflows/pages.yml` builds Jekyll and deploys.
4. The site will be available at `https://<user>.github.io/<repo>/`.

If your repo name isn't the same as the URL path you want, set `baseurl` in `_config.yml` to match (e.g. `"/conan-srd"` if the URL is `https://user.github.io/conan-srd/`).

### Option 2 — Classic Pages (gh-pages branch)

1. Push to GitHub.
2. Settings → Pages → Source: **Deploy from a branch** → `main` (or `gh-pages`) → `/ (root)`.
3. GitHub will run Jekyll for you using the `github-pages` gem. This is why the Gemfile pins to it — local build matches the remote.

## Editing

- **Content pages** live in `_pages/` (a Jekyll collection). Each has YAML front matter (`title`, `chapter`, optional `subtitle`); the rest is Markdown.
- **Sidebar order** is set by the `nav:` list in `_config.yml`. Adding a page means adding both the file and an entry there.
- **Theme** is one SCSS file (`assets/css/style.scss`). All the palette variables are at the top.
- **Drop caps** are applied automatically to the first paragraph of every chapter via `:first-of-type::first-letter`.

## A note on scope

This SRD covers mechanics. It does not cover:

- The Hyborian gazetteer or any kingdom-specific lore.
- Named NPCs from the rulebook (Conan, Bêlit, Thoth-Amon, etc.).
- The published adventure.
- The full spell list, talent list, or weapon catalog — only enough of each to teach the *system* of each.

For all of those, use the rulebook. This is a quick-lookup companion, not a replacement.

## License

The site code (Jekyll configuration, layouts, CSS, build workflow) is released to you under the MIT License — do what you want with it.

The *game system* it documents is the work of its publisher; this site is an unofficial fan reference and asserts no claim over the rules it summarizes. The Hyborian Age and its characters are the property of their respective rights-holders.
