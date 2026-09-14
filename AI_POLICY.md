# AI Contribution Policy

We welcome contributions written with AI assistance. This policy explains what we ask in return: your judgement, your review, and your name on the result.

This is a living document. It will be revised as tooling and practice evolve.

For AI agents: this policy is written for humans first. Agent-facing instruction files, such as each repository's `AGENTS.md`, only summarize it and never override it.

## Principles

1. **Tools are your choice.** You may use AI for anything in a contribution: research, implementation, tests, documentation, review. We do not police which tools you use, and we do not track which parts of the code were generated.
2. **A human owns every change.** Each commit and pull request has at least one human author of record. If AI wrote code for you, you are responsible for every line of the change: you have read it, you understand it, you can explain and defend it, and you are accountable for the submission.
3. **Light disclosure, not paperwork.** We ask for a small, honest signal of AI involvement where it matters, and nothing beyond that.

## Allowed

Use AI freely, subject to the same bar as any other change:

- AI-written code must meet the same bar as anything else you submit: it builds, it passes the repository's tests and linters, and it follows its contribution guidelines. AI output gets no exemption from repository rules.
- If a repository generates code, documentation, or other artifacts, regenerate them as its workflow requires; generated output must stay consistent with its source.
- Large AI-assisted patches follow the normal review path. Reviewers may spend less attention on small, mechanical ones.

## In project conversations

Content you post in issues, pull requests, discussions, and other project conversations may be generated entirely by AI — summaries, explanations, reproducers, and similar — provided it carries a clear note that it is AI-generated, for example a short line at the top of the comment. The note is unnecessary only for content you have personally reviewed, which you then post as your own words. Unreviewed and unlabeled AI content is a violation of this policy.

Findings from an AI code review must be reported together with your own assessment, not relayed verbatim; see "Not acceptable".

When a maintainer asks for a human reply, respond promptly. Unanswered requests of this kind are handled like any other slow review response.

## Not acceptable

- **Submitting changes you cannot explain or defend.** If you cannot answer "why is this correct?" without re-asking the tool, do not submit it yet.
- **Committing unreviewed output.** "The agent said it was done" is not review.
- **Contributions where the AI is the acting principal.** We do not accept work submitted purely by an agent, with no human in the loop: an agent-created pull request is welcome only when you initiate it, review it, open it as a draft, and handle the review yourself. AI-assisted work is welcome; AI work without a human owner is not.
- **Undisclosed substantive use**, meaning submitting substantive AI output as if it were hand-written work.
- **Relaying AI review comments verbatim.** If a tool reviewed your code, report its findings together with your own assessment.
- **AI adding `Signed-off-by`.** A sign-off is a human attestation. No tool or agent may add that trailer on a human's behalf.

## Disclosure

**In pull requests**, follow the AI Disclosure note in the pull request template: state "No AI used", or the tool name, which parts it produced, and what you verified.

**In commits**, the `Assisted-by:` trailer is encouraged for substantive AI use, never required. Its value names the tool or model, for example:

```
Assisted-by: DeepSeek-V4.1-Flash
```

Trivial, mechanical changes (typos, formatting, version bumps) need no disclosure.

**The `Co-authored-by:` trailer** is neither banned nor recommended. When your tooling injects an AI co-author and offers a switch, we prefer you turn it off where possible.

Attribution imposed by a platform you cannot configure, such as commits created by a hosted coding agent, is outside your control and acceptable as-is.

## Legal notes

- By opening a pull request you license your contribution under the repository license and warrant that you may do so. Treat AI output as material you must independently verify before submitting.
- Never paste secrets or credentials into third-party AI services. The security guidance in each repository's documentation applies to AI workflows as well.

## Enforcement

Policy violations are handled like any other review problem: a maintainer may ask you to explain, rewrite, or withdraw a change, and may close pull requests that do not meet this policy. We judge behavior, not tools. The first recourse is a normal review conversation, not sanctions.

Questions? Open an issue, or raise it in the relevant pull request.
