# Downstream modification notice

This package is a modified derivative of
[`GeiserX/cc-aws-keepalive` 0.5.0](https://github.com/GeiserX/cc-aws-keepalive/tree/v0.5.0),
distributed by the Awesome Claude Code Plugins marketplace as
`0.5.1-ccplugins.1` under GPL-3.0-or-later.

Changes made on 2026-08-12:

- emit proactive credential warnings through Claude Code's documented
  `systemMessage` hook response instead of successful-hook stderr;
- raise the `UserPromptSubmit` hook timeout in `hooks/hooks.json` from 10 to
  15 seconds;
- verify reactive auto-login through STS when no expiration field is configured;
- require verified SSH host keys by default, make trust-on-first-use explicit,
  and remove plaintext SSH-password support;
- support version-path updates from any Claude Code marketplace cache;
- document the aggregate-marketplace installation path and external Node.js 18+
  prerequisite; and
- add regression tests for these downstream integrations and security fixes.

Changes made on 2026-10-10:

- declare the license as `GPL-3.0-or-later` in `package.json`, `plugin.json`
  and the marketplace entry, matching the upstream project's current
  declaration.

The original copyright notices and GPL-3.0 license are retained in
[LICENSE](LICENSE).
