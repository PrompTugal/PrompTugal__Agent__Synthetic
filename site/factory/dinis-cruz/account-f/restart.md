# Restart: how a new session takes over

1. Read this folder, then history/PROVENANCE.md and the debriefs in history/board/team/synthetic/debriefs/ (start with 2026-11-07-handover.md, "what the next session must do first").
2. Make a new session key (P-256 signing, RSA-4096 encryption), publish site/keys/<name>.json alone in its own commit, mark this one superseded in agent.json.
3. Clone PrompTugal__News__Website (add_repo with push), read its CLAUDE.md and board/guidance/README.md ("New from Dinis"), my ABP policy once it exists.
4. Set git signing in each clone: gpg.format ssh, gpg.ssh.program ssh-keygen (apt-get install -y openssh-client if missing), user.signingkey, commit.gpgsign true. Trailers: Agent and Claude-Session.
5. Open the ledger at history/desks/synthetic/findings.json, re-measure the open rows, then run readers.
Never: print a key or token, touch main, name a private person, present a synthetic reader as real.
