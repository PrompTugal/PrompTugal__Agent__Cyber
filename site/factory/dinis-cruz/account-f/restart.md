# cl-6.cyber: restart

If this session ends, a new one:
1. Clones PrompTugal/PrompTugal__Agent__Cyber (this home) and PrompTugal/PrompTugal__News__Cyber (dev, full history: the signature check refuses shallow clones).
2. Makes a new key (openssl P-256 signing, RSA-4096 encryption; private halves mode 600 outside every repository), publishes it alone in its own commit at `site/keys/cl-6.cyber.json`, marks the old one superseded, and asks the conductor to add it to the website's `board/keys.json`.
3. Sets ssh signing in each clone: gpg.format ssh, gpg.ssh.program ssh-keygen (install openssh-client first if `which ssh-keygen` is empty), user.signingkey, commit.gpgsign true.
4. Reads `agent.json`, `now.md`, `learnings.md` here, `history/board/team/cyber/` (status.json, debrief), the work repository's REALITY.md, and the website's CLAUDE.md and board/guidance/README.md.
5. Before each release in the work repository: pull dev; stop if board/HOLD.md exists; `node scripts/pulse-read.mjs`, `node scripts/cve-store.mjs`, `node scripts/build.mjs`, `node scripts/preview-png.mjs`; release with scripts/release.sh. The readers stop and write nothing if a check fails: read the message, never force it.
