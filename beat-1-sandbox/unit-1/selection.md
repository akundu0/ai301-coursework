# Unit 1 — Issue Selection

Path: `beat-1-sandbox/unit-1/selection.md`

Record of the issue carried into Unit 2, and of the evaluation runs that produced
`eval-run.txt`. This file is graded at the path above; a copy kept anywhere else in the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the
wrong label is not graded.

---

## Selected issue

**Issue link**

[The individual Path Review issue page. A link to the repository or the issue list
does not satisfy this field.]
https://github.com/codepath/pathreview-ai301-fa26-s3/issues/68

**Verdict output**

[Your skill's live-mode output for this issue, pasted verbatim and ending with the
fenced JSON verdict block. A summary does not satisfy this field.]

**The verdict must record `accept` for this issue.** Choose an issue your own skill
accepts. If your skill rejects every candidate you try, that is a signal about your
rubric rather than about the issues: revise it and re-run — retries are unlimited and a
partial re-run costs about $0.20 — or run the skill on different candidates. Output
recording `reject` for the issue you chose earns no credit for this field.

Note: the skill is rejecting candidates because of the repo_in_use condition, but I think this is a necessary and useful constraint, so I am leaving it for now! But since this is a classroom repo, it is rejecting issues. If it was removed, the skill would accept all issues.

```
paste the output here, including the closing JSON block
```
- 0 pull requests in the repo, total, in any state
- docs/CONTRIBUTING.md (189 lines) contains no mention of AI, assistance, generation, or disclosure; no AI_POLICY.md; PR template has no AI checkbox

Per-issue — all three are structurally near-identical: opened by Aburke225 (COLLABORATOR) on 2026-09-10, labeled bug + good first issue + tier-1, no assignees, no linked or mentioned PRs, single bounded bug with named files.

 The claim comments on #69 (Yina-Mu, 2026-09-20) and #68 (acordero4852, 2026-09-19) are both from author_association: NONE classmates; per the Path Review house rule I ignored them, and your rubric's not_assigned and issue_open checks don't read claim comments anyway. #54 has no comments at all.

Worth flagging: this is a rubric bug, not a real signal. Your scope pins the field to exactly one repo, and that repo is an 11-day-old classroom seed — a teaching copy will never cut a release or collect 20 stars. As written, your rubric rejects 100% of the issues it is allowed to see, so it can't select anything. repo_in_use is a sound check for wider GitHub, but it needs a Path Review carve-out or a signal that actually varies in a classroom (the repo has 10 forks and an active seeding maintainer). I left the verdicts as the rubric dictates — the fix belongs in rubric.md, not in this run.

For when you do fix it: all three pass everything else, and on your fit profile (Python backend, wanting AI-platform and ML-engineering exposure) #68 would rank first — KeywordSearcher.index() / BM25 is retrieval-infrastructure work in rag/, the closest of the three to AI platform engineering, and the narrowest change. #69 is also rag/ but parser-shaped; #54 is regex work in ingestion/. That ordering is fit only and does not change the verdicts above.

[
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/69",
    "checks": [
      {"name": "maintainer_active", "grade": "pass", "evidence": "Newest main commit 2026-09-16T21:42:18Z by Aburke225 (human COLLABORATOR), 5 days before today"},
      {"name": "repo_active", "grade": "pass", "evidence": "archived: false; last push to any branch 2026-09-16, within 90 days"},
      {"name": "repo_in_use", "grade": "fail", "evidence": "0 releases and 0 tags; stargazers_count = 2, below the 20+ threshold"},
      {"name": "issue_open", "grade": "pass", "evidence": "state: open; repo has 0 PRs in any state; timeline shows no cross-referenced or connected PR"},
      {"name": "not_assigned", "grade": "pass", "evidence": "assignees: []"},
      {"name": "scope_bounded", "grade": "pass", "evidence": "Single bug in output_parser.py opened by a COLLABORATOR, labeled bug/good first issue/tier-1, two named files, no umbrella or design debate"},
      {"name": "ai_policy_allows", "grade": "pass", "evidence": "docs/CONTRIBUTING.md has no AI mention; no AI policy file; PR template has no AI disclosure"},
      {"name": "newcomer_signal", "grade": "pass", "evidence": "labels include 'good first issue'"},
      {"name": "clear_acceptance", "grade": "pass", "evidence": "'The fallback path should handle array responses' plus definition of done: remove the H-02 xfail marker"}
    ],
    "verdict": "reject"
  },
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/68",
    "checks": [
      {"name": "maintainer_active", "grade": "pass", "evidence": "Newest main commit 2026-09-16T21:42:18Z by Aburke225 (human COLLABORATOR), 5 days before today"},
      {"name": "repo_active", "grade": "pass", "evidence": "archived: false; last push to any branch 2026-09-16, within 90 days"},
      {"name": "repo_in_use", "grade": "fail", "evidence": "0 releases and 0 tags; stargazers_count = 2, below the 20+ threshold"},
      {"name": "issue_open", "grade": "pass", "evidence": "state: open; repo has 0 PRs in any state; only comment is a student claim, no PR mentioned"},
      {"name": "not_assigned", "grade": "pass", "evidence": "assignees: []"},
      {"name": "scope_bounded", "grade": "pass", "evidence": "Single bug in KeywordSearcher.index() opened by a COLLABORATOR, labeled bug/good first issue/tier-1, two named files, no design debate"},
      {"name": "ai_policy_allows", "grade": "pass", "evidence": "docs/CONTRIBUTING.md has no AI mention; no AI policy file; PR template has no AI disclosure"},
      {"name": "newcomer_signal", "grade": "pass", "evidence": "labels include 'good first issue'"},
      {"name": "clear_acceptance", "grade": "pass", "evidence": "\"index() shouldn't raise on an empty corpus either\" plus definition of done: remove the H-01 xfail marker"}
    ],
    "verdict": "reject"
  },
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/54",
    "checks": [
      {"name": "maintainer_active", "grade": "pass", "evidence": "Newest main commit 2026-09-16T21:42:18Z by Aburke225 (human COLLABORATOR), 5 days before today"},
      {"name": "repo_active", "grade": "pass", "evidence": "archived: false; last push to any branch 2026-09-16, within 90 days"},
      {"name": "repo_in_use", "grade": "fail", "evidence": "0 releases and 0 tags; stargazers_count = 2, below the 20+ threshold"},
      {"name": "issue_open", "grade": "pass", "evidence": "state: open; repo has 0 PRs in any state; timeline shows only label events, no cross-reference"},
      {"name": "not_assigned", "grade": "pass", "evidence": "assignees: []"},
      {"name": "scope_bounded", "grade": "pass", "evidence": "Single regex bug in _detect_sections() opened by a COLLABORATOR, labeled bug/good first issue/tier-1, three named failing tests, no umbrella or debate"},
      {"name": "ai_policy_allows", "grade": "pass", "evidence": "docs/CONTRIBUTING.md has no AI mention; no AI policy file; PR template has no AI disclosure"},
      {"name": "newcomer_signal", "grade": "pass", "evidence": "labels include 'good first issue'"},
      {"name": "clear_acceptance", "grade": "pass", "evidence": "Runnable repro snippet with 'observed: []  (expected: Education, Skills)'"}
    ],
    "verdict": "reject"
  }
]
---

## Eval iterations

Quote source text directly in each field below. Paraphrase does not satisfy them.

**Run history**

[The agreement score of each run you did, in order. A single run is a complete answer if
only one run occurred. **The last score in your list must match the agreement line in the
`eval-run.txt` you committed** — that file is the record of your final run.]

Run 1:
item    |  gold |   verdict | agree  |note|
|---|---|---|---|---|
issue-01 | accept  |reject  | NO    | failed: scope_small, newcomer_signal (preferred)
issue-02 | reject | reject  | yes    |
issue-03  |reject | reject  | yes    |
issue-04  |accept | reject  | NO  |   failed: scope_small, clear_acceptance
issue-05  |reject | reject |  yes |   
issue-06  |accept  |reject   |NO     |failed: repo_in_use
issue-07  |reject  |reject   |yes    
issue-08  |reject | reject |  yes    
issue-09 | accept | reject |  NO    | failed: maintainer_active
issue-10  |reject  |reject  | yes    
issue-11 | accept | reject  | NO  |   failed: scope_small, newcomer_signal (preferred)
issue-12 | reject|  accept  | NO  |   graded accept
issue-13  |reject| reject  | yes    
issue-14|  accept | accept|   yes    
issue-15  |reject |accept  | NO     |graded accept
issue-16 | accept | accept |  yes    
issue-17 | reject | reject | yes    
issue-18  |reject | reject |  yes    
issue-19 | accept  reject|   NO |    failed: scope_small, clear_acceptance, newcomer_signal (preferred)
issue-20 | reject  |reject|   yes    

categories: claimed 4/4  clear-accept 2/8  dead-repo 3/3  policy 0/1  scope 3/4
agreement: 12/20 scored items  (bar: 18/20: below the bar; category floor unmet: no match in policy)


Run 2 (partial run on disagreements):
- Changed maintainer active window from 30 to 90 days.
- repo_active window is 90 days instead of 60.
- repo_in_use removed forks and dependents.
- reads PRs mentioned in comments.
- added AI policy check (must allow AI usage)
grading 8 bundle(s) with rubric.md, model sonnet, 5 worker(s)...
  issue-06: accept
  issue-11: accept
  issue-04: accept
  issue-09: accept
  issue-01: reject
  issue-12: reject
  issue-15: reject
  issue-19: reject

item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: scope_bounded, newcomer_signal (preferred)
issue-04  accept  accept   yes    
issue-06  accept  accept   yes    
issue-09  accept  accept   yes    
issue-11  accept  accept   yes    
issue-12  reject  reject   yes    
issue-15  reject  reject   yes    
issue-19  accept  reject   NO     failed: scope_bounded, newcomer_signal (preferred), clear_acceptance (preferred)

agreement: 6/8 scored items

Run 3 (full run, check):

item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: scope_bounded, newcomer_signal (preferred)
issue-02  reject  reject   yes    
issue-03  reject  reject   yes    
issue-04  accept  accept   yes    
issue-05  reject  reject   yes    
issue-06  accept  accept   yes    
issue-07  reject  reject   yes    
issue-08  reject  reject   yes    
issue-09  accept  accept   yes    
issue-10  reject  reject   yes    
issue-11  accept  accept   yes    
issue-12  reject  reject   yes    
issue-13  reject  reject   yes    
issue-14  accept  accept   yes    
issue-15  reject  reject   yes    
issue-16  accept  accept   yes    
issue-17  reject  reject   yes    
issue-18  reject  reject   yes    
issue-19  accept  reject   NO     failed: scope_bounded, newcomer_signal (preferred), clear_acceptance (preferred)
issue-20  reject  accept   NO     graded accept

categories: claimed 4/4  clear-accept 6/8  dead-repo 3/3  policy 1/1  scope 3/4
agreement: 17/20 scored items  (bar: 18/20: below the bar)

Final run:
- updated scope_bounded condition in rubric
  
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: scope_bounded, newcomer_signal (preferred)
issue-02  reject  reject   yes    
issue-03  reject  reject   yes    
issue-04  accept  reject   NO     failed: scope_bounded, clear_acceptance (preferred)
issue-05  reject  reject   yes    
issue-06  accept  accept   yes    
issue-07  reject  reject   yes    
issue-08  reject  reject   yes    
issue-09  accept  accept   yes    
issue-10  reject  reject   yes    
issue-11  accept  accept   yes    
issue-12  reject  reject   yes    
issue-13  reject  reject   yes    
issue-14  accept  accept   yes    
issue-15  reject  reject   yes    
issue-16  accept  accept   yes    
issue-17  reject  reject   yes    
issue-18  reject  reject   yes    
issue-19  accept  accept   yes    
issue-20  reject  reject   yes    

categories: claimed 4/4  clear-accept 6/8  dead-repo 3/3  policy 1/1  scope 4/4
agreement: 18/20 scored items  (bar: 18/20: PASS)
run written to eval-run.txt

**Issue analysis**
issue-01 (conda/conda#16475, "Add permanent docs for installing PyPI packages with conda install"). My rubric decided reject; the gold label is accept. Every required check passed except scope_bounded, which the grader graded fail. It was reading the issue's "Proposed changes" section, which has separate headings for a new task page and for updates to manage-pkgs.rst, pip-interoperability.rst, new-features.md, and an optional troubleshooting.rst entry. My rubric's umbrella condition said "the issue is itself an umbrella or tracking issue ", and five headings matched "a checklist of separate deliverables." The gold label treats the issue as one bounded docs task: a single goal (a permanent home for one workflow) where the other headings are edits pointing readers to the new page, and the issue never calls itself an umbrella, has no tracking label, and links to no separate issues. My check counted headings and did not ask whether the list was meant to be split, which is the question the evidence guide's umbrella condition poses.

**Check rationale**

| ai_policy_allows | "contribution policy" line under Repo facts (CONTRIBUTING.md, AI policy files, PR/issue templates) | Fail only if the policy outright bans AI-generated or AI-assisted contributions. Conditions (disclosure, personal understanding, testing, human review) pass. No stated policy passes. | required |

Since this course is AI-assisted, this check verifies that the repo allows contributers to use AI-generated or assisted contributions.

**Trade-offs**

[What the quoted check gives up. Any one of these is a complete answer: an issue whose
result it changes, a canary you re-ran with `--only`, a case you accept it will miss, or a
stated reason nothing changed elsewhere. "Nothing changed, and here is how I know" earns
the point in full when the reason follows.]

The quoted ai_policy_allows check gives up what it can't see. It reads only the "contribution policy" line in the bundle, so a ban stated somewhere the bundle doesn't quote (a linked doc, a PR template) would pass. Adding it changed issues 12 and 15 from accept to reject, both matching the gold label. Its "silence passes" rule means a repo that never mentions AI is accepted, which I accept because the evidence guide says silence is not a restriction.

---

## Selection rationale

Graded on whether all three are answered, in your own words. Not on how good the
reasoning is, and not on length — a short honest answer to each earns the full marks.
This is also the basis for the claim comment you write in Unit 2.

**Selection rationale**

[Answer all three:

1. The issue's fit to your interests and to the time available.
2. What the verdict identified correctly, and what you weighed that the rubric could
   not.
3. The anticipated difficulty in claiming it.]

The issue fits my interests in RAG and AI platform engineering. I verified that it fit my interests, and the verdict identified this correctly. It also identified that it was a good first issue, no AI policy, and no assignee. I also weighed the difficulty of the issue, which I felt was within my ability.

It may be difficult to claim, there is already a comment on the repo.

---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/issue-select/`.
