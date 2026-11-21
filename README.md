# TALS Editorial Tracker

Internal tracking repository for the editorial office of *Transactions on Applied
Language Systems* (TALS). One Markdown file per manuscript lives in `submissions/`,
named after the submission ID. The YAML front matter of each file is the record of
record for the manuscript's review state.

Field reference:

| field | meaning |
| --- | --- |
| `submission_id` | manuscript identifier used in all correspondence |
| `title`, `authors`, `corresponding_author` | bibliographic record |
| `article_type` | `research`, `survey` or `systems` |
| `submitted` | date the manuscript entered the system |
| `round` | current review round (starts at 1) |
| `status` | `under_review`, `major_revision`, `minor_revision`, `accepted`, `rejected`, `withdrawn` |
| `last_decision_date` | date of the most recent editorial decision, empty while undecided |
| `revision_due` | deadline for the current revision, empty when no revision is pending |

Weekly digests produced for the publisher are kept under `reports/`.
