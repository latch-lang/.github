# Security policy

latch is a secure-logging language whose users rely on its guarantees, so we treat flaws in those guarantees as security issues, not just ordinary bugs.

## What counts as a security issue

- Anything that lets a latch program break a guarantee the documentation states: a secret reaching an output, I/O outside the declared capabilities, a record lost without being counted, tampering that the verifier does not detect, or untrusted input crashing a program.
- **Soundness bugs:** the checker accepting a program it should refuse, a gap between a proof and what the compiler actually does, or an assumption missing from the trusted-base register.
- Bugs in the compiler, runtime, standard modules, cryptographic integration, verifier, build and release process, or published artifacts.
- The website and the in-browser playground.

Ordinary bugs (wrong error messages, crashes of the compiler on bad input, documentation errors) go to the issue tracker once the repository is public.

## How to report

- **After launch (public repository):** use GitHub's private vulnerability reporting — the "Report a vulnerability" button on the repository's Security tab.
- **Now, and at any time:** email **latchlanguage@gmail.com** with a subject line starting `[security]`.
- Please do not open public issues, pull requests or discussions about a suspected vulnerability.

Please include: the latch version or commit, the profile (`rail`, `space`, `scada`, `ics` or default) and backend, a minimal program or input that shows the problem, what you expected, and what happened.

## What happens next

| Step | Target |
|---|---|
| Acknowledge your report | within 5 working days |
| Confirm or rule out the issue, and agree a severity with you | within 15 working days |
| Fix, release and publish an advisory | coordinated with you; normally within 90 days of the report, sooner if the issue is being exploited |

- Fixes are developed privately (in a temporary private fork when the repository is public).
- Each confirmed issue is published as a **GitHub Security Advisory**. GitHub is a CVE Numbering Authority, so confirmed issues receive a **CVE ID** through the advisory.
- Issues that affect a qualified long-term-support line are also issued as a **safety bulletin** to holders of that line, with the impact analysis and the regenerated evidence package.
- With your agreement, we credit you in the advisory.

## Supported versions

latch is pre-release; there are no supported versions yet. At the first release this section will list the current 1.x release line and each qualified long-term-support line with its support end date.

## No bug bounty

There is no paid bug bounty at this time.
