# Go PR review fixtures
Five independent Go PR fixtures support the Building Your Go Agent lessons on the course
platform. Follow the lesson for assignment steps; each review branch is based on main.
The base contains model, API adapter, and repository packages. No application deployment
or credentials are required. Use a supported Go release (language baseline in go.mod: 1.22).
Validate locally using go test ./... and go vet ./... .
PR-05 contains an intentionally non-isolated test skipped by default. Keep RUN_LIVE_TESTS
unset. Credential strings in review branches are synthetic examples, never real secrets.

## Course PRs

| Case | Pull request | Teaching input |
| --- | --- | --- |
| PR-01 | [1](https://github.com/nebius-academy-templates/go-pr-review-practice/pull/1) | Ride history service |
| PR-02 | [2](https://github.com/nebius-academy-templates/go-pr-review-practice/pull/2) | Notification manager |
| PR-03 | [3](https://github.com/nebius-academy-templates/go-pr-review-practice/pull/3) | Payment client |
| PR-04 | [4](https://github.com/nebius-academy-templates/go-pr-review-practice/pull/4) | Trip service |
| PR-05 | [5](https://github.com/nebius-academy-templates/go-pr-review-practice/pull/5) | Checkout service |

Configure the reviewer in the separate
[building-your-go-agent](https://github.com/nebius-academy-templates/building-your-go-agent)
repository. Codex CLI and Claude Code use the same Go inputs; Codex Desktop is optional.
Use the agent repository's hosted GitHub MCP setup from the walkthrough. Record each reviewed head SHA;
case numbers are fixed while a PR's content can change. Each branch is based independently
on main; do not stack or merge them. Keep the teaching defects intact.

For prompt-injection exercises use temporary local copies of the diffs, never a comment or
commit on these PRs. The required course exercises decline publication and need read access
only. Evidence belongs in the agent repository, with credential values redacted.
