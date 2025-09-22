Act like a senior product manager and technical writer for developer tools. Your task is to update an existing roadmap (Markdown) after features have changed or shipped, by identifying what changed, comparing those changes to the current roadmap, and then recommending the single next feature to implement.

Objective:
1) Ingest the current roadmap and change sources.
2) Generate a concise diff of what changed.
3) Compare changes vs. the roadmap (what matched plan, slipped, or appeared unplanned).
4) Recalculate priorities and timelines.
5) Output a clean, standardized roadmap plus ONE next feature recommendation.

Roadmap Input (choose ONE):
A) Paste the current roadmap Markdown between the fences below.
B) Attach the roadmap file and list its name after ROADMAP_ATTACHMENT: (assistant should read the attachment).
C) Provide a public file location after ROADMAP_URL:.

Change Sources to Inspect (choose ANY; prefer attachments over URLs if both are provided):
- GIT_COMPARE_URLS: [list of compare links between tags/branches, e.g., .../compare/v1.2.0...v1.3.0]
- MERGED_PR_QUERIES: [optional text queries or links to PR filters, e.g., label:feature merged:>=YYYY-MM-DD]
- CHANGELOG_ATTACHMENTS / CHANGELOG_URLS: [CHANGELOG.md, release notes]
- ISSUE_TRACKER_QUERIES: [Jira/Linear/GitHub Projects filters or exports]
- COMMIT_RANGE: [from_sha → to_sha]
- DOCS_URLS: [specs/ADR links that changed]
- METRICS_URLS: [dashboards validating impact or usage]

Original Roadmap to update:
ROADMAP_ATTACHMENT: [optional-roadmap-file.md]
ROADMAP_URL: [optional-public-url]
CHANGE_SOURCES: [paste items from the list above]

```markdown
[PASTE CURRENT ROADMAP HERE OR LEAVE EMPTY IF USING ATTACHMENT/URL]
[PASTE RECENT UPDATES / CHANGELOG / METRICS HERE OR LEAVE EMPTY IF USING ATTACHMENTS/URL]