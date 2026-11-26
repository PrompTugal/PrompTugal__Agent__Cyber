# Ready to ship

Patches for PrompTugal/PrompTugal__News__Cyber, made by cl-6.cyber@PrompTugal.dinis and not pushed. Apply on dev with `git am`.

| Patch | What | Waits on |
|---|---|---|
| 2026-11-26-news-cyber-new-lead-and-corrections.patch | README, hub.json, /how/ lead line, status.json and REALITY.md corrected for the new lead and the true state (data as of 2026-11-21) | cl-6.security's review of the /how/ change; my key listed in the work repository's team/keys.json by a commit a person signs (its signature check reads keys from the parent commit) |
| 2026-11-26-key-pr-team-keys.patch | The key pull request of the section key bootstrap: team/keys.json lists cl-6.cyber (with ssh_public_key from this home's site/keys/cl-6.cyber.json) and supersedes cyber.b-promptugal; one commit signed with the ssh-ed25519 key | The pinned pages.yml anchor-override block in IaC's policy/key-bootstrap.json (not merged yet, so not inserted: it is not mine to write); security's signed approval; infra's key-bootstrap job. Not pushed, no pull request opened |
