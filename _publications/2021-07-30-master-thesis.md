---
title: "Neural Models for Source Code Synthesis and Completion"
collection: publications
permalink: /publication/2021-07-30-master-thesis
excerpt: 'LLM (BART, RoBERTa, Transformer, GPT2) to translate natural language to source code snippet (NL2Code) and code completion system.'
date: 2021-07-30
venue: 'IWR, Heidelberg University, Germany'
paperurl: 'https://drive.google.com/file/d/1M3gXVON_-9NA401fOxY_mn30xVFuiPXT/view'
citation: 'Mitodru Niyogi. (2021). &quot;Neural Models for Source Code Synthesis and Completion.&quot; <i>IWR, Heidelberg University, Germany</i>.'
---
Abstract
=====
Natural language (NL) to code suggestion systems assist developers in programming Integrated Development Environments (IDEs)
by translating NL utterances into compilable code snippet. This facilitates the programmers to answer “how to” questions
while using a new language or API, without the need to adequately familiarize themselves with the new programming languages,
and the latest commonly used open source APIs. The development of these systems poses several challenges because of the 
lack of large (NL, code) annotated corpora, the misalignment between NL and code tokens, the syntactic and semantic
requirements of the target code, and its contextual dependencies.

The current approaches mainly involve hard-coded, rule-based systems based on semantic parsing. These systems make heavy
use of hand-crafted rules that map patterns in NL or elements in its syntax parse tree to various query constructs and
can only work on a limited subset of NL with a restricted NL syntax. These systems are unable to extract semantic
information from the coding intents of the developer, and fail to infer types, names, the context of the source code, 
and the developer’s intent to get accurate system-level code suggestions. Hence, these systems are non-scalable for 
real-time deployment.

In this master thesis, we present novel sequence-to-sequence deep learning models and training paradigms to map NL to 
general-purpose programming languages that can assist users with suggestions of source code snippets, given a NL intent,
and also extend auto-completion functionality of the source code to users while they are writing a code. These developed
architectures incorporate contextual awareness into neural models which generate source code tokens directly instead of 
generating parse trees/abstract meaning representations from the source code and converting them back to source code.

The proposed pretraining strategy and the data augmentation techniques improve the performance of the proposed architectures. 
An ablation study of the system was performed to gauge the important components of the developed AI system.
The proposed Seq2Seq-BART has been found to exceed the performance of a neural semantic parser, TranX, based on the BLEU-4
metric by 10.82%. Thereafter, a finer analysis for the parsable code translations from the NL intent for CoNaLA[^1] challenge
was introduced. The proposed system is bidirectional as it can be also used to generate NL code documentation given
source code. Lastly, a RoBERTa masked language model for Python code was proposed to extend the developed system for
code completion.

[^1]: https://conala-corpus.github.io/

[Download paper here](https://drive.google.com/file/d/1M3gXVON_-9NA401fOxY_mn30xVFuiPXT/view)

Recommended citation: Mitodru Niyogi. (2021) "Neural Models for Source Code Synthesis and Completion", <i>IWR, Heidelberg University, Germany</i>.
