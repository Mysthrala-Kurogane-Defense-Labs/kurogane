# Public architecture boundary

The implemented example path is:

```text
Invented model → finite JSONL events → local schema validation → read-only report
                                     → Elixir event validation / dry-run preview
```

Optional Node-RED emits synthetic messages using builtin nodes. There is no public receiver, authenticated transport, protocol driver or production topology in these repositories. A hub-and-satellite design is conceptual until the actual components and versioned integration contract are reviewed.

For a real proposal, request source permissions, authentication, asset mapping, timestamps, data flows, queue bounds, acknowledgment semantics and recovery behavior. Record unanswered decisions. Use the [security trust-boundary guide](https://github.com/Mysthrala-Kurogane-Defense-Labs/kurogane-security-model/blob/main/trust-boundaries.md) to define evidence rather than treating this diagram as an implementation specification.
