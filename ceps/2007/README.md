# CEP 2007: Module Image Requirement
## Abstract
This CEP documents the semantics, syntax and conventions associated with using images in training and assessment modules.
## Rationale
The aim of this CEP is to standardize how images are used in training and assessment modules in order to ensure consistency of user experience. By presenting images in a consistent manner within a module and across all modules, the student's learning process is not interrupted by adapting to changes in how images are used. An example is the ability to read information within an image without having to take any measures, physically (squinting or moving closer to the screen) or technically (magnification). Another way this is achieved is by being able to locate and/or identify the image that is being referenced within the text (such as the image caption) with a reasonable expectation that this method will be the same or similar in every instance.  

The actual manner of presentation is intended to be intuitive and simple -- an image and a caption with a figure number. The significant point is that presentation be consistent.

If you violate these conventions it will prohibit programmatic identification of the images and degrade the value of the module. Following this CEP is critical for a unified user experience.
## Specification
### What is a “Module Image”
A “Module Image” is any media item used within a content module task. The following list describes the semantics used for these media types.
* **Screen shot**. Snapshots taken by an author of an interface or screen display. This may include the entire interface/screen or a portion of it.
* **In-house illustration**. A picture created by a staff artist.
* **Stock graphic**. Pictures that come from an outside source, whether freely available or paid. These may include photographs, icons, cartoons.
* **Logo**. Pictures used as an official representation of a commercial brand, product, or organization. Examples are the apple image for Apple Inc., or emblems for branches of armed services.
* **Video**. A recording of moving images, often screen captures to demonstrate a feature or process. May include audio.
### Requirements
* Images must have a maximum width of 800 pixels.
    * Images must be created in the appropriate size, so that imagery and text will not be scaled down and rendered unreadable.  
    * Images must be created so that text and pictoral information can be read and seen without additional magnification.  
* All images used in tasks will have a caption with a sequential figure number, "Figure \[sequential number]\". The exception is the image used in the Module Introduction task.
* Images must not exceed a file size of 2.2 MB.
   * This restriction is based on current SimSpace portal restrictions.
* All images must have a copyright license agreement. (See footnote)
## References and Footnotes
* CEP for [Screen Snap Requirements](ceps/xxxx/README.md)  

Copyright: Process to be determined by which an author and/or illustrator  ensures that use of an image meets copyright or license permissions.

NOTE: Add links to related CEPs

NOTE: What about shrinkage when the screen in narrowed?