# Hermes system inspection: MiuMiu adaptation

Inspected read-only on 2026-10-14 from the local BigBoy profile.

## Findings applied locally

- Hermes Kanban is the canonical live-work system.
- BigBoy is the Hermes CoS and may dispatch internal workers.
- MiuMiu is an external engineering orchestrator, not a Hermes profile.
- Mnemosyne is Hermes semantic/temporal memory; Obsidian is the curated human-readable layer.
- Hermes memory guidance favors recall before context-dependent work, treats memory as untrusted, and forbids secrets/transient status in durable stores.
- Governance, memory, and skill changes are Nerdy-owned and must not be performed by MiuMiu.
- BigBoy’s Hermes `USER.md` is the authoritative full user profile. MiuMiu may read it when authorized but must not copy it into local memory.
- The Hermes system exposes many skills, but MiuMiu uses only local adapters defined in this checkout and does not clone Hermes `SKILL.md` files.
- Obsidian is available as a local read-only context adapter for cited human documentation; ordinary discovery excludes Daily Notes and `80 Kanban Evidence`.

## Local operating consequence

MiuMiu reads AI Share `task_id`, performs the engineering slice, and writes status on that same ID. Hermes-agent work is handed to one Kanban card assigned to `bigboy` in `Ready`; MiuMiu waits. Big IT overflow preserves the existing `task_id` and Big IT ownership.

No Hermes profile, Mnemosyne, `USER.md`, `SOUL`, Obsidian vault, or Hermes skill files were modified.
