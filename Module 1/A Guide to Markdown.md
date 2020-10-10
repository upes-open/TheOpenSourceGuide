# A Guide to Markdown: The Formatting Language Of The Internet.


Let’s start with an **introduction** to make you well acquainted with the **language, it’s use and how to get started.**


	Markdown is a lightweight markup language with plain-text-formatting syntax, created in 2004 by John Gruber with Aaron Swartz. Markdown is often used to format readme files, for writing messages in online discussion forums, and to create rich text using a plain text editor.

	 While Markdown is a minimal markup language and is read and edited with a normal text editor, there are specially designed editors that preview the files with styles, which are available for all major platforms. Many general purpose text and code editors have syntax highlighting plugins for Markdown built into them or available as optional download. Editors may feature a side-by-side preview window or render the code directly in a WYSIWYG fashion.
> Doxygen

> RStudio

> Github Flavoured Markdown (GFM)

> Discount

> MarkAPL

> PHP Markdown

> Markdig 



	Now you might be wondering, why people use Markdown instead of WYSIWYG(What You See Is What You Get) editor? 
Some basic features that offer the advantage to Markdown over WYSIWYG editor are:
1.	Markdown can be used for everything. People use it to create websites, documents, notes, books, presentations, email messages, and technical documentation.
2.	Markdown is portable. Files containing Markdown-formatted text can be opened using virtually any application.
3.	Markdown is platform independent.
4.	Markdown is future proof. Even if the application you’re using stops working at some point in the future, you’ll still be able to read your Markdown-formatted text using a text editing application.
5.	Markdown is everywhere. Websites like Reddit and GitHub support Markdown, and lots of desktop and web-based applications support it.


I hope that you’re now well versed with the ability of this Language and hence without any further ado, we’ll dive into the basic syntax of Markdown. 

## Basic Syntax :

### Headings:-
*To create a heading, add number signs (#) in front of a word or phrase. The number of number signs you use should correspond to the heading level.*

For example:<br>
### Output:

# Heading level 1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;    Heading level 1

## Heading level 2 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Heading level 2

### Heading level 3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Heading level 3

#### Heading level 4 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Heading level 4

##### Heading level 5 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;   Heading level 5
  
###### Heading level 6 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Heading level 6

<br>
* NOTE: Markdown applications don’t always agree on how to handle a missing space between the number signs (#) and the heading name. For compatibility, always put a space between the number signs and the heading name.
<br>
<br>

### Paragraphs:-<br>
*To create paragraphs, use a blank line to separate one or more lines of text.*<br>
### Output: 

The UPES-OPEN community was created to                    
promote the use of open source softwares.                   
 <br>
*NOTE: Unless the paragraph is in a list, don’t indent paragraphs with spaces or tabs.<br>

### Line Breaks:-<br>
*To create a line break (<br>), end a line with two or more spaces but since it is hard to see trailing white spaces in an editor, you may want to use something other than trailing whitespace for line breaks. Fortunately, there is another option supported by nearly every Markdown application: the <br> HTML Tag.*
### Output: 
First line with two spaces after.        
And the next line.                          

First line with the HTML tag after.<br>  
And the next line.                        
<br>
<br>
### Bold:-<br>
*To bold text, add two asterisks or underscores before and after a word or phrase. To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.*
<br>
### Output: 
We are **UPES-OPEN**.                                                     
We are __UPES-OPEN__.                                                    
<br>
*NOTE: Markdown applications don’t handle underscores in the middle of a word very well. For compatibility, use asterisks to bold the middle of a word for emphasis.
<br>
<br>
### Italic:-
*To italicize text, add one asterisk or underscore before and after a word or phrase. To italicize the middle of a word for emphasis, add one asterisk without spaces before and after the letters. For compatibility, use asterisks to italicize the middle of a word for emphasis.*
<br>
### Output: 
We are *UPES-OPEN*.                                                       
We are _UPES-OPEN_.                                 
<br>
<br>
### Bold and Italic:-
*To emphasize text with bold and italics at the same time, add three asterisks or underscores before and after a word or phrase. To bold and italicize the middle of a word for emphasis, add three asterisks without spaces before and after the letters.*
<br>
### Output: 
One of the important benefits of                                     
open standards is ***Interoperability***.                            
<br>
<br>
### Blockquotes:-
*To enclose a segment of text in blockquotes, one must prefix each written line with a greater-than sign.*<br>

### Output: 	
>This is a blockquoted text.                                                          
>>This is nested blockquoted.                                                                   
<br>
<br>

### Horizontal rules:-
*You can create a horizontal rule by placing 3 or more hyphens, asterisks, or underscores on a single line by themselves. You can also place spaces between them.*<br>

### Output:
***
 
<br>
<br>

### Links:-
*To create a link, enclose the link text in brackets and then follow it immediately with the URL in parentheses.*<br>
### Output:
This is an [example link]( http://example.com/).                      
<br>
*You also have an option of adding a title for a link. This will appear as a tooltip when the user hovers over the link. To add a title, enclose it in parentheses after the URL.*
### Output:
This is an [example link]( http://example.com/ “with a title”).                      
<br>
<br>

### URLs and Email Addresses:-
*To turn a URL or email address into a link, simply enclose it in angle brackets.*<br>
### Output:
https://www.markdownguide.org         
 fake@example.com    
 <br>
 <br>
### Images:-
*To add an image, add an exclamation mark (!), followed by alt text in brackets, and the path or URL to the image asset in parentheses. We also have the option of adding a title after the URL in the parentheses.*
<br>
### Output:
![UPES-OPEN](open.png "OPEN SOURCE")
<br>
<br>

**Congratulations!**   You’re all set to try on working with this minimalist formatting  language, you’ve learned all the basics you need to get started.
If you enjoyed it and would like to dive deep into the intelligence of this language, here are some links to open source Markdown guides:
>https://www.markdownguide.org<br>
>https://guides.github.com/features/mastering-markdown

                                         



