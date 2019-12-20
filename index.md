# ![UCCA logo](logo6.png) The UCCA Resource Webpage

Universal Conceptual Cognitive Annotation (UCCA) is a novel semantic approach to grammatical representation. It was developed in the Computational Linguistics Lab of the Hebrew University by [Omri Abend](http://www.cs.huji.ac.il/~oabend) and [Ari Rappoport](http://www.cs.huji.ac.il/~arir).

The central idea of the project is to analyze and annotate natural languages using purely semantic categories and structure (a graph). Syntactic categories and structure are not part of the manual annotation, and are ideally learned implicitly by the parsers. The basic set of semantic categories (the foundational layer) is inspired by work in linguistic typology, cognitive grammar, and neuroscience. The development of additional layers, such as semantic roles and super-senses (adapted from the [CARMLS project](https://github.com/nert-gu/streusle/)) is underway.

The annotation so far focused on argument-structure and linkage phenomena. We build primarily on _Basic Linguistic Theory_ (R.M.W. Dixon, 2010a; 2010b; 2012), a widely used approach for language description. We acknowledge that there many applicable analyses for a given sentence, but select, for practical reasons, a small set of highly useful distinctions, and apply them to provide one plausible annotation.

We have annotated 160K tokens from English Wikipedia with the UCCA scheme, as well as a 30K English-French parallel corpus based on Jules Verne's "20K Leagues Under The Sea", and a 120K tokens corpus of the entire book in German. Pilot studies were conducted on several other languages as well.

This page contains links to all of UCCA's resources: corpora, annotation guidelines, parser and code. If you use these resources in your research, please cite the following or other relevant [publications](#publications):

**Universal Conceptual Cognitive Annotation (UCCA)**  
[Omri Abend](index.html) and [Ari Rappoport](http://www.cs.huji.ac.il/~arir), _[ACL 2013](http://acl2013.org)_  
\[Paper: [pdf](papers/ucca_acl.pdf)\]

## Annotation Web-App

The UCCAApp web application for phrase-based annotation in general, and UCCA parsing in particular can be found here.

Formally, it supports DAG structures, discontiguous units and multiple categories.

The app supports configurable multi-layer annotation and task management, and is written in Django and AngularJS.

\[[Paper](#uccaapp)\] \[[Demo](http://ucca-demo.cs.huji.ac.il)\] \[[Code](https://github.com/omriabnd/UCCA-App)\]

## Guidelines

UCCA-annotated corpora include the guidelines version they were compiled with in their repository. The most up to date guidelines are available here (the most recent one is generally in draft mode, but see releases): \[[pdf](https://github.com/UniversalConceptualCognitiveAnnotation/docs)\].

## UCCA-Annotated Corpora

All publicly available with a [Creative Commons Attribution-ShareAlike 3.0 Unported](http://creativecommons.org/licenses/by-sa/3.0/) license. The guidelines with which each of them was annotated can be found in the repository.

*   English Wikipedia corpus: \[[github](https://github.com/UniversalConceptualCognitiveAnnotation/UCCA_English-Wiki)\]
*   English 20K Leagues Under The Sea corpus: \[[github](https://github.com/UniversalConceptualCognitiveAnnotation/UCCA_English-20K)\]
*   German 20K Leagues Under The Sea corpus: \[[github](https://github.com/UniversalConceptualCognitiveAnnotation/UCCA_German-20K)\]
*   French 20K Leagues Under The Sea corpus: \[[github](https://github.com/UniversalConceptualCognitiveAnnotation/UCCA_French-20K)\]
*   Excerpt of the PTB WSJ corpus: \[[github](https://github.com/UniversalConceptualCognitiveAnnotation/UCCA_English-WSJ)\]

## UCCA Parser

TUPA is a transition-based parser for Universal Conceptual Cognitive Annotation (UCCA), developed by Daniel Hershcovich, Omri Abend and Ari Rappoport. \[[Code](https://github.com/danielhers/tupa/)\] \[[Demo](http://www.cs.huji.ac.il/~danielh/ucca/)\]

## Source Code

Python source code for reading and manipulating the UCCA structures. The code was written by Amit Beka and Daniel Hershcovich. \[[Code](https://github.com/danielhers/ucca)\]

## Publications

**Multitask Parsing Across Semantic Representations.**  
[Daniel Hershcovich](http://www.cs.huji.ac.il/~danielh/), Omri Abend and [Ari Rappoport](http://www.cs.huji.ac.il/~arir). _[ACL 2018](http://acl2018.org) (long paper)._  
\[Paper: [pdf](papers/multitask_tupa.pdf)\] \[Supp. Material: [pdf](papers/multitask_tupa_supplementary.pdf)\] \[Code: [github](https://github.com/danielhers/tupa)\]

**Simple and Effective Text Simplification using Semantic and Neural Methods.**  
[Elior Sulem](http://www.cs.huji.ac.il/~eliors/), Omri Abend and [Ari Rappoport](http://www.cs.huji.ac.il/~arir). _[ACL 2018](http://acl2018.org/)_ (long paper).  
\[Paper: [pdf](papers/simplification_ucca.pdf)\] \[Data: [github](https://github.com/eliorsulem/simplification-acl2018)\]

**Reference-less Measure of Faithfulness for Grammatical Error Correction**  
[Leshem Choshen](https://ktilana.wixsite.com/leshem-choshen/) and Omri Abend. [NAACL 2018](http://naacl2018.org/) (short paper).  
\[Paper: [pdf](papers/uccasim_main.pdf)\] \[Supp. Material: [pdf](papers/uccasim_supplementary.pdf)\] \[Code: [github](https://github.com/borgr/USim)\]

**Semantic Structural Evaluation for Text Simplification**  
[Elior Sulem](http://www.cs.huji.ac.il/~eliors/), Omri Abend and [Ari Rappoport](http://www.cs.huji.ac.il/~arir). [NAACL 2018](http://naacl2018.org/) (long paper).  
\[Paper: [pdf](papers/samsa.pdf)\] \[Data & Code: [github](https://github.com/eliorsulem/SAMSA)\]

**A Transition-Based Directed Acyclic Graph Parser for UCCA.**  
[Daniel Hershcovich](http://www.cs.huji.ac.il/~danielh/), Omri Abend and [Ari Rappoport](http://www.cs.huji.ac.il/~arir). _[ACL 2017](http://acl2017.org) (long paper)._ Outstanding Paper Award.  
\[Paper: [pdf](papers/tupa.pdf)\] \[Supp. Material: [pdf](papers/tupa_supp.pdf)\] \[Code & Data: [github](https://github.com/danielhers/tupa/)\] \[[Demo](http://www.cs.huji.ac.il/~danielh/ucca/)\]

**UCCAApp: Web-application for Syntactic and Semantic Phrase-based Annotation.**  
Omri Abend, Shai Yerushalmi and [Ari Rappoport](http://www.cs.huji.ac.il/~arir). _[ACL 2017](http://acl2017.org) (demo paper)._  
\[Paper: [pdf](papers/ucca_app_demo_cameraready.pdf)\] \[Code: [github](https://github.com/omriabnd/UCCA-App)\] \[[Demo](http://ucca-demo.cs.huji.ac.il)\]

**The State of the Art in Semantic Representation.**  
Omri Abend and [Ari Rappoport](http://www.cs.huji.ac.il/~arir). _[ACL 2017](http://acl2017.org) (long paper)._  
\[Paper: [pdf](papers/sem_rep_survey.pdf)\]

**HUME: Human UCCA-Based Evaluation of Machine Translation**  
[Alexandra Birch](http://homepages.inf.ed.ac.uk/abmayne/), Omri Abend, [Ondřej Bojar](http://www1.cuni.cz/~obo/) and [Barry Haddow](http://homepages.inf.ed.ac.uk/bhaddow/), _[EMNLP 2016](http://www.emnlp2016.net/) (long paper)._  
\[Paper: [pdf](papers/hume.pdf)\] \[Data: [github](https://github.com/bhaddow/hume-emnlp16)\] \[[Demo](hume_demo.html)\]

**Conceptual Annotations Preserve Structure Across Translations: A French-English Case Study**  
[Elior Sulem](http://www.cs.huji.ac.il/~eliors/), Omri Abend and [Ari Rappoport](http://www.cs.huji.ac.il/~arir),  
_[ACL 2015 Workshop on Semantics-Driven Statistical Machine Translation (S2MT)](http://hlt.suda.edu.cn/workshop/s2mt/)._  
\[Paper: [pdf](papers/S2MT_paper.pdf)\]

**Universal Conceptual Cognitive Annotation (UCCA)**  
[Omri Abend](index.html) and [Ari Rappoport](http://www.cs.huji.ac.il/~arir), _[ACL 2013](http://acl2013.org) (long paper)_  
\[Paper: [pdf](papers/ucca_acl.pdf)\]

**UCCA: A Semantics-based Grammatical Annotation Scheme**  
Omri Abend and [Ari Rappoport](http://www.cs.huji.ac.il/~arir), _[IWCS 2013](http://www.ling.uni-potsdam.de/iwcs2013/) (long paper)_  
\[Paper: [pdf](papers/ucca_iwcs.pdf)\]

## Theses

**Measuring Semantic Preservation in Machine Translation with HCOMET: Human Cognitive Metric for Evaluating Translation**  
Pedro Marinotti, MSc Thesis,  
The University of Edinburgh, 2014  
\[Paper: [pdf](papers/pedro_thesis.pdf)\]

**Integration of a cognitive annotation into machine translation: Theoretical foundations and bilingual corpus analysis**  
[Elior Sulem](http://www.cs.huji.ac.il/~eliors/), MSc Thesis,  
The Hebrew University of Jerusalem, 2014  
\[Paper: [pdf](ucca/Elior_Sulem_thesis.pdf)\]

**Semi-supervised identification of scene-evoking nouns in UCCA**  
Amit Beka, MSc Thesis,  
The Hebrew University of Jerusalem, 2013  
\[Paper: [pdf](papers/beka_thesis.pdf)\]

**Grammatical Annotation Founded on Semantics: A Cognitive Linguistics Approach to Grammatical Corpus Annotation**  
[Omri Abend](index.html), PhD Thesis,  
The Hebrew University of Jerusalem, 2013  
\[Paper: [pdf](papers/omri_thesis.pdf)\]

## Reports

**Distinguishing Human Translations and Machine Outputs with UCCA**  
Michal Kessler, Lab Report,  
The Hebrew University of Jerusalem, 2019  
\[Paper: [pdf](ucca/michal_lab_summary.pdf)\]

## Contact

For any questions or feedback, please email Omri Abend at _oabend@cs.huji.ac.il_.
