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
The template is self-contained; shared Python-product components are not part of
this minimal infrastructure product.

`README.md` is create-once. Copier updates preserve an edited README, do not
restore one deleted by the consumer, preserve unrelated files, and continue to
update template-managed files.
