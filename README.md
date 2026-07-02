# dss-dar-checklist

The **NIAGADS DSS Data Access Request (DAR) Submission Checklist** — a single,
self-contained static page:

**https://dss.niagads.org/dar-checklist/**

It is one self-contained HTML file (no external assets) and is intentionally not
part of the WordPress/portal build.

```
public/
  index.html      # the page — edit this
```

## Editing

Edit `public/index.html`, commit, and merge to `main`. Merges to `main` are
deployed automatically by GitHub Actions.

## Deployment

Deploys run via GitHub Actions using short-lived, OIDC-federated AWS credentials
(no long-lived secrets in the repo). All environment-specific identifiers are
stored as repository **Actions secrets**, not in the workflow. See
`.github/workflows/deploy.yml`.

Operational/runbook details are maintained internally by NIAGADS DevOps.
