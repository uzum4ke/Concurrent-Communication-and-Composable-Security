# Concurrent Communication and Composable Security

These research notes develop a game semantics for multiparty communication protocols and build cryptographic extensions on that foundation. The semantics is non-probabilistic. It describes which interactions can occur, how events depend on one another, and what participants can observe.

Protocols are strategies on polarized event structures. Connecting two protocols matches events at their shared ports and hides the internal exchange. The distinction between a message and its transmission matters. If two sends carry the same payload, a protocol history can still record which send supplied a particular delivery. Scott-open predicates express observations supported by finite evidence, and discrete payloads recover ordinary messages and words.

The cryptographic extension uses the same interfaces to describe public information and private distinctions. A coalition’s view determines which assertions it can establish and which internal histories it cannot distinguish. Correctness and security give factorizations in opposite directions over the honest interface, with simulators that compose sequentially and in parallel.

Sections 2–5 develop the game semantics, communication, distributed control, and execution. Sections 6–8 cover cryptography, protocol evidence and policy, and finite verification. Worked examples include FIFO and lossy channels in Appendix A, and authenticated channels and threshold disclosure in Appendix B.
