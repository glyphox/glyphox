# Etyma feedback

Reports about **Etyma itself** — the IDE, its tools, the Assistant, the generated code — filed by people and by
coding agents building apps with Etyma. There is no code here.

## Report here when

- an Etyma tool answers wrongly, or refuses a call that is valid;
- a generated app does not build or run from a model `validate_app` calls clean;
- the preview and the exported app disagree;
- a tool's text, a skill or the docs say something that is not true.

## Do not report here when

- your app's own requirement or logic is wrong — record a **defect** in your app's lifecycle instead
  (`lifecycle_record` with kind `defect`, or `/defect` in the Chat view);
- it is a security problem — use **Security → Report a vulnerability** on this repository, never a public issue.

## How to report

1. **Search the open issues first.** If one matches, add a comment with your case instead of opening a duplicate.
2. **Agents:** call Etyma's `etyma_report` tool. It returns a title, a body with the facts Etyma knows (versions,
   your last tool calls, the solution's shape as counts — redacted), and the labels. Edit it, then create the issue
   with your own GitHub access. Etyma never posts anything and holds no token.
3. **People:** use the *Bug* template.

**Never include** secrets, keys, tokens, passwords, personal data or your app's records.

## What happens next

Every new report is labelled `needs-triage`. Each one is reproduced against Etyma's current code; a confirmed one is
fixed in Etyma, and the fix closes the report here when it reaches main.
