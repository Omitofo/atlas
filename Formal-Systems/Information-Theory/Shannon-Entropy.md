---
title: Shannon Information Theory / Entropy
aliases: [Shannon Entropy, Information Theory]
tags: [principle, information, entropy, computer-science]
domain: Formal-Systems
subdomain: Information-Theory
authors: [Claude Shannon]
year: 1948
status: stable
related: [Second-Law-of-Thermodynamics]
---

# Shannon Information Theory (Entropy of Information)

## One-sentence definition
> Information can be quantified; the entropy of a message measures the average uncertainty or the minimum number of bits needed to encode it, setting fundamental limits on compression and reliable communication.

## Full explanation
Claude Shannon defined the entropy of a discrete random variable \( X \) as \( H(X) = -\sum p(x) \log_2 p(x) \). This quantity is the average information content per symbol and the lower bound on the average number of bits needed to encode messages from that source. Channel capacity theorems give the maximum rate at which information can be transmitted reliably over a noisy channel. The theory created the mathematical foundation for all digital communication, data compression, and coding.

## Feynman-style explanation
Imagine you want to send a message with the fewest possible yes/no questions (bits). If the message is completely predictable, you need almost no bits. If it is completely surprising, you need many. Shannon entropy tells you exactly how many bits, on average, are required. It also tells you how much noise you can tolerate before the message becomes unrecoverable.

## Key metaphors & analogies

1. **“Vng mñn”** — Removing vowels compresses the message; context (redundancy) still allows recovery.
2. **Dictionary of expected words** — Common messages get short codes; rare ones get long codes (like Huffman coding).
3. **Surprise meter** — The more surprising an event, the more information it carries.

## Concrete examples

1. **Data compression** — ZIP, JPEG, MP3 all approach (but cannot beat) the entropy limit of the source.
2. **Error-correcting codes** — Shannon’s channel coding theorem explains why we can send data almost error-free if we stay below channel capacity (used in deep-space communication, 5G, etc.).
3. **English language** — Entropy of written English is roughly 1–1.5 bits per character due to high redundancy.

## Quantitative / data anchors
- Entropy: \( H(X) = -\sum p_i \log_2 p_i \)
- Binary entropy function for a fair coin: 1 bit
- Channel capacity of a noisy channel: \( C = B \log_2 (1 + S/N) \) (Shannon-Hartley)

## Historical & discovery context
Shannon’s 1948 paper “A Mathematical Theory of Communication” founded the field. It was motivated by problems at Bell Labs on transmitting information over noisy telephone lines.

## Relationships

### Builds on / presupposes
- Probability theory
- Concept of information as reduction of uncertainty

### Influences / leads to
- All modern digital communication and storage
- Deep formal analogy with thermodynamic entropy
- Machine learning (cross-entropy loss, etc.)

### Contrasts with
- Semantic theories of information (Shannon deliberately ignored meaning)

## Common misconceptions
- “Information theory is about the meaning of messages.” → Shannon’s theory is about the statistical properties of signals, not semantics.
- “You can compress any file arbitrarily.” → Lossless compression cannot go below the entropy of the source on average.

## See also
- [[Science/Physics/Thermodynamics/Second-Law-of-Thermodynamics|Second Law of Thermodynamics]] (deep mathematical and conceptual links)

## Tags
#principle #information-theory #entropy #shannon #compression #communication