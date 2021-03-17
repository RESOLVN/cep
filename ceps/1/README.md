# CEP 1:  Purpose and Guidelines

## What is a CEP?

**Note: This will be implemented in CEP release version 1.0.0.** 

CEP stands for Cyber Education Proposal. CEPs are standards maintained by SimSpace and intended to provide guidelines for the design and style for content modules, learning delivery platforms and cyber ranges used in cyber education. Each CEP describes a component that can be included in these functions. The CEP specifies why and how a component is to be used.

SimSpace intends CEPs to be the primary mechanism for:
- proposing or modifying standards.
- collecting community feedback and ideas on issues.
- documenting design decisions.

CEPs are maintained as text files (with .md extension) in a public version control repository for optimal management.

Submissions and modifications for CEPs are done through a formal process that involves a delegate, an editor, and an advisory council. These roles and the process are explained in this document.
 
### CEP Types
 
There are three types of CEP:

-  **Features**: Describes a new feature or implementation for the learning delivery platform, or portal.
-  **Informational**: Describes a non-required design or process issue which currently lacks support to become a
 required standard. Content Developers are free to ignore or use them.
-  **Process**: Describes a process or style surrounding a content module or the delivery platform, or proposes a change to a current CEP style or process implementation. Examples include procedures, guidelines,
  changes to the decision-making process, and changes to the tools, environment or style used in content modules.

## CEP Roles

### CEP Audience

The primary audience for CEPs are the content developers for the SimSpace learning delivery platform. Content developers for the SimSpace commercial platform are required
to follow these guidelines in order to publish content of any type. These guidelines are critical for any content
development team or individual to document expected portal conventions and manage complex design problems that require
collaboration across multiple modules.

### CEP Advisory Council

The CEP Advisory Council is comprised of elected board members, who have the final authority whether a CEP will be accepted, rejected, removed or revised.

### CEP Editors

CEP editors manage the administrative aspects of the CEP workflow (outlined in this document). They assign numbers to CEPs and
 update the status of CEPs.

CEP editorship is by invitation from an existing editor. Editors can be contacted at ceps@simspace.com. Email communication would
 normally only be used to contact the editors semi-privately. All standard CEP workflow can be conducted via the GitHub
 CEP repository issues and pull requests.

#### CEP Editor Responsibilities

A CEP editor must have access and edit permissions to the Github repository. Normal correspondence between editors
happens in a semi-private shared Slack chat room “X Name”. Github issues and pull requests will be notified in
chat and be discussed when time permits for the CEP editors.

### Delegate
Delegates propose, support and shepherd a CEP through the workflow process. There are two types of delegates:
- The **core delegate** is responsible for creating, updating and collecting community feedback on ideas for the CEP.
- The **support delegate** works with the core delegate to approve the CEP for
submission.  

#### CEP Delegate Selection Process

The original author of the CEP is the core delegate. The core delegate can assign support delegate status at will.
A new core delegate can be assigned by the CEP Advisory Council in case the current delegate no longer has time or is
no longer available to manage the CEP.

If you are interested in the core delegate role for a CEP, you can submit a pull request with the core delegate
modification which can be reviewed by the CEP editors to decide if it passes the qualifications to be presented to the
CEP Advisory Council.

## CEP Workflow:
**Note: This Workflow will be implemented when CEP is ratified with the release of version 1.0.0.** 

The workflow outlined here is intended for building consensus based on community feedback and ideas while also documenting conflicting ideas. CEP
proposals that address functional gaps in SimSpace Portal or Cyber Range should be phrased as problem statements rather
than feature requests.

### Idea for a Content Module

The CEP process starts with a suggestion for a new standard. It is required that a single CEP contain only a single key
proposal. The more direct and to the point a CEP is, the more success it is likely to have for being approved. The CEP editors may reject CEP proposals if they seem too large in scope or contain more than a single idea.

Starting in the official CEP release version 1.0.0, each CEP proposal must have a support delegate and a core delegate. The
first goal is to determine if the idea is possible, and if it's optimal for cyber education. Posting in the shared
community Slack room is the required place to start in order to properly vet the idea.

Vetting an idea in a semi-public environment is intended to save the core delegate time from writing a CEP that is
 guaranteed to be rejected based on prior discussions. It's important to get feedback from the community first
  in order to build the best CEPs.

### Submitting a CEP

**Note: This will be implemented when CEP is ratified with the release of version 1.0.0.** 

In order for a CEP to be considered, it needs a CEP editor to agree to be a support delegate for it. The core delegate is the original
creator and author of the CEP. A support delegate can also be a co-author, but it isn't required.

Once the core delegate and support delegate agree, the CEP is ready to be reviewed by the CEP Advisory Council.
The process to submit the CEP is outlined in the next sections.

#### Stage 1: Submission

-  The CEP delegate forks the main CEP repository and creates a file named cep-9999.md that contains the new CEP. All drafts should use "9999"
-  In the Commit Message field, enter:
   - ` Type Header: [Features/Informational/Process]`
   -  `Status: Draft`
-  Push this commit to the Github fork and create a pull request

#### Stage 2: Validation

The CEP editors review the pull request for structure, formatting or errors.

-  The Title should accurately describe the content and idea.
-  The CEP style and language (phrasing, sentence structure), as well as the spelling, grammar and punctuation should be correct.
-  The CEP will be checked by Continuous Integration/Continuous Deployment (CI/CD) and must pass all checks to move to the Review stage.
-  When the CEP is validated, a new CEP number is assigned by the support delegate, who also creates a folder in the appropriate file structure.
   - A unique CEP number (Feature 0-999, Informational 1000-1999, Process 2000+).
   - Ideally the next available number under the assigned CEP type.

The support delegate (a CEP editor) should not unreasonably deny publication of a CEP. Their primary efforts are to ensure it is written appropriately and passes CI/CD. Reasons for denying CEP status can include duplication of effort, being technically unsound, not providing proper documentation or backwards compatibility.

#### Stage 3: Review

-  When the validation process is complete, the CEP editors will squash commit the pull request into master.
-  The final authority for a CEP approval is the CEP Advisory Council. A meeting takes place (insert time frame) in which the CEPs are voted on.
-  Voting on a single CEP can take place in a Slack chat.
-  A proposed CEP must be a clear and complete description of the proposed enhancement, as well as being technically and logically sound. The CEP must represent a net improvement. CEPs should not complicate the development process; they should add clarity to it.

#### Stage 4: Verdict

-  **Deferred**: This is the status of a CEP that has been denied and not in revision. The CEP delegate can re-assign it to a draft status if applicable.
-  **Rejected**: The final rejection of a specific CEP. The CEP can not be considered for approval again.
-  **Accepted**: The CEP is accepted and will be included in the next release of CEP standards.

## CEP Maintenance

**Note: This will be implemented when CEP is ratified with the release of version 1.0.0.** 

As the standard matures, the Features track updating should become rare and CEPs should no longer be modified after they
have been finalized. Once a CEP has been finalized, it will become the formal documentation of the expected
style and design.

Informational and Process CEPs will continue to evolve as format and features change. The exact process
followed in these proposals will depend on the context and nature of the CEP being updated.

### Updating CEPs and Reporting Bugs

For a CEP that has been implemented, a
Github issue is the proper process. Use the issue reporting template in the repository.

## What is in a Successful CEP

Each CEP should contain the following items:

-  **Abstract**: Brief summary of the CEP. Provides a concise overview in one or a few sentences. It says more than the title, but is not a repeat of the entire specification.
-  **Rationale**: Explains why the CEP is needed or is useful, or a problem that it solves.
-  **Specification**: Describes the CEP in detail. Includes explicit requirements and other information organized under sub-headings as appropriate. It may include examples and sub-headings such as:
   -  Definition
   -  Requirements
-  **References and Footnotes**: Any documents that were used in preparing the CEP, or which provide additional information. May indicate sources from which wording or descriptions were derived.
-  **License/Copy**: Apache 2.0 for SimSpace CEPs.
-  **Acknowledgements**: Gives credit to individuals or an entity that was helpful or inspirational in preparing the CEP.

### Auxiliary Files

**Required Version >= 1.0.0**

CEPs may include files such as diagrams, pictures, and supporting documents. Such files should use the naming convention:

    cep-xxxx-y.extension

 where `xxxx` is the CEP number, `y` is a serial number (starting at 1), and `extension`
is replaced by the actual file extension (Example: `.jpg`).

These files should be included in the CEP sub-folder. This is a suggested format and is not required for content module
certification.
