# Ext B: Black Pond Brews

This standalone public repo is for marketing and email automation tools for Black Pond Brews LLC, a brewery in Danielson, Connecticut. Civic AI Club students at Pomfret School build the project; discovery is complete, but Phase 1 has not been chosen.

## Beginner quick start

Full guide: https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md

1. First time: check Git with `git --version`, set your Git name and GitHub email, accept the club invite, and sign in with GitHub Desktop or `gh auth login`. Clone only your project's repo, open its folder, and read its README setup steps.
2. Start each work session from the latest main, then make a branch:

```sh
git checkout main
git pull origin main
git checkout -b feature/short-description
# Make and check your changes before continuing.
git status
git add .
git commit -m "Describe your change"
git push --set-upstream origin feature/short-description
```

Use `feature/`, `fix/`, or `chore/` as appropriate, with lowercase names and hyphens. Commit small working pieces; do not edit or push main directly.
3. Open a PR on GitHub, fill in the template, and get someone else's approval and passing checks where CI exists. Push review fixes to the same branch. After it is merged, pull main again before starting another branch.
4. If stuck, ask in the case chat, then Keke, then Luke or Cayden. Ask before doing anything drastic.

## Shared workflow

- All paths below start at this repo's root. Prefer clear code over clever code for high school developers learning collaboration. If you generate code the developer cannot explain, say so and explain it in plain English.
- Never push to `main`; use a branch and PR with one approving review. Use lowercase `feature/`, `fix/`, or `chore/` names with hyphens and no spaces.
- Make small, frequent commits with plain-English messages. Use `.github/pull_request_template.md` for PRs.
- Never commit API keys, tokens, email account or app passwords, or `.env` files. Every environment variable needs a placeholder in `.env.example`.
- Never add Co-authored-by, Generated with, Made-with, Claude-Session or any other AI attribution line to a commit message or pull request description. When squash merging, delete any such lines GitHub puts in the merge message.
- Use the onboarding guide above for Git, branching, PR, and merge-conflict questions. Project context is in `README.md` and `.cursor/rules/ext-b-black-pond-brews.mdc`.

## Scope and client work

- The team is still to be assigned; Cayden Auyang is the club lead. Confirm Phase 1 scope with Cayden before building. When developers are assigned, update the team line in the project rule and `.github/CODEOWNERS`.
- In client-facing emails, demos, and handover docs, describe a time-saving tool. Do not lead with "AI" or name the school's faculty projects.
- Do not promise scope or timelines without Cayden.
- Discovery notes, contacts, and client requirements belong in the private running doc linked from the Civic AI Club Google Drive, never this public repo.
- If code does not express a needed requirement, ask the developer to check the running doc instead of guessing. Implement the requirement without pasting notes, examples, or client data into comments.

## Client data and safety

- Never commit client data. Sales PDFs, exports, spreadsheets, customer lists, and email lists stay in gitignored `data/` or Drive. Read `data/README.md`.
- `.gitignore` blocks `data/*` except `data/README.md`, plus `*.pdf`, `*.xlsx`, `*.xls`, `*.xlsm`, and `*.csv`. Never suggest `git add -f` to bypass it.
- Customer names and email addresses are the brewery customers' personal data. No phone numbers, customer names, email addresses, or other personal contact details beyond the README's existing baseline in code, comments, tests, commit messages, or PR descriptions.
- Follow the stricter project rule for new documentation: keep contact details, discovery notes, and client requirements out of comments, tests, docs, commit messages, and PR descriptions. Refer to the README rather than copying its contact details here.
- Tests and examples must use fabricated values labeled as fake.
- If client data is staged or committed, stop and tell the developer to contact Cayden. Deleting it in a later commit does not remove it from history.

## Setup and checks

The README gives no implementation stack or setup/run commands because Phase 1 is not chosen. Do not invent commands or select a stack; confirm scope with Cayden first.

## Sources

- `README.md`
- `.cursor/rules/civic-ai-workflow.mdc`
- `.cursor/rules/ext-b-black-pond-brews.mdc`
- `.cursor/rules/commit-messages.mdc`
- `data/README.md` is the named data-handling follow-up; the canonical beginner guide is linked above.
