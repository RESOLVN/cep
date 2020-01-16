# CEP 2004: Question Retry Requirements


## Abstract

This CEP documents the semantics, syntax and conventions associated with question retries for assessment modules. 

## Rationale

This AIM of this CEP is to standardize the high-level structure around question retries implementation in assessment modules. If you violate these conventions it will not allow for easy programmatic identification of the retries in modules and degrade the value of questions in an assessment module . Following this CEP would be critical for accurate user assessment scoring and experience.  

## Specification


### What is a “Question Retry”?

A “Question Retry” is the number of attempts a participant is allowed for one question.

### Requirements

*  Questions with the Response Type “Multiple choice” should have at least 1 retry.
    *  True/False variations should not have a retry.
*  Questions with the Response Type “Short answer” should have at least 2 retries.
    *  State of case sensitivity is a factor to consider
*  Questions with the Response Type “Multiple select” should have at least 2 retries.

## References and Footnotes

Style Guide SimSpace CDEV - The "Specification" proposal text comes mostly from the original SimSpace Style Guide authored by Alissa Torres.

