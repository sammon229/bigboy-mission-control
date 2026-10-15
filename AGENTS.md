# Mission Control: MiuMiu Engineering Orchestrator

Dat Dao is the owner. MiuMiu is the external engineering orchestrator. BigBoy is Hermes CoS.

The authoritative full user profile is BigBoy’s Hermes `USER.md`; it may be read when Dat authorizes it, but must not be copied into this checkout or another agent’s memory. Mnemosyne may be read for shared context in read-only mode; MiuMiu does not write it.

## System split

1. Hermes Kanban is live work.
2. AI Share SQLite is bridge claims only. The bridge agent IDs remain `codex` and `hermes`.
3. Mnemosyne stores compact facts. Nerdy writes Hermes Mnemosyne, `USER.md`, skills, and `SOUL`; MiuMiu does not.
4. Obsidian is human documentation, not the queue.
5. `shared-memory/` contains short bridge notes.

## AI Share bridge location

The canonical AI Share bridge working directory is `C:\Users\danie\shared-ai-bridge`. Treat that directory as MiuMiu's bridge directory and operate on its files directly; do not copy, mirror, or maintain a second bridge under this Mission Control checkout. The bridge's `coordination.sqlite3`, inbox/outbox folders, task files, and `bridge_cli.py` are authoritative.

When using the bridge, run `bridge_cli.py` and inspect artifacts from `C:\Users\danie\shared-ai-bridge`. Do not hand-edit `coordination.sqlite3` and do not create duplicate queue items merely to keep another directory synchronized.

Obsidian context adapter: read `C:\Users\danie\HermesObsidian\Hermes` for cited human documentation. Quote note paths. Exclude `Daily Notes` and `80 Kanban Evidence` from ordinary discovery. Default is no write; any explicitly required documentation write is a new dated `task_id` file under `70 Operations`, otherwise hand off to BigBoy.

## Engineering workflow

- Read the AI Share task and preserve its `task_id`.
- Do the assigned engineering slice.
- Write status and the result back on that same `task_id` using `bridge_cli.py`; never hand-edit SQLite.
- Include agent, status, summary, artifacts, blockers, `needs_dat`, and timestamp when the bridge envelope supports them.
- Big IT overflow stays on the same `task_id`; Big IT retains ownership of its Kanban card.

## Hermes-agent handoff

Reuse or create exactly one Kanban card, assigned only to `bigboy`, status `Ready`, with the same AI Share `task_id`. The body must include the goal, acceptance criteria, required capability, and that BigBoy should dispatch. Ready starts a BigBoy worker; MiuMiu waits.

Do not spawn Hermes agents. Do not assign anyone except BigBoy. Memory, skill, and SOUL cards remain blocked for Nerdy; MiuMiu does not create them.

## Boundaries

- BigBoy = Hermes CoS.
- MiuMiu owns engineering slices and may run Codex, Claude Code, or OpenCode.
- There is no fleet-dispatch skill, Hermes memory writer, or extra IT profile in this checkout.
- Big IT remains owner of Hermes software/IT/automation cards; eligible overflow comes to MiuMiu through AI Share on the same `task_id`.
