# CEP 2001: Knowledge Check Formatting and Style Requirements

## Abstract

This CEP documents the semantics, syntax and conventions associated with the format and style of knowledge checks in training and assessment modules. 

## Rationale

The aim of this CEP is to standardize the presence and the presentation of knowledge checks in training and assessment modules. Refer to other CEPs for a complete understanding of knowledge checks, including but not limited to, the formulation or construction of wording, point values, retry attempts and use of hints.

Note: Within the SimSpace Portal content creation interface, the task for a knowledge check is labeled "question", even though the knowledge check may not be worded as an actual question. This and related CEPs therefore use the term "knowledge check".

 "Presence" refers to the location of knowledge checks within a module, and how many are required.
 
 "Presentation" refers to the style format of knowledge checks.
 
 A knowledge check can contain various components. These are listed below and described in detail under **_Specifications_**.
 
A knowledge check _must_ include:
* The **request** to which the user provides a response.
* Instruction for how to provide the response.
 
 A knowledge check _may_ include the following items:
 * Scenario
 * Steps
 * Example response
 * Note
 
 Using these guidelines provides consistency in how knowledge checks are presented (or displayed). This allows the student to spend more of their time and effort focusing on the content and task, and less cognitive activity and time being spent on processing the mechanics of the knowledge check function.
 
Compliance with this convention facilitates programmatic identification of questions within modules. Using this CEP is critical to a unified user experience. 

## Specification

### What is a “knowledge check”

 A knowledge check is a sentence or phrase that requests information or knowledge about the content that preceded that knowledge check task. The components of a knowledge check are described below.
 
 #### Scenario
 A scenario describes a situation related to a knowledge check. A scenario precedes the request and is presented in the default paragraph format.

#### Steps
Steps describe specific actions the student must take in order to be able to respond to the request. A single step contains one and only one action. Steps precede the check and use the numbered list format.

#### Request
The actual **request** (question or action to which the student must provide an answer or response) uses the H2 style. (This style is bold, so it is not necessary to apply bold separately.) Because the request is bold, no other component of the knowledge check should be bold or use H2. The request is an independent paragraph, 1-2 sentences, maximum 120 works each. The request includes the instructions for providing a response.

#### Response/Answer Instruction
 The instruction is the method to submit a response, such as whether to select one or more of the available choices, or whether to enter text in a box. Authors should not assume that the method for providing a response is obvious. Examples of instructions are listed below.
* Select the answer that best describes ....
* Choose all of the options that apply.
* Enter the 4-digit value for ...
* Enter the name of the file, including the file type extension.
Request instructions may be presented as part of the request sentence or as a separate sentence (no new line). They use the H2 style.

#### Example Response/Answer
An example response is typically needed only for short answer requests, and then not always. An example response is presented on a new line, in parentheses,  preceded with a phrase such as "For example:" and uses the default paragraph style, italicized. Examples of example responses are provided below:
* _(For example: 1234)_
* _(For example: badfile.pdf)_ 
* _(Use this format: 000.000.000)_

#### Note
Notes should be used rarely. A note should be used only to add clarity to the knowledge check, but not be essential. It is not to be used to make a comment about the level of difficulty, to provide a tip or hint, or to remind the student about something. A note is a distraction. If used, a note is presented below the request (and example response, if used), separated by a blank line, preceded by "NOTE:" and uses the default paragraph style. 

### Requirements
- A training module must include X question tasks.

![test][C:\Users\laurie.hagar\Documents\How-to_Snaps\knowledge_check_sample.png]

## References and Footnotes

NOTE: The typical use for a note would be to explain point reductions. However, this may be able to be programmatically included.
NOTE: Not sure whether to enforce the "request" being phrased as a sentence with a question mark.
NOTE: What should be requirement for knowledge checks? Because modules may be constructed in various ways (mult chains, single chain with multi tasks, or multi chains and multi tasks, it's difficult to couch the requirement relative to chains/tasks. For example, can't say that the last task in a chain must be a question.)
