# CEP 2034: Question Hint Requirements
 
## Abstract

This CEP documents the semantics, syntax and conventions associated with question hint(s) for assessment modules. 

## Rationale

This AIM of this CEP is to standardize the high-level structure around question hint(s) implementation in assessment modules. Violation of these conventions will skew measurement of participant performance in assessments. Following this CEP is critical for a consistent and efficacious learner data footprint.  

## Specification

### What is a “Question Hint”

A “Question Hint” is a generic term and a synonym for “learning aid”. The Hint section contained in the details card in the content module task that a user can use for assistance on a question at the possible cost of point(s) or percentage value of points.

### Requirements

*  Questions must have at least one hint.
*  Content Modules should remain consistent with point reduction inside that module.
*  Actual hint deduction value can be determined by the content author within the criteria defined in the Learning Aid Type table that defines the four types of Learning Aids. 
*  User Assistance versus Learning Aids: Hint point deduction value of 0 is allowed only if related to the use of the platform and not the content of the assessment.
*  The number of hints allowed per question should remain consistent based on the question difficulty.
* If multiple hints are used, the following progression should be adhered to:
    * Level 1: General hint (what to research)
    * Level 2: A stronger hint that provides more refined research (specific document, website, book/chapter, video, etc.)
    * Level 3: The answer is encoded or obfuscated in some manner (XoR, Mod2, steganography, etc.)


## References and Footnotes

Style Guide SimSpace CDEV - The "Specification" proposal text comes mostly from the original SimSpace Style Guide authored by Alissa Torres.

