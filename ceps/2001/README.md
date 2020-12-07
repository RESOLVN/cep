# CEP 2001: Question Task Formatting
# CEP 2001: Knowledge Check Formatting and Style Requirements

## Abstract

This CEP describes the visual format to use for question task types in training and assessment modules. (For information about the number of question tasks, use of retries, hints and point values, refer to related "Question" CEPs.)

## Rationale

The aim of this CEP is to standardize on how question tasks are presented in terms of the content or information that is included in such a task, and the visual styles (such as bold) to use.

Refer to other CEPs for a complete understanding of question tasks, including but not limited to, the wording for various types of questions, formulation of questions, point values, retry attempts and use of hints.

Within the content creation interface of the SimSpace Portal, the "question" task type allows the author to choose a response type, and to insert correct and incorrect answers.

Using these guidelines provides consistency in how question tasks are presented (or displayed). This allows the student to anticipate a similar or common experience for all question tasks, instead of having to decode different approaches taken by various authors.

Compliance with this convention facilitates programmatic identification of questions within modules. Using this CEP is critical to a unified user experience.

NOTE: Question tasks used in instructional modules created by SimSpace use the prefix "Knowledge Check" in the task title. It is suggested to adopt this practice because not implies a review of knowledge or information presented previously, and while it does require a response, it may not phrased as a literal question.

## Specification

### What is a “question”

A question or "knowledge check" requests a response from the student. It may not literally use a question mark, but the student must respond in some manner in order to complete the module satisfactorily.

A question/knowledge check may contain the following components:
- Scenario
- An action
- Assignment
- An example response
- A note

The assignment is required. All other components are optional.

#### Assignment
Required. The **assignment** is the question or action to which the student must provide an answer or response.

Instructions should be presented as part of the assignment sentence or as a separate sentence in the same paragraph. The instruction provides the method for submitting a response, such as whether to select one or more of the available choices, or to enter text in a field. Authors should not assume that the method for providing a response is obvious. Examples of instructions are listed below.
* _Select the answer that best describes how to ...._
* _Choose all of the options that apply._
* _Enter the 4-digit value for ..._
* _Enter the name of the file, including the file type extension._

Use the H2 style. The assignment is the only component of the question task that uses H2. The assignment paragraph  contains 1-2 sentences, maximum 120 words each.

#### Scenario
A scenario describes a situation related to a question. A scenario precedes the request and uses the default paragraph format. It might be a brief story or incident that applies to the assignment.

#### Steps
Steps describe specific actions the student must take in order to be able to respond to the assignment. A single step contains one and only one action. Steps precede the assignment and use the numbered list format.

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