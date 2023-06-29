---
title: "Neural Code Synthesis and Completion"
collection: talks
type: "Talk"
permalink: /talks/2021-08-25-msc-thesis-defense
venue: "Faculty of Mathematics and Computer Science, Heidelberg University"
date: 2021-08-25
location: "Heidelberg, Germany"
---

In my MS thesis, I presented my work on Neural Code generation from natural language and Neural code completion.

Goal
* Natural language to code translation
    * Aims to develop a versatile Seq2Seq architecture for both objectives of translating text to code (NL2Code) and of generating comments, docstring,  
  method documentation from source code input (Code2NL).
    * Aims to use various neural-based subword tokenizers to incorporate the
contextual embeddings of the input.
    * Aims at performing an ablation study to gauge the importance of the crucial
components of the developed AI system.
    * Aims to develop transfer learning and data augmentation techniques to generate
more diverse and accurate source code translations.
* Code completion
    * Aims to develop a novel RoBERTa based neural language model for source code.
    * Aims at investing the performance of the model for the fill-in-mask task and
compare the predicted masked tokens with the ground truth.


| **Models trained on Dataset/Augmented Datasets**                     | **Test BLEU** |
|----------------------------------------------------------------------|---------------|
| Seq2Seq-BART on 3$x$ size of CoNaLa dataset                          | 25.7710       |
| Seq2Seq-BART on 5$x$ size of CoNaLa dataset                          | 25.1601       |
| Seq2Seq-BART on CoNaLa dataset                                       | 24.2990       |
| Fine-tuned Seq2Seq-BART on CoNaLa,, pretrained on mined100k corpus   | 26.5379       |
| Fine-tuned Seq2Seq-BART on 3x CoNaLa, pretrained on mined100k corpus | **27.8235**   |
| Fine-tuned Seq2Seq-BART on 5x CoNaLa, pretrained on mined100k corpus | 25.3153       |
| Vanilla Seq2Seq on CoNaLa                                            | 13.3270       |
| Transformer-CoNaLa code tokenizer on CoNaLa                          | 15.3834       |
| Transformer-BPE on CoNaLa                                            | 19.3402       |
| Transformer-Unigram on CoNaLa                                        | 20.9678       |
| Transformer-WordPiece on CoNaLa                                      | 17.3237       |
| Seq2Seq-RoBERTa without pretraining                                  | 17.0032       |
| Fine-tuned Seq2Seq-RoBERTa on CoNaLa, pretrained on mined30k corpus  | 18.8853       |
| TranX on CoNaLa                                                      | 25.1050       |



<object data="https://dopu2k16.github.io/files/msc-thesis-mitodru-ppt.pdf" width="1000" height="1000" type='application/pdf'></object>
