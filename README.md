# claude-review

The Claude code review, kept in one place. Each repository that uses it has one small
workflow, `.github/workflows/claude-code-review.yml`, that calls
`.github/workflows/review.yml` here on its pull requests and passes its
`CLAUDE_CODE_OAUTH_TOKEN` secret. The rules, the lenses and the scripts are in `review/`;
a change here applies to every repository on its next pull request event.

The review takes a project's own rules only from that repository's documentation, if it
has any. Nothing here is specific to any one repository.
