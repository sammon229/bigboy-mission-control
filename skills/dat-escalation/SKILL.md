# dat-escalation

When blocked on Dat Dao, set the AI Share task status to `needs_dat` if the bridge supports it, preserving the same `task_id`. BigBoy pings Alerts. Do not create a second queue item or write Hermes memory. If the bridge CLI lacks `needs_dat`, record the blocker in the existing task note/output and escalate to BigBoy without hand-editing SQLite.
