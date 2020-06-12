# CEP 2004: Retry Requirements


## Abstract

This CEP documents the semantics, syntax and conventions associated with the number of retries for question tasks types in modules. 

## Rationale

The aim of this CEP is to standardize how retries are implemented for the various "response types" (Selections, Multiple Choice, Short Answer) in instructional and challenge modules. Using this convention allows for programmatic identification of the retries in modules, and contributes to the integrity and consistency of content across the these types of modules, as well as a unified user experience.

There are three response types used in instructional and challenge modules: Selections, Short Answer and Multiple Choice. By default, the retries field is set to zero, which means the user always has an initial attempt, and no more than that. Therefore, the number of total attempts the user has to submit a correct response is 1 + number-of-retries. All three response types must have at least one retry.

Guidelines about the structure and number of answer options are provided in CEP 2036, [Knowledge Checks, Instructional, Amount](ceps/2036/README.md). This may impact the number of retries. Too many retries could guarantee a certainty of a correct response. Therefore, it's important to consider whether the goal is to assess whether the student has acquired the desired knowledge and to score them appropriately, or whether the goal is that they actually do get to a correct response because it is necessary to move forward in the module. The latter circumstance is sometimes the case in challenge modules. The number and nature of Hints is intertwined with retries ([Question Hint Requirements](ceps/2034/README.md)).

## Specification


### What is a “Retry”?

A “Retry” is the number of attempts a participant is allowed after submitting a first response that is incorrect.

### Requirements

*  Selections responses must have at least 2 retries.
    * Challenge modules with more than 10 answer options might have upwards of 10 retries.
*  Short Answer responses must have at least 2 retries.
    *  State of case sensitivity is a factor to consider.
*  Multiple Choice responses must have at least 1 retry.
    *  True/False variations should not be used, but if so, must have no retry.

## References and Footnotes

* CEP 2036 for [Knowledge Checks, Instructional, Amount](ceps/2036/README.md)
