# CEP 2001: Knowledge Check Formatting and Style Requirements

## Abstract

This CEP documents the semantics, syntax and conventions associated with the format and style of knowledge checks in training and assessment modules. (For information about the number of knowledge checks, use of retries, hints and point values, refer to related knowledge check CEPs.) 

## Rationale

The aim of this CEP is to standardize on the presence and the presentation of knowledge checks in training and assessment modules. Refer to other CEPs for a complete understanding of knowledge checks, including but not limited to, the formulation or construction of wording, point values, retry attempts and use of hints.

Note: Within the SimSpace Portal content creation interface, the task for a knowledge check is labeled "question", even though the knowledge check may not be worded as an actual question. This and related CEPs therefore use the term "knowledge check".

 "Presence" refers to the location of knowledge checks within a module, and how many are required.
 
 "Presentation" refers to the style format of knowledge checks.
 
 A knowledge check can contain various components. These are described below under **_Specifications_**.
 
 Using these guidelines provides consistency in how knowledge checks are presented (or displayed). This allows the student to spend more of their time and effort focusing on the content and task, and less cognitive activity and time being spent on processing the mechanics of the knowledge check function.
 
Compliance with this convention facilitates programmatic identification of questions within modules. Using this CEP is critical to a unified user experience. 

## Specification

### What is a “knowledge check”

 A knowledge check is a sentence or phrase that requests information or knowledge about the content that precedes a given knowledge check task. The components of a knowledge check are described below.
 
 #### Scenario
 A scenario describes a situation related to a knowledge check. A scenario precedes the request and is presented in the default paragraph format. It might be a brief story or incident that applies to the assignment.

#### Steps
Steps describe specific actions the student must take in order to be able to respond to the assignment. A single step contains one and only one action. Steps precede the assignment and use the numbered list format.

#### Assignment
The **assignment** is the question or action to which the student must provide an answer or response. It uses the H2 style. The H2 style is bold, which distinguishes the assignment from all other components of the knowledge check. Therefore, no other component of the knowledge check should be bold or use H2. The assignment is an independent paragraph, 1-2 sentences, maximum 120 words each. The assignment includes the instructions for providing the response.

#### Response/Answer Instruction
Instructions may be presented as part of the assignment sentence or as a separate sentence in the same paragraph (using the H2 style). The instruction provides the method to submit a response, such as whether to select one or more of the available choices, or whether to enter text in a box field. Authors should not assume that the method for providing a response is obvious. Examples of instructions are listed below.
* _Select the answer that best describes how to ...._
* _Choose all of the options that apply._
* _Enter the 4-digit value for ..._
* _Enter the name of the file, including the file type extension._

#### Example Response/Answer
An example of a response is typically needed only for short answer assignment, and then not always. An example response is presented on a new line, in parentheses, preceded with a phrase such as "For example:", and uses the default paragraph style, italicized. Examples of example responses are provided below:
* _(For example: 1234)_
* _(For example: badfile.pdf)_ 
* _(Use this format: 000.000.000)_

#### Note
Notes should be used rarely. A note should be used only to add clarity to the knowledge check, but should not include essential information. It is not to be used to make a comment about the level of difficulty, to provide a tip or hint, or to remind the student about something. A note is a distraction. If used, a note is presented below the request (and example response, if used), separated by a blank line, preceded by "NOTE:", and uses the default paragraph style. 

### Requirements
* A module must include at least one question task (knowledge check).
A knowledge check _must_ include:
* The question task must have an **assignment** paragraph (to which the user provides a response), formatted with H2 style.
* The assignment must include instructions for how to provide the response.
 
 The following list contains optional components of a knowledge check:
 * Scenario
 * Steps
 * Example response
 * Note
 
## References and Footnotes

For a sample presentation of a knowledge check, see module: [A Sample Module for Formatting](https://portal.simspace.com/index.html#/catalog/content-modules/edit/module-9ca26d85-763c-4100-a63b-1202f6255b60/tasks/task-1f03f92a-83e8-498e-a6e2-5cc1830bc7c5), (first question task).