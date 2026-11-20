# Concurrent Communication and Composable Security

When a participant asks for the next reply in a protocol, has the ideal resource already disclosed enough for a simulator to produce it? These exploratory notes use category theory and concurrent games to study that question for multiparty communication.

The model records which events a reply depends on. Scott-open predicates on a coalition’s visible history describe what it can establish from finite evidence. In this symbolic model, security requires one simulator to reproduce the real protocol’s observable behaviour using the ideal interface. Simulators compose when protocols run in sequence or in parallel, including when an attacker interacts with both parallel components.

## Where to start

- **Section 4.2** develops streams of observable payloads and recovers finite words over a discrete alphabet.
- **Section 6** describes correctness and security as factorizations in opposite directions over the honest interface. Theorem 6.51 characterizes when a deterministic service’s future reply behaviour can be recovered continuously from its initial public disclosure.
- **Theorem B.44** gives a worked example. A simulator answers share requests before it learns the secret. At the threshold it learns the secret and interpolates a polynomial consistent with every share it has already issued.

