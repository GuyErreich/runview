# runview

Cross-backend run narration for CLI tools and CI.

`runview` is a small Python library that presents the same run (phases, status,
messages, tables, summary) through one of three renderers:

- **rich** — one-page live dashboard for local TTYs
- **plain** — unstyled milestone lines for non-TTY CI
- **github** — GitHub Actions groups, annotations, and step summary

A separate forensic file sink is always available. Host apps configure app name,
theme, and quiet third-party loggers via a constructor `Config` — no product
logic lives here.

This repository is a name claim and future home for the package currently being
extracted from [Action-Semver-Control](https://github.com/GuyErreich/Action-Semver-Control).
Implementation lands here after the in-repo sibling package (`src/runview/`)
stabilizes.

## License

Mozilla Public License 2.0 (MPL-2.0).
