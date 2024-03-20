## _Nanopublications:_ rethinking global knowledge sharing

<br><br>

Tobias Kuhn, [Knowledge Pixels](https://knowledgepixels.com/)

**Metagov Seminar - 20 March 2024**

<small>These slides: [https://knowledgepixels.com/slides/metagov-nanopubs/](https://knowledgepixels.com/slides/metagov-nanopubs/)</small>

---

## <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 8 8" height="1ex"><path d="M5,8H8L3,0H0M8,4.8V0H5M0,3.2V8H3"/></svg>  What are Nanopublications?

- _Tiny packages of knowledge graph contributions_
- with provenance and metadata
- encoded in machine-interpretable language (RDF)

<img src="nanopub.png" height="250px">

<small>[https://nanopub.net/](https://nanopub.net/)</small>

---

## <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 8 8" height="1ex"><path d="M5,8H8L3,0H0M8,4.8V0H5M0,3.2V8H3"/></svg> Nanopublications

- _Can be about anything:_
  - e.g. domain-level links between genes/diseases/organisms/drugs/etc., data entries, metadata, reviews, comments, opinions, workflows, etc.
- Reliable hash-based identifiers and digital signatures
- Linked to their creators (e.g. via [ORCID](https://orcid.org/))
- Vocabulary terms can be defined on the fly if needed

---

## Vision: _Knowledge Space_

ecosystem for sharing knowledge much more efficiently

<img src="knowledge-space.svg" height="450px">

<small>[https://w3id.org/knowledge-space/](https://w3id.org/knowledge-space/)</small>

---

## Ecosystem of Services

<img src="network.png" height="250px">

- _Decentralized and open network of servers_
- Publishing layer: publish, retrieve, archive knowledge (ID-based lookup)
- Querying layer: access knowledge (complex queries via SPARQL etc.)

---

## Querying

<div class="container">

<div class="col">

_Query to network:_

    ?np np:hasAssertion ?assertion .
    graph ?assertion {
      ?assoc a
        biolink:OrganismTaxonToEnvironmentAssociation .
      ?assoc biolink:subject ?taxon .
      ?taxon biodiv:hasTaxonName ?taxonname .
      ?assoc biolink:predicate ?pred .
      ?association biolink:object ?env .
    }

<small>get all taxon-environment relations<br>(simplified example)</small>

</div>

<div class="col">

_Result from network:_

<img src="query.png" width="100%">
</div>

</div>

---

<img src="https://nanodash.knowledgepixels.com/images/logo.svg" height="150px">

- Web interface to _browse and search_ nanopublications
- and _publish_ nanopublications via template-based forms
- Connects to network of services (no local DB)

[https://nanodash.knowledgepixels.com/](https://nanodash.knowledgepixels.com/)

---

## Demo

Visit [https://knowledgepixels.com/nanopub-demo/](https://knowledgepixels.com/nanopub-demo/)

<img src="demo.png" height="500px">

---

## Thank you for your attention!

