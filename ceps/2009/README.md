# CEP 2009: Paragraph Requirements


## Abstract

This CEP documents the semantics, syntax and conventions associated with paragraph(s) in  training and assessment content modules. 

## Rationale

The aim of this CEP is to standardize the high-level writing structure of paragraph(s) in  training and assessment content modules. Adhering to these conventions allows for programmatic validation of the component and maintains the quality and integrity of the module. This CEP is critical for a unified user experience and engagement levels.

A paragraph is a single sentence or group of sentences that intentionally starts on a new line. A paragraph discusses a single idea. In some cases, a paragraph may consist of only one sentence.

###Paragraph Length and Format
Paragraphs may not exceed 150 words. Paragraphs should be comprised of about 1-6 sentences, with each sentence having about 5-30 words. In general, sentences should be kept short and to the point. Using these parameters, along with subheads, bulleted lists and other style formatting devices improves organizational structure, facilitates the ability to find information and creates visual appeal.

Paragraphs are to be separated by a blank line space.

#### Simplified Writing
Simplified writing does not mean writing in a "dumbed down" way. It means writing in a manner that is concise and direct and avoids superfluous words. Often the student or user just wants the essential information, written simply and briefly. Writing in this manner may conflict with a goal to write in a conversational tone. However, not everyone is capable of or adept at a conversational style of writing, and among those who are, different conversational tones can be the result. Standardizing on a simple and direct style of writing creates uniformity and consistency across the company's instructional modules. A secondary goal, but worthy of consideration, is to better meet the needs of an audience that may not be native English speakers.  

A conversational tone can be useful is some circumstances. For example, it may help the material to be viewed as more friendly and approachable. Therefore, it is suggested that it be used primarily in the Introduction task, or when describing real-life scenarios or an actual event. It is not necessary to give up all creative phrasing, but strive to keep it within the boundaries of short, direct and simplified sentences.

In the Plain Writing Act of 2010, the US government undertook to implement "plain language" that the public can understand and use. This initiative offers basic, common-sense guidelines. As part of this, each agency has prepared its own writing guidelines, including the Department of Defense. These sites are useful references for writers.

Additionally, the Simplified Technical English (STE) initiative was started in the 1980s by a consortium of European aerospace and defense organizations. This initiative recognized that English is the international language of science, technology and human relations, and is also the language of the aerospace and defense industry. As a result, STE aims to help the readers of English-language documentation understand what they read, particularly when they are non-native English speakers. It has since expanded globally and beyond the aerospace industry.

####Punctuation
Within a paragraph, sentences are separated with a single space. Where four or more items are separated by commas, consider whether using a bulleted list could be an option.

Do not use semicolons, and only rarely a colon, dash or ellipsis. In almost all cases, there are alternatives for those types of punctuation that express an idea more clearly. Using such punctuation can be a distraction, and is subject to improper usage.

####Verb Tense and Voice
Use present verb tense and an active voice.  
 No: "If no user is specified, the ssh command will attempt to ..."  
 Yes: "If no user is specified, the ssh command attempts to ..."  
 No: "It is responsible for bringing together all the hardware ..."  
 Yes: "It brings together all the hardwar e..."
 
####Adjectives
Avoid adjectives that refer to relative points in time.   
No: "**Current** versions of Windows ..."  
Yes: "Windows 8 and later ..."  
No: "**Modern** web browsers ..."  
Yes: "Since about 2010, web browsers ..."  
No: "The **next** release is expected to address this."  
Yes: "Release 4.0 is expected to address this."

Avoid superlatives that convey little or no real meaning.  
No: "This command can **vastly** reduce the time in takes to ..."  
Yes: "This command can save you time by not ..."  
No: "Running xyz command can take a **long** time, therefore ..."  
Yes: "Running xyz command often takes more than two hours, therefore ..."  

####Point of View
Point of view is also called "voice narrative" and refers to first-person, second-person or third-person pronouns. Examples are:
* First-person: I, we, us, my
* Second-person: You
* Third-person: They, he, she, it

As a general rule, use first-person sparingly and primarily in the Introduction task. Refer to the [Simplified Writing](#simplified-writing) section in this CEP for additional guidance.

The example below, which is both conversational in style and uses first-person tense, should be avoided:  
No: "Next, we will take a look at how such-and-such has impacted cyber attacks."   

Instead, use a sub-heading to introduce the 'next' topic and get right to the point:  
"Such-and-such has had an adverse impact on cyber attacks."

Another aspect of point of view puts a subtle pressure on the reader. This occurs in phrases such as "In the xyz window, you can see…" or "Remember to factor in ..." or "Recall that we previously discussed how ...". The reader may not see, may not remember and may not recall. 
 
Alternatives:
- "In the xyz window, there are ..."
- "Be sure to factor in ..."
- "A previous section described ..."

####Slang and Shortcuts
Avoid short-cut or slang-like versions of words such as demo, demoing, info. Better to say demonstrate, demonstrating, information.

Avoid idioms and expressions. ("A dime a dozen." A system that becomes "hosed". Things that are neat, cool, dope, whacked, wicked.)
 
Avoid making a noun into a verb, unless it has been widely accepted into the lexicon. Using "Google" as a verb is barely acceptable (depending on context). Better to say "Search for ..."

Avoid using shell commands as verbs within a complete sentence.  
No: "When you cd into the xxxx folder ..."  
Yes: "When you navigate to the xxxx folder ..."

Be wary of using sland and shortcuts the are common in military or government, but may not be prevalent in the private sector. If in doubt, don't use it, or define it first.

#### Abbreviations and Acronyms
It's acceptable to use acronyms if the meaning has been defined and the acronym will be used more than twice in the module. If more than three tasks separate the definition from a second use, redefine it.

Don't define an acronym if it won't be used again in the module.

Do not use "e.g.", "i.e.", and "etc." in instructional modules.

Be wary of using too many different acronyms within a module, especially if they are similar.

Be wary of using acronyms and abbreviations the are common in military or government, but may not be prevalent in the private sector. If in doubt, don't use it, or define it first.

## Specification

### What is a “Paragraph”

 A “Paragraph” is any sentence or group of sentences that starts on a new line.

### Requirements

* Paragraphs must not exceed 150 words.
* Within a paragraph, sentences must be separated by a single space.

## References and Footnotes

[Word Counter](https://wordcounter.net/blog/2016/01/07/10986_how-many-words-paragraph.html).

[Writing Style Guide](https://www.esd.whs.mil/Portals/54/Documents/DD/iss_process/Writing_Style_Guide.pdf?ver=2018-06-25-144030-870) PDF for U.S. Department of Defense.

[Plain Language Guidelines](https://www.plainlanguage.gov/guidelines/) in U.S. government writing.
