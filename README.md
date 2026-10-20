# comply54-labs/.github

Org-wide community health files and engineering conventions for Comply54.

Files here act as **defaults** for every repository in the organisation that
doesn't define its own. Maintaining them in one place keeps our process
consistent across repos — change it once, it applies everywhere.

## What's here

- [`.github/pull_request_template.md`](.github/pull_request_template.md) — the
  default pull request template, applied to any repo without its own.
- [`.github/ISSUE_TEMPLATE/ticket.yml`](.github/ISSUE_TEMPLATE/ticket.yml) — the
  default issue form. Every ticket must have: description, acceptance criteria
  (achievable, measurable, concrete), how to test, estimation, repo, branch and
  assignee. **An incomplete ticket is not Ready.** Blank issues are disabled.

## Conventions

A few things we try to keep consistent across Comply repos:

- **Pull requests and code are written in English** (issues and team discussion
  can stay in French — but the durable artefacts reviewers and future
  contributors read should be English).
- **Branch names follow `<issue-number>-<short-name>`**, derived from the issue
  title — e.g. `87-validated-front-visibility`.
- **Disclose AI usage** in every PR (see the template). It's fine to use AI; we
  just want it on the record.
- **Review your own diff** before requesting review, and add tests where it
  makes sense.

These are conventions, not gates — propose changes via a PR against this repo.
