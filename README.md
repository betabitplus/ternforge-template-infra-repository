# ternforge-template-infra-repository

Minimal language-neutral Copier template for Ternforge infrastructure
repositories.

The generated product contains only the role-neutral repository shell:

- `.agents/`
- `.editorconfig`
- `.gitattributes`
- `.gitignore`
- `LICENSE`
- `.github/pull_request_template.md`
- `.copier-answers.yml`
- `README.md`

Role-specific workflows and configuration belong to the consuming repository.
Released components are materialized as committed Vendir snapshots under
`template/_components` and are excluded from generated repositories.

`README.md` is create-once. Copier updates preserve an edited README, do not
restore one deleted by the consumer, preserve unrelated files, and continue to
