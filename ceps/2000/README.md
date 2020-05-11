# CEP 2000: Learning Objectives

## Abstract

This CEP documents the semantics, syntax and conventions associated with Learning Objectives for instructional content modules. 

## Rationale

The aim of this CEP is to define what constitutes a learning objective and to standardize the presentation format and style for learning objectives in instructional content modules. A definition of learning objectives is important in order to distinguish them from learning _outcomes_ because the two terms are sometimes used interchangeably or have various other meanings attached to them.
 
 This CEP applies specifically to instructional modules, as opposed to assessment modules. An instructional module's primary purpose is to teach a topic, and includes definitions, explanations, best practices and/or examples.
 
 Objectives are the information that the module intends to cover, or what will be taught. They can serve as a high-level outline for the module, but should  be more than a list of one- or two-word topics. 

Objectives differ from outcomes in that they do not prescribe what the student should be able to _do_ at the conclusion of the module. Therefore, objectives do not use verbs that are observable or measurable terms, as would be used for outcomes, nor should they use verbs such as "to understand".)
  
Objectives are presented in a bulleted list format and use periods at the end even if each item is not a complete sentence. The use of a period is subjective, but it is based on the idea that a period completes a thought or idea. A lead-in sentence is not required for the list because the heading speaks for itself.  

Compliance with this convention facilitates programmatic identification of objectives within modules. Adhering to this CEP is critical to a unified user experience.

## Specification

### What is a “Learning Objective”

A  “Learning Objective” is one or more statements in the Introduction task about a topic or information that will be covered or taught in an instructional content module. A module can have one or more learning objectives. Each objective should be confined to a single idea. 

#### Examples of Learning Objectives

-  Introduce and explain numeric systems used in computing
-  How to use Wireshark to identify network traffic.
-  Explore the principles of basic network reconniassance.
-  Introduce the nmap tool.
-  How nmap can be used to ...
-  How to dissect specific protocol headers.

### Requirements
- A module will have a minimum of three (3) objectives.
- Objectives must be included in the Introduction task.
- Objectives are identified with an H3 title labeled "Learning Objectives".
- Objectives are presented in a bulleted list format.
- Each objective ends with a period.
- Each objective has a maximum of 120 characters.

## References and Footnotes
NOTE: Prefer to change this to just "objectives" or "goals" to help eliminate confusion between this and "learning outcomes". I think there are some business reasons for having both objectives and outcomes, and both can serve a purpose. But they also need to be distinctive, and having dissimilar labels will help to achieve that.  

NOTE: If certain components of assessment modules, of which this is one, will require unique CEPs, then the reference to assessment modules may be able to be removed from this.  

NOTE: Revisit the minimum of 3 objectives (reason for any minimums should be discussed in the rationale).  

NOTE: Why is there a 120-character limitation? (This should be stated in the rationale.)

