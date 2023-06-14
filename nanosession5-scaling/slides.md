## Scaling Nanopublications: Considerations on the Long and Short Run

_Tobias Kuhn_

Nano Session #5, 13 June 2023

---

## If successful, there will be MANY nanopublications

Barend Mons: _"we are talking about 10<sup>14</sup> nanopublications"_

<br>

### 100 000 000 000 000

<br>

(only Life Sciences; not including meta-level nanopublications like reviews etc.)

---

## Barend is always a bit ahead of time :)

Barend Mons (2016): _"we are talking about 10<sup>14</sup> nanopublications ... We are not there yet, but we have solved the main fundamental problems by now."_

---

## Ingredients for scaling

- Strong identifiers
- Immutability
- Breaking down the problem
- Distribution
- Redundancy

---

## Strong identifiers

- Handling 100 000 000 000 things needs _very solid methods to identify these things_
- Issuing of identifiers should not depend on single database (bottleneck)
- _Cryptographic hashes for identifiers:_
  - No bottleneck
  - Enforce immutability
  - Example: _Trusty URIs_

---

## Immutability

- _Seems to make problem worse:_
  - each update creates new thing ...
  - ... but full version history is good anyway! (see Git)
- _Further benefits:_
  - Efficient caching
  - Consistency is much easier to achieve (only adding, never deleting/updating data)

---

## Breaking down the problem

- Publishing servers:
  - _focus on publishing/archiving_
  - lookup by identifier
  - efficiently find updates since last visit
  - otherwise no query features at all
- Query servers:
  - _allow for (complex) queries_
  - rely on publishing servers (and other query services)
  - do not deal with publishing/archiving at all

---

## Distribution

- No single server needs to hold it all
- _Allow for distribution / federation / decentralization_
- For example, a (publishing/query) server should be able to only deal with the subset of nanopublications relevant to a given field

---

## Redundancy

- Harness openness:
  - Private data should be localized ...
  - _... but open data can be spread and copied!_
- Everything is available at multiple places
- Ideally, these places are _independent_:
  - with respect to hardware, software, and organization

---

## How to get there

- Scaling to 100 000 000 000 is a long path
- We won't get it right on the first try
- But we can agree on _principles_ that lead us there

---

## Principles

- Agreed identifier and container formats _(nanopublications)_
- Decentralization as an _unstructured peer-to-peer network_
  - "Unstructured": nodes agree on interface, but not on behavior
  - New behavior can emerge gradually
- _Layers of services_
  - publishing / core queries / advanced queries

---

## Knowledge Space

More elaborate explanation of principles and vision:

https://w3id.org/knowledge-space/

---

## Short run

1. _Always consider long-run performance:_
   - According to principles
   - Such that it can evolve to scale
2. _Pay as you go:_
   - Fix performance problems where and when they occur
   - Because of 1, there is aways a solution
3. _On the short run, things are slower than what they could be:_
   - That's the price for being ready for the long run

---

## Thank you for your attention!

