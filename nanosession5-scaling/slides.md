## Scaling Nanopublications: Considerations on the Long and Short Run

_Tobias Kuhn_

Nano Session #5, 13 June 2023

---

## If successful, there will be MANY nanopublications

Barend Mons: _"we are talking about 10<sup>14</sup> nanopublications"_

<br><br>

### 100 000 000 000 000

---

## Barend is always a bit ahead of time :)

Barend Mons (2016): _"we are talking about 10<sup>14</sup> nanopublications ... We are not there yet, but we have solved the main fundamental problems by now."_

---

## Ingredients for Scaling

- Strong identifiers
- Immutability
- Breaking down the problem
- Distribution
- Redundany

---

## Strong identifiers

- Handling 100 000 000 000 things needs _very solid methods to identify these things_
- Issuing of identifiers should not depend on single database (bottleneck)
- Cryptographic hashes for identifiers:
  - No bottleneck
  - Enforce immutability

---

## Immutability

- Seems to make problem worse: each update requires creation of new thing
- ... but full version history is a good thing anyway (see Git)
- Further benefits:
  - Efficient caching
  - Consistency is much easier to achieve (only adding, never deleting/updating data)

---

## Breaking down the problem

- Separate publishing from querying

---

## Distribution

- No single server needs to hold it all

---

## Redundancy

- Harness openness
- Everything is available at multiple (independent) places

---

## How to get there

- Scaling to 100 000 000 000 is a long path
- We won't get it right on the first try
- But we can agree on _principles_ that lead us there

---

## Principles

- Agreed identifier and container formats (nanopublications)
- Decentralization as an unstructured peer-to-peer network
  - "Unstructured": nodes agree on interface, but not on behavior
  - New behavior can emerge gradually
- Layers of services: publish / core query / advanced query

---

## Short run

1. Always consider long-run performance:
   - According to principles
   - Such that it can evolve to scale
2. Pay as you go:
   - Fix performance problems where and when they occur
   - Because of 1, there is aways a solution
3. On the short run, things are slower than what they could be:
   - That's the price for being ready for the long run

