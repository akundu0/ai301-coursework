# Rubric: is this a good first issue?

<!--
THIS IS THE PART YOU WRITE. The skill in SKILL.md executes whatever checks
you define here. It ships empty on purpose: the judgment is your work.

A filled rubric must contain:

1. At least one row in the checks table. Each row needs all four columns:
   - Check: a short name (used in the output JSON).
   - Evidence: exactly what to look at, and where. Name the source
     (repo-facts block, issue body, comment thread, or the locations in
     references/evidence-guide.md). "The repo" is not a source; "the last
     5 default-branch commit dates" is.
   - Pass condition: a condition someone else could apply and get your
     answer. Prefer thresholds with numbers ("a maintainer commented
     within 30 days") over adjectives ("maintainer is responsive").
   - Weight: `required` (a fail here rejects the issue) or `preferred`
     (never changes the verdict; a nice-to-have that helps rank the
     issues you accept).

2. A verdict rule below the table: how the check grades combine into
   accept or reject, including how `unclear` is treated. The verdict
   space is binary. If you write no rule for `unclear`, the skill treats
   it as fail.

Cover what actually kills first contributions. The lecture named four
families: the maintainer is alive, the repo is in use, the scope fits a
newcomer, and nobody else is already on it. A rubric that ignores a family
will fail eval issues designed around that family.
-->
All recency thresholds are measured against the capture date in the bundle
(in live mode, against today).
## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| maintainer_active | Repo facts: last 5 default-branch commits (dates and authors); maintainer first-response sample; author_association badges in the Comments section | Either the newest default-branch commit is within 90 days, OR a comment by an Owner, Member, or Collaborator appears within 90 days. A commit authored only by a `[bot]` does not count, unless it merged a human's pull request. | required |
| repo_active | Repo facts: "archived:" flag and "last push to any branch" | Repo is not archived AND the last push to any branch is within 90 days. | required |
| repo_in_use | Repo facts: "latest release" and stars on the repo line | Latest release is within 12 months, OR the repo has 20+ stars. If neither release nor star data appears, grade unclear. | required |
| issue_open | Issue state; "linked PRs:" with state per PR; PRs mentioned in the Comments section | Issue is open AND no linked or mentioned PR is open or merged. A closed, unmerged PR is an abandoned attempt and does not fail this check. If the sidebar and the thread disagree, believe the thread. | required |
| not_assigned | "this issue: assignees:" under Repo facts | Assignee list is empty. | required |
| scope_bounded | Issue body and comment thread | Pass unless one of these is true: the issue is an umbrella or tracking issue (a list of sub-items meant to be split up); the thread shows the design is still debated with no maintainer decision; a maintainer says the fix touches core internals; the issue is a pure usage question ("how do I...?"); or it has been open for years with several closed, unmerged PR attempts. A short body or a missing reproduction is not a failure. | required |
| ai_policy_allows | "contribution policy" line under Repo facts (CONTRIBUTING.md, AI policy files, PR/issue templates) | Fail only if the policy outright bans AI-generated or AI-assisted contributions. Conditions (disclosure, personal understanding, testing, human review) pass. No stated policy passes. | required |
| newcomer_signal | Issue labels | Has a label like good first issue or help wanted. | preferred |
| clear_acceptance | Issue body | States the expected behavior, or includes reproduction steps or a concrete definition of done. | preferred |


## Verdict rule

<!-- State how the grades above combine into accept or reject, and how
unclear is treated. Example shape (write your own): "accept if every
required check passes; preferred checks never change the verdict, they
rank accepted issues; unclear counts as fail." -->

Accept if every required check passes; preferred checks never change the verdict, they rank accepted issues; unclear counts as fail.

