# Security improvement backlog

Recorded on 2026-11-10 after a preliminary static review. These are proposed improvements, not a complete security audit.

- [ ] Authenticate incoming local HTTP requests that modify state, including `/event`, `/permission`, `/usage`, `/quit`, and `/settings`. The current approval token authenticates responses to hooks, not incoming requests. Test missing, invalid, and valid tokens; update both Swift and Node hook installers.
- [ ] Verify downloaded release binaries before installation. Publish and validate checksums for integrity; evaluate signed artifacts or attestations bound to a trusted publisher identity for authenticity. Review ad-hoc signing and removal of the quarantine attribute.
- [ ] Make chat replies safer: verify the intended app remains focused before pasting and before Return, cancel on a focus change, and consider a paste-without-send option. App-level checks alone cannot distinguish terminal tabs or windows.
- [ ] Harden HTTP parsing and resource limits: reject invalid lengths, cap headers and bodies, enforce request timeouts and connection limits, and test malformed requests. Negative lengths are currently clamped to zero; browser-origin requests are already blocked.
- [ ] Add `SECURITY.md` with a private reporting channel, permission explanations, and the local trust model. Repository owners can evaluate private vulnerability reporting and repository security settings separately.

Validation should cover legitimate hook workflows and timeout/fallback behavior, without installing hooks into real user configurations during automated tests.
