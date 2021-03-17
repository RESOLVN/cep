# CEP 2038: Images: Screen Snaps
## Abstract
This CEP documents the semantics, syntax and conventions associated with using author-created screen snaps in training and assessment modules. For general image requirements, refer to [CEP 2007: Module Image Requirements](https://github.com/Simspace/cep/blob/master/ceps/2007/README.md).

## Rationale

The aim of this CEP is to provide standards for using screen snaps within modules. Screen snaps are typically created by the author, and therefore are subject to variability in appearance. By specifying standards, this variability is reduced or eliminated, providing a consistent appearance. This creates a professional impression and lessens distractions created by having screen snaps that look noticeably different in ways that include size, embellishments or methods of highlighting areas of an image.

The term *interface*, as used here, is synonymous with the terms graphical user interface, user interface, GUI, or UI.
  
A *screen snap* may be variously referred to as screen capture, screencap, screenshot, screengrab, or other similar terms.
  
_Embellishments_ are visuals added to a screen snap by a drawing or illustration program, often to draw the viewer's attention to a particular area

Author-made image modifications are limited in order to maintain consistency in appearance and so that authors' time can be focused on written content. The following modifications may be made by authors:
* A red rectangle for the purpose of drawing the user's attention to an area that is discussed in the text.
* The blurring of identifying information.

Embellishments such as labels or arrows, other forms of highlights, or any other effects should be done by an on-staff illustrator. This is to maintain consistency and professional appearance, and for appropriate use of resource time.

SimSpace uses the third-party product Snagit (by TechSmith) for creating screen snaps. The  modifications that authors make can therefore be achieved using the same tools, thereby increasing the uniformity of appearance. 

All screen snaps should have a "drop shadow" effect, which can be applied using Snagit. It is incumbent on the author to apply this effect. If the author is unable or unwilling to do so, they should contact the team's illustrator or content development specialist for assistance.

Screen snaps that contain text pose a special problem in terms of readability. What may be readable to the author in the original interface often becomes unreadable in a module due to scaling and other variables. Therefore, when inserting a screen snap of a Command Prompt, PowerShell, Terminal or similar type of window, or of any other interface window, text must not display smaller than the default paragraph text in a module.

## Specification
### What is a "screen snap"
A screen snap is a snapshot taken of an interface within a software application, or of a whole or portion of the display on a computer screen.
  
Optional embellishments are limited to those listed below:
- An unfilled rectangle with 3-point line weight and red color value of 255-0-0.
- A blur effect to mask undesired identifying information. (A "blur" tool is available in Snagit.) If a blur tool is not available, mask the information using a filled rectangle with dark gray color value of 68-68-68.  

### Requirements

* Screen snap maximum width is 800 pixels.
* Text within image, after being inserted into a module, must not display smaller than default paragraph text in module.
* Screen snaps will have a drop shadow applied at the lower right corner, with a size of 8 and dark gray color value of 68-68-68.

## References and Footnotes

* [CEP 2007 for Module Image Requirements](../2007/README.md)  
