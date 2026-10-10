# File and Module Audit

Use one row per meaningful candidate. Never treat a candidate as safe to delete until references and runtime discovery paths have been checked.

| Path/module | Current purpose | Action | Evidence/callers/symbols | Confidence | Risk | Target owner/path | Prerequisites | Validation | Rollback note |
|---|---|---|---|---|---|---|---|---|---|
| `path/to/file` | | KEEP / SPLIT / MERGE / MOVE / MIGRATE-THEN-REMOVE / DELETE / INVESTIGATE / ADD-BOUNDARY | | confirmed / likely / needs investigation | low / medium / high | | | | |

## Evidence checklist
- [ ] Static imports and exports checked
- [ ] Call sites and symbol references checked
- [ ] Dynamic imports/lazy routes/registry loading checked where relevant
- [ ] Test, fixture, script, build, package, deployment references checked
- [ ] Public API and downstream consumers considered
- [ ] Persistent data, generated code, and migrations checked
- [ ] Focused validation identified
