# Repository protection tiers

GitHub Free does not provide organization-wide multi-repository rulesets or
rulesets for private organization repositories. These files are canonical
repository-level policies applied after a repository is public.

## Experiment

`experiment.json` prevents default-branch deletion and force pushes. Pull
requests are encouraged but not required.

## Maintained

`maintained.json` additionally requires pull requests, resolved review
conversations, an up-to-date branch, and the stable `PR Verify` status check.
The repository must emit that check successfully before this ruleset is enabled.

When a second active maintainer joins, change the approval count to one and
enable code-owner review. Add deployment checks such as Vercel only after the
repository emits the exact check successfully.

Organization owners retain an explicit emergency bypass. Bypass use should be
exceptional and visible in repository history.
