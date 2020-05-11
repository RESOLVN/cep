# CEP 2005: Module Introduction Task Requirement


## Abstract

This CEP documents the semantics, syntax and conventions associated with the module introduction card that is required for training and assessment modules. 

## Rationale

This aim of this CEP is to specify what information is to be included in the introduction task for all modules. Some categories of information listed here are detailed in their own individual CEPs, and links are provided.

The introduction is intended to prepare the student for the module. By indicating what the module will cover and what the student's outcomes should be, it enables the student to begin to assess what they already know and what they don't know, and become engaged in the topic.  

If you violate these conventions it will not allow for programmatic identification of the Introduction card in modules(and the sections in them) and degrade the value of module. Following this CEP is critical for a unified user experience.  

##Specifications

### What is a “Module Introduction Card”

A “Module Introduction Card” is the first task in a content module. It provides an overview of the module and contains various components, which are described below.
 #### Estimated time to complete
The estimated time it is expected to take to finish the module is displayed at the top of the body of the module, above the concept image. This information is programmatically derived from metadata. Therefore, while the author needs to add this information as metadata, they do not need to include any verbiage in the module related to the module duration.

#### Prerequisite Skills
Prerequisite skills are optional. They are minimum skills that the user/student needs in order to do any activities in the module, and which are not included in instructions. As a simple example, in an instructional module, if the user needs to navigate through a file system in a command or terminal window, they need to know basic navigation commands such as cd and ls. Thus, 'basic navigation commands' might be a prereq skill. If, however, the activity provides the necessary commands, they do not need to be considered a prereq skill.

Skills are optional because modules can serve different purposes. An assessment module, or one used for a CTF event, may not need to list skills. Skills, however, can be useful when a sequential progression of training modules is not enforced. In such a case, they alert the user to the skills that are necessary to be successful in the current module.

#### Picture
The picture in the introduction is typically a conceptual image that represents the subject of the module. It can be an illustration, photo or other type of image.  

#### Description
The description is a paragraph that provides a brief summary of the module. It should not be a rehash of the Learning Objectives or Learning Outcomes. Nonetheless, as a writing guideline, consider that this paragraph ought to be able to stand on its own (without objectives or outcomes) and still provide the user with a solid idea of what will take place in the module.

#### Objectives, Outcomes, Toolkit
See related CEPs.

### Requirements

The information below must be included in the order listed. All are required unless stated otherwise.
* The task title box contains the verbiage "Introduction to \[module title\]".
* "Estimated time to complete \[module title\]: xxx"
* (optional) "Prerequisite Skills"
* Picture
* Description of the module, at least one paragraph.
* "Learning Objectives" in H2 style.
* "Learning Outcomes" in H2 style.
* "Toolkit" in  H2 style.

The information below is optional. If used, it follows 'Estimated time to complete'.
* "Prerequisite Skills" in H2 style.

## References and Footnotes

* CEP for [Learning Objectives](ceps/2000/README.md)
* CEP for [Learning Outcomes](ceps/2032/README.md)
* CEP for [Toolkit](ceps/2006/README.md)