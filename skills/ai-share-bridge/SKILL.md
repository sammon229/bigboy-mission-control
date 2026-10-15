# ai-share-bridge

Use the canonical bridge at `C:\Users\danie\shared-ai-bridge` and `bridge_cli.py`. Read the AI Share `task_id`, claim/update/complete that same ID as `codex`, and write result artifacts to the appropriate bridge output. Never hand-edit SQLite. IDs stay `codex` and `hermes`.

AI Share is for bridge claims only; it is not the Kanban queue, Mnemosyne, or Obsidian. Preserve the handoff envelope fields when present: `conversation_id`, `task_id`, `agent_id`, `intent`, `context_query`, `memory_policy`, and `writeback`.

Canonical reporting fields are `agent`, `status`, `summary`, `artifacts`, `blockers`, `needs_dat`, and `timestamp`. BigBoy and MiuMiu read the same task record; private-chat completion is not authoritative.
