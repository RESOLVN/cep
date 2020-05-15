# CEP 2017: Module Naming and Format Requirements


## Abstract

This CEP documents the semantics, syntax and conventions associated with the title requirements for content modules of all types. 

## Rationale

The aim of this CEP is to standardize the structure, format, and content of module titles.

A module title is the name that represents a group of "chains" and "tasks" (the parlance used in the SimSpace Portal when creating content modules) and clearly states the main subject of the module.

If a program name and/or number is used as part of the title, it should precede the subject portion of the title and be separate with a colon and a space. Within SimSpace, it should be a rare use case where this is used as part of the actual module title. In general, such information may be stored as module metadata and combined with the actual title in a programmatic manner.

Titles may have a maximum of 65 characters, including spaces. This length provides optimal display in the SimSpace Portal.

When creating a title, avoid using puns or other creative wording if it obscures the clear meaning of what the module is about. A good litmus test is to consider whether the title could be translated to another language and maintain its meaning, or be readily understood by a user for whom English is a second language.

Avoid punctuation used in programming (\` \$ ' " \& \?  \@ \# \< \> \( \) \{ \} \[ \] \/ \\). The exception is if it part of a proper noun, such as in "ATT&CK".

As with most titles, use 'title case', which means to capitalize nouns, verbs, adjectives, adverbs, etc. Do not capitalize conjunctions, short prepositions, and articles. 
Here is a [quick resource for title case.](https://apastyle.apa.org/style-grammar-guidelines/capitalization/title-case)

If you violate these conventions it will impede search, retrieval, and adoption of content modules. Using this CEP is important for a unified user experience.

## Specification

### What is a “Module Title”

The module title is the name that represents the main subject of a group of chains and/or tasks. It may or may not include a program name and/or numbering scheme.

### Requirements

* Use title case.
* Do not use punctuation (unless in a proper noun).
* A task title has a 65 character or 12 word limit.

## References and Footnotes

APA.org - style and grammar guidelines