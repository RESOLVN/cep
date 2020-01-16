# CEP 1:  Purpose and Guidelines

## What is a CEP?

**Note: This will be implemented in CEP release version 1.0.0.** 

CEP stands for Content Enhancement Proposal for the SimSpace style guidelines on content modules. A CEP is a design document providing information to the Content Development Community, or describing a new feature for the Portal, or it's processes and environments. The CEP includes a concise technical specification of the format and a logical rationale for its implementation.

SimSpace intends CEPs to be the primary mechanisms for proposing major new Content Module standards, for collecting community feedback and ideas on issues, and for documenting the design decisions that have gone into the Portal. The CEP delegate is for building consensus based on community feedback and ideas while also documenting conflicting ideas. CEP proposals that address functional gaps in SimSpace Portal or Cyber Range should be phrased as problem statements rather than feature requests. 

CEPs are maintained as text files(with .md extension) in a public version control repository for optimal management.

## CEP Audience

The primary audience for CEPs are the content developers themselves in the SimSpace Portal as a strict guideline to content modules for optimal experience of users. Content Developers on SimSpace Commercial Platform [only] are required to follow these guidelines in order to publish content of any type. These guidelines are critical for any content development team or individual to document expected Portal conventions and manage complex design problems that require collaboration across multiple modules.
CEP Types

**Note: This will be implemented in CEP release version 0.0.2.**
 
**Currently there are three types of CEP:**

-  A Features Track CEP describes a new feature or implementation for the SimSpace Portal.
-  An Informational CEP describes a non required design or process issue which currently lacks support to become a required standard. Content Developers are free to implement these ignore or use them.
-  A Process CEP describes a process or style surrounding the Portal or a Content Module, or proposes a change to a current CEP Style or Process implementation(not a change to the Portal). Examples include procedures, guidelines, changes to the decision-making process, and changes to the tools, environment, or style used in Content Modules.

## CEP CEP Advisory Council

**Note: This will be implemented when CEP release version 0.0.3.** 

Commonly there are a number of references in these CEPs to the "CEP Advisory Council". This refers to the current members of elected board members that have the final authority if a CEP will be accepted, rejected, removed or revised.

## CEP Editors

**Note: This will be implemented in CEP release version 0.0.3.** 

The CEP editors are responsible for managing the administrative aspects of the CEP workflow. They assign CEP numbers and update current status of them. See CEP Editors Responsibilities and Functions for more details.

CEP editorship is by invitation from a current editor and they can be contacted at ceps@simspace.com, however this would normally only be used to contact the editors semi-privately. All standard CEP workflow can be conducted via the GitHub CEP repository issues and pull requests.

## Starting with an idea for a Content Module

**Note: This will be implemented in CEP release version 0.0.3.** 

The CEP process starts with a suggested new idea for a Content Module. It is required that a single CEP contain one key proposal. The more direct and to the point a CEP is the more success it is likely to have. The CEP Editors reserve the right to reject CEP proposals if they appear too large in scope or contain more than a single idea.

Starting in the official CEP release version 1.x.x each CEP proposal must have a support delegate, and a core delegate. The core delegate is responsible for creating, updating and collecting community feedback on ideas for the CEP. The first goal is to determine if the idea is possible, and if it's optimal for content delivery. Posting in the shared community slack room is the required place to start in order to properly vet the idea.

Vetting an idea in a semi-public environment is intended to save the core delegate time from writing a CEP that is guaranteed to be rejected based on prior discussions . It's important to get feedback from the community on ideas first in order to build the best CEPs.

## Submitting a CEP

**Note: This will be implemented when CEP is ratified with the release of version 1.0.0.** 

In order for a CEP to be considered it needs another CEP editor to agree to be a co-delegate the CEP. The original creator and author of the CEP is the core delegate. A co-delegate works with the core delegate to approve the CEP for submission. A co-delegate can also be a co-author but isn't required.

Once the co-delegate and core delegate agree the CEP is ready to be reviewed by the CEP Advisory Council. The following process must be used to submit the CEP. 

**Standard CEP Submission Workflow:**

**Note: This Workflow will be implemented when CEP is ratified with the release of version 1.0.0.** 

### Stage 1: Submission

-  The CEP delegate forks the main CEP repository and creates a file named cep-9999.md that contains the new CEP. All drafts should use "9999"
-  In the Type Header field enter "Features Track", "Informational", or "Process" CEP
-  For the "Status" field use "Draft"
-  Push this commit to the Github fork and create a pull request

### Stage 2: Approval

-  The CEP editors review the PR for structure, formatting or other possible errors
-  Fully Complete, the proposal makes sense and is logically reasonable
-  Title accurately describes the content and idea
-  The CEP language(spelling, grammar, and sentence structure) and style(CEP approved) should be correct
-  The CEP will be checked by CI/CD and must pass all checks to be reviewed
-  Once approved, a new CEP number will be assigned

### Stage 3: Review

-  Once the approval process is complete by the CEP editors the CEP editors will squash commit the pull request into master
-  The CEP editors will not unreasonably deny publication of a CEP
-  Reason for denying CEP status include duplication of effort, technically unsound, not providing proper documentation or backwards compatibility.
-  The final authority for a CEP approval is the CEP Advisory Council. A meeting takes place (insert time frame) that calls a vote on CEPs
-  Expedited votes can be called to vote on a single CEP in slack chat
-  It must be a clear and complete description of the proposed enhancement. The CEP must represent a net improvement. The proposed CEP, if applicable, must be solid and must not complicate the content modules development process.

### Stage 4: Verdict

-  Deferred: This is the status of a CEP that has been denied and not in revision. The CEP delegate can re-assign it to a draft status if applicable.
-  Rejected: The final rejection of a specific CEP. In the rejected verdict case the CEP can no longer be considered for approval again.
-  Accepted: The CEP is accepted and will be included in the next release of CEP standards.

## CEP Maintenance

**Note: This will be implemented when CEP is ratified with the release of version 1.0.0.** 

As this documentation matures the Features track updating should become very rare and no longer be modified after they have reached the Final state. Once a CEP has been finalized, it will become the formal documentation of the expected format on a content module/feature.

Informational and Process CEPs will continue to evolve over time as format and features change. The exact process followed in these proposals will depend on the context and nature of the CEP being updated.

## What is in a successful CEP

**Each CEP should contain the following features:**

-  Abstract  (Required Version >= 0.0.2)
-  Rationale  (Required Version >= 0.0.2)
-  Specification  (Required Version >= 0.0.2)
-  Define the CEP
-  Requirements section
-  References and Footnotes (Required Version >= 0.0.2)
-  License/Copy (Required Version >= 1.0.0)
-  Acknowledgements  (Required Version >= 1.0.0)

## Auxiliary Files

**Required Version >= 1.0.0**

CEPs normally would include media files such as diagrams, pictures, and supporting documents. Such files should be named “cep-xxxx-y.extension” where "XXXX" is the CEP number, "Y" is a serial number (starting at 1), and "extension" is replaced by the actual file extension (Example: ".jpg").

These files should be included in the sub CEP folder. This is a suggested format and isn’t required for content module certification. 

## Updating CEPs and Reporting Bugs

For the early draft stages of a CEP the preferences will vary based on the owner delegate. If the CEP is finalized a Github issue is the proper process. Please use the included issue reporting template in the repository. 

## CEP Delegate Selection Process

The original author of the CEP starts as the core delegate. The core delegate can assign co-delegate status at will. A new core delegate can be assigned by the CEP Advisory Council in case the current delegate no longer has time or is no longer available to manage the CEP.

If you are interested in the core delegate role of a CEP, you can submit a pull request with the core delegate modification which can be reviewed by the CEP editors to decide if it passes the qualifications to be presented to the CEP Advisory Council.

## CEP Editor Responsibilities

A CEP editor must have access and edit permissions to the Github repository. Normal correspondence between editors will happen in a semi-privately shared slack chat room “X Name”. There Github issues and pull requests will be notified in chat and be discussed when time permits for the CEP editors. 

### New CEPs Process:

-  Ensure the CEP has a co-delegate and core delegate.
- Title represents the content and contains the core requirements.
- Read the CEP for completeness(spelling, grammar, sentence structure). It should be sound logical, and to the point. 
- The proposal should be technical sense even if it is accepted/rejected.
- Ensure unit tests pass on the CEP.

Once a CEP passes the basic checks the editor will start the assignment process next.

### CEPs Assignment Process:

- Assign a unique CEP number(meta cep 0-999, informational 1000-1999, process 2000+)
- Ideally the next available number under the assigned CEP type.
- Send informational email to core CEP delegate with next steps instructions. 
- Assign CEP to next 
