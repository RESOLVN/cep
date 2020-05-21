# CEP 2010: Module Code Format and Style Requirements


## Abstract

This CEP documents the semantics, syntax and conventions associated with inserting code examples into text for content modules. 

## Rationale

The aim of this CEP is to standardize when and how to use the code style formats. Code styles display such text in a monospaced font to distinguish it from default text.

Use the inline code style when using a command or piece of programming language within a sentence.

Use the code block style, which starts a new line, when referring to a complete entry that one would make in a command window, or one or more lines of program code. A rule of thumb is that if the code contains a space, use a code block.

Do not include any instructions to the user in a code block. Instructions are always presented in default paragraph style, preceding the code block.

Be aware of the distinction between a tool and a code. An example is "nmap". References to the tool do _not_ use code style. But if referring to the actual `nmap` command, use code style.

Examples:
* Don't use code style: "Nmap is used to ..."  
* Use code style: "Use the `nmap` command to scan ..."
* Inline code: "In this section, the variable will be named `myvar`."  
* Code block: "To define the variable, enter:"  
```myvar = "abc"```

####Code Styles vs. Screen Snaps

Use code styles when you intend for the user to replicate the code exactly. The code style is usually easier to read for this purpose.
 
A screen snap is a better approach when you are providing an example of something that includes results or feedback, or that you don't expect the user to repeat verbatim. (Be sure to indicate that the image represents an example.) For screen snaps -- especially when extensive code is involved -- use the standards in [CEP 2038: Images: Screen Snaps](../2038/README.md) or [CEP 2007: Module Image Requirements](../2007/README.md).

If you want the user to enter a series of sequential commands or lines of code that you provide, present them as a numbered list that incorporates code style. (Depending on the nature of the steps, it may not be necessary to include an instruction such as "enter".)

Example:

1. Enter: `this`
2. Enter: `this` 
3. After you have the ip address, enter:  
 ```do this next thing```   

Adhering to these standards is important for a unified user experience.

## Specification


### What is “Module Code”

"Module Code” is any code-related content that is included as text inside the content module task. Code-related content is any part of a command line or a programming language.

Use the inline code style for single word code within a sentence.

Use the code block style for sample code the includes spaces.

### Requirements
*  All code text must use a code style format.

## References and Footnotes

[CEP 2038: Images: Screen Snaps](../2038/README.md)  
[CEP 2007: Module Image Requirements](../2007/README.md)