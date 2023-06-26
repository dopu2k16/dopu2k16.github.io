---
title: "IR-IITBHU at TREC 2016 Open Search Track: Retrieving documents using Divergence
From Randomness model in Terrier"
collection: publications
permalink: /publication/2017-02-16-trec
excerpt: ''
date: 2017-02-16
venue: 'The Twenty-Fifth Text REtrieval Conference (TREC 2016) Proceedings. NIST Special Publication:SP 500-321'
paperurl: 'https://trec.nist.gov/pubs/trec25/papers/IR-IITBHU-O.pdf'
citation: 'M. Niyogi, S. Pal. (2017). &quot;IR-IITBHU at TREC 2016 Open Search Track: Retrieving documents using Divergence
From Randomness model in Terrier.&quot; <i>The Twenty-Fifth Text REtrieval Conference (TREC 2016) Proceedings. NIST Special Publication:SP 500-321</i>.'
---

Abstract
======

In our participation at TREC 2016 Open Search Track which focuses on ad-hoc scientific literature search, we used Terrier,
a modular and a scalable Information Retrieval framework as a tool to rank documents. The organizers provided live data 
as documents, queries and user interactions from real search engine that were available through Living Lab API
framework. The data was then converted into TREC format to be used in Terrier. We used Divergence from Randomness (DFR)
model, specifically, the Inverse expected document frequency model for randomness, the ratio of two Bernoulli's processes
for first normalisation, and normalisation 2 for term frequency normalisation with natural logarithm, i.e., In_expC2
model to rank the available documents in response to a set of queries. Altogether we submit 391 runs for sites CiteSeerX
and SSOAR to the Open Search Track via the Living Lab API framework. We received an "outcome" of 0.72 for test queries
and 0.62 for train queries of site CiteSeerX at the end of Round 3 Test Period where, the outcome is computed as:
#wins / (#wins + #losses). A 'win' occurs when the participant achieves more clicks on his documents than those of the
site and 'loss' otherwise. Complete relevance judgments is awaited at the moment. We look forward to getting the users'
feedback and work further with them.

[Download paper here](https://trec.nist.gov/pubs/trec25/papers/IR-IITBHU-O.pdf)

Recommended citation: M. Niyogi, S. Pal. (2017). "IR-IITBHU at TREC 2016 Open Search Track: Retrieving documents using Divergence
From Randomness model in Terrier". <i>The Twenty-Fifth Text REtrieval Conference (TREC 2016) Proceedings. NIST Special Publication:SP 500-321</i>. 
