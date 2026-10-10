# Instinct Tasks

An independent, unofficial guide and task library. Not affiliated with Instinct. This repository does not contain or run an AI assistant.

**Browse the guide: https://instincttasks.com/**

This repository preserves a dated snapshot of the guide's public JSON feed, with 128 task records. Each record includes its source links, a task-page URL, evidence type, category, summary and update metadata. The guide has not independently reproduced the source reports or examples; inclusion is not proof of product capability.

## Read the snapshot

Open `tasks.json` in any JSON viewer, or inspect it locally with Python:

```python
import json
from pathlib import Path

snapshot = json.loads(Path("tasks.json").read_text())
for task in snapshot["items"]:
    print(task["title"], task["url"], task["sources"])
```

The snapshot is useful without an account or access to the underlying assistant: readers can browse task summaries, inspect evidence labels, follow public references and compare what each task asks a person to review. It contains published metadata, not private user tasks or execution logs.

## Provenance and updates

- Feed: https://instincttasks.com/api/tasks
- About and editorial scope: https://instincttasks.com/about/
- Source register: https://instincttasks.com/sources/
- Retrieved: 2026-10-10T06:41:45.513627+00:00
- Snapshot ID: `c7988f7b-e5d1-47cd-91a2-0cce59325b1e`
- Pagination: 7 responses, followed via `nextCursor`; 128 unique task IDs.
- `tasks.json` SHA-256: `bb26b72b6d11d463570d18ba847c3b5fb54f11dc5cdb77b4ac991a3d69834c8d`

This is a fixed snapshot, not an automatically synchronized mirror. Visit the guide for current pages, prompts and approval boundaries. Source labels distinguish official product examples from community reports; neither implies an independent test by this guide.

## Attribution and rights

Source URLs are retained for attribution and verification. Third-party source material and trademarks belong to their respective owners. No blanket open-source or dataset license is asserted for those materials. This repository is a reference snapshot, not an endorsement or an official product distribution.
