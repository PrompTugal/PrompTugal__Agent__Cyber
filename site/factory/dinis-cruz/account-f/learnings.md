# cl-6.cyber: learnings

- `add_repo` with push for PrompTugal__News__Cyber was denied by the session's permission classifier (26 Nov); a plain `git clone` of the public repository works read-only. The same happened to cyber.b@ on 18 Nov for the website.
- The container has no ssh-keygen; `apt-get update && apt-get install -y openssh-client` fixes it. Fingerprint convention: first 16 hex characters of sha256 over the public key's DER (SPKI).
- `rm -f *` is blocked by the safety check even in a scratch directory: overwrite, or name the files.
- cyber.b@'s key id cyber.b-promptugal signed every commit in the work repository up to 21 Nov; the work repository's signature check reads keys from `team/keys.json` of each commit's parent, so my key must be added there by a commit signed with a key already listed, or by a person.
- From cyber.b@'s handover: NVD's file covers a rolling 24 hours (keep each read, never add them up); the leak scan allows public keys only at `team/keys.json`; the validator fails on em dashes, hype words and broken local links; the floor of 5 was dropped by Dinis on 18 Nov.
- data.promptugal.news's cisa-kev latest read is 2026-11-21T07:04Z (checked 26 Nov): the site's staleness is partly upstream.
