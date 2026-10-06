# latch

**A small, capability-secure language for logging and telemetry on embedded rail, space and industrial systems** — where a leaked secret, a runaway loop or an unbounded parser is not an option.

- **Safe by construction.** Every program declares what it may read and write; unvalidated input can't reach the wire; secrets can't be emitted directly; there are no unbounded loops, no recursion and no heap.
- **Machine-checked.** Core rules are proved in Coq, and a verified native RISC-V route ties compiled code to the official Sail specification model.
- **Evidence, not just logs.** Hash-chained, signed, gap-detectable record streams that an auditor can verify independently.

**Status:** pre-release. The source is not public yet; the website and first release are coming.

**Contact:** latchlanguage@gmail.com · Security reports: see [SECURITY.md](../SECURITY.md)
