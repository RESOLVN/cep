# CEP 2005: Introduction Task Requirement


## Abstract

This CEP documents the semantics, syntax and conventions associated with the module introduction card that is required for training and assessment modules. 

## Rationale

This aim of this CEP is to specify what information is to be included in the introduction task for all modules. Some categories of information listed here are detailed in their own individual CEPs, and links are provided.

The introduction is intended to prepare the student for the module. By indicating what the module will cover and what the student's outcomes should be, it enables the student to begin to assess what they already know and what they don't know, and become engaged in the topic.  

Use these conventions to allow for programmatic identification of the Introduction card in modules (and the sections in them). This CEP is critical for a unified user experience.  

## Specifications

### What is a “Module Introduction Card”

A “Module Introduction Card” is the first task in a content module. It provides an overview of the module and contains the components, described below, in the order they should occur.

#### Estimated time to complete
The estimated time it is expected to take to finish the module is displayed at the top of the body of the module, above the concept image. Eventually, this information will be programmatically derived from metadata. Therefore, the author needs to add this information as metadata, and also enter the content "Estimated time to complete: xxx"

#### Key Skills Needed
Key skills are the minimum skills that the user/student needs in order to do any activities in the module, and for which instruction is not otherwise provided in the current module. For example, if the user needs to navigate through a file system in a command or terminal window, they need to know commands such as `cd` and `ls`. Thus, "basic Command Prompt/Terminal window navigation commands" might be a key skill needed. If, however, a task in the module provides steps that include the `cd` and `ls` commands, the user does not need these basic navigation command skills.

The key skills do not need to be comprehensive. They do not need to include every conceivable skill that will be utilized. And higher level modules do not need to include every skill down to the foundational level. As an example, if network configuration is a key skill, it's not necessary to also list SSH, DHCP, routers, subnets, etc. The aim is to provide the student or user with a sense of whether they what they need to successfully complete the module. 

In instructional modules, a skills-needed list is useful when a sequential progression of  modules is not enforced. In this case, the list may indicate to the user that they need to first acquire another skill.

In challenge modules, there is usually an assumption that the user has a higher level of skills. Therefore, it may be sufficient to list skill _sets_, such as "Windows system administration".

#### Picture
The picture in the introduction is typically a conceptual image that represents the subject of the module. It can be an illustration, photo or other type of image. No header is required. 

#### Description
The description is a paragraph that provides a brief summary of the module. It should not be a rehash of the Topics list or Learning Outcomes. As a writing guideline, consider that this paragraph ought to be able to stand on its own (without topics or outcomes) and still provide the user with a solid idea of what will take place in the module. No header is required.

#### Topics, Learning Outcomes, Toolkit
See related CEPs. Each of these items requires an H2 header.

### Requirements

The information below must be included in the order listed. All are required unless stated otherwise.
* The task title box contains the verbiage "Introduction to \[module title\]".
* "Estimated time to complete: xxx" (no header)
* "Key Skills Needed" in H2 style.
* Picture (no header).
* Description, at least one paragraph (no header).
* "Topics" in H2 style.
* "Learning Outcomes" in H2 style.
* "Toolkit" in H2 style.

## References and Footnotes

* CEP 2000 for [Introduction Module Topics List](ceps/2000/README.md)
* CEP 2032 for [Learning Outcome Requirements for Instructional Modules](ceps/2032/README.md)
* CEP 2006 for [Module Toolkit Requirements](ceps/2006/README.md)