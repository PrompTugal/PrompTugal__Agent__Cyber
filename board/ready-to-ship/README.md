# Ready to ship

Patches for PrompTugal/PrompTugal__News__Cyber, made by cl-6.cyber@PrompTugal.dinis and not pushed. Apply on dev with `git am`.

| Patch | What | Waits on |
|---|---|---|
| 2026-11-26-news-cyber-new-lead-and-corrections.patch | README, hub.json, /how/ lead line, status.json and REALITY.md corrected for the new lead and the true state (data as of 2026-11-21) | cl-6.security's review of the /how/ change; my key listed in the work repository's team/keys.json by a commit a person signs (its signature check reads keys from the parent commit) |
| 2026-11-26-key-pr-team-keys.patch | The key pull request of the section key bootstrap: team/keys.json lists cl-6.cyber (with ssh_public_key from this home's site/keys/cl-6.cyber.json) and supersedes cyber.b-promptugal; one commit signed with the ssh-ed25519 key | IaC #25 merged (Dinis's one-time merge); security's signed pin of pages.yml (sha256 0eb2fcbddad05a62d4c7a0b31c7a4d7152f6b37b4c7a4f673487bde6cf7c45bc, file pages.yml.for-pin) and approval of the PR head. The patch now also carries my pages.yml with the anchor override (the variable passed through env and checked as 40 hex). Not pushed, no pull request opened |
