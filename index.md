---
layout: base
title:  'Akkadian UD'
udver: '2'
---

# UD for Akkadian <span class="flagspan"><img class="flag" src="../../flags/svg/IQ.svg" /></span>

## Tokenization and Word Segmentation

* In [RIAO](../treebanks/akk_RIAO/index.html), sentence boundaries were arrived at by syntactically annotating the unsegmented corpus, and identifying words that are head words but are not themselves dependents of other words. The separate trees produced this way were considered to be separate sentences.
* Words are only exceptionally delimited by whitespace or punctuation in the original cuneiform texts. Thus, this treebank is based on the bound transcription (normalized text).
* Enclitic pronouns and clitics are separated during tokenization and marked as multi-word tokens with a syntactic relation.

## Morphology

### Tags

* In [RIAO](../treebanks/akk_RIAO/index.html), 13 universal tags have been used. 
* The tags [AUX](...), [INTJ](...), [PUNCT](...), [SYM](...) are not used.
* The words tagged [PART](...) are the emphatic *lū*, the quotation particle *mā*, the clitics *ma* and *ni*, and the negation particles *lā* and *ul*.

### Nominal Features

* Nominal words are ([NOUN](...), [PROPN](...) and [PRON](...)) and adjectives ([ADJ](...))

For nouns, adjectives and non-finite verbal forms the subcategories are:
* [Case](...) has 3 possible values: Nom, Gen, Acc
* [Number](...) has 2 possible values: Sing, Plur
* [Gender](...) has 2 possible values: Masc, Fem
* [Base](...), which can have four different values:
  * free (status rectus),
  * bound (status constructus),
  * suffixal (followed by pronominal suffixes) and
  * terminal (status absolutus). 


### Verbal Features

In [RIAO](../treebanks/akk_RIAO/index.html), the following subcategories of verbs are annotated:
* Finiteness (Finite, Infinitive, Stative),
* Stem (G, D, Š, N, etc.),
* Mood (Indicative, Imperative, Precative, Prohibitive),
* Tense (Present, Past, Pgp), person (1, 2, 3),
* Number (Sing, Plur) and
* Gender (Masc, Fem).

Following Streck (2011: 363), we consider subordinative and ventive as subcategories of their own, which we tag as boolean values. 

## Syntax

### Word order
For the most part, Akkadian word order is SOV.

### Core Arguments, Oblique Arguments and Adjuncts
* Nominal subjects are in the nominative case without an adposition.

### Relations Overview

* The following relation main types are not used in this treebank: aux, clf, compound, cop, dislocated, expl, flat, orphan, punct, reparandum.
* The following relation subtypes are used in Akkadian:
  * acl:relcl for relative clauses
  * advmod:emph for the particle lū in its asseverative function
  * advmod:neg for the negation particles lā and ul
  * det:poss for possessive determiners
  * nmod:poss for the construct state

## Syntax

### Word Order
* The usual word order in Akkadian is SOV, but there are many exceptions to this generalization.

### Core Arguments, Oblique Arguments and Adjuncts
* Nominal subject is in the nominative case without an adposition.
* Prepositional objects are considered oblique.

### Relations Overview
* The following relation main types are not used in this treebank: [aux](...), [clf](...), [compound](...), [cop](...), [dislocated](...), [expl](...), [flat](...), [orphan](...), [punct](...), [reparandum](...).
* The following relation subtypes are used in Akkadian:
  * [acl:relcl](...) for relative clauses
  * [advmod:emph](...) for the particle *lū* in its asseverative function
  * [advmod:neg](...) for the negation particles *lā* and *ul*
  * [det:poss](...) for possessive determiners
  * [nmod:poss](...) for the construct state

## Treebanks

There are [2](../treebanks/akk-comparison.html) Akkadian UD treebanks:

  * [PISANDUB](../treebanks/akk_PISANDUB/index.html)
  * [RIAO](../treebanks/akk_RIAO/index.html)
