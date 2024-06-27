What are HTML Entities?
 Ans : In HTML some characters are reserved like ‘’, ‘/’, etc. To use these characters in our webpage we need to use the character entities called HTML Entities. Below are a few mapping between the reserved character and its respective entity character to be used.
Character(<,>,&) - entityname(&lt,&gt,&amp) - entity number(&#60,&#62,&#38)

### What are different types of lists in HTML?
Ans : In HTML, there are mainly three types of lists: 
1. Ordered List (`<ol>`): This type of list is used when the items need to be numbered or ordered sequentially. Each item in an ordered list is marked with a number by default, but this can be customized using CSS if needed.
      <ol>
      <li>First item</li>
      <li>Second item</li>
      <li>Third item</li>
      </ol>
      
2.Unordered List (`<ul>`): This type of list is used when the order of items is 
not important. Each item in an unordered list is marked with a bullet point by 
default, but this can also be customized using CSS.
        <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        </ul>
        
3. Definition List (`<dl>`): This type of list is used to define terms and their 
corresponding descriptions. It consists of a series of term-definition pairs. 
Each term is enclosed in a `<dt>` tag, and each definition is enclosed in a 
`<dd>` tag

  <dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
  <dt>JavaScript</dt>
  <dd>A programming language used to make web 
  pages interactive</dd>
  </dl>
  
  
### Define multipart form data? 
Ans : Multipart form data is one of the values of the enctype attribute. It is 
used to send the file data to the server-side for processing. The other valid 
values of the enctype attribute are text/plain and application/x-www-form-urlencoded.


 
**What are the different kinds of Doctypes available? 
Ans : The three kinds of Doctypes which are available:
1) Strict Doctype : This DOCTYPE declaration refers to HTML documents 
that adhere strictly to the HTML specification without any deprecated 
elements or attributes. In earlier versions, such as HTML 4.01, this 
DOCTYPE was commonly used to create well-structured and standardscompliant web pages.
2) Transitional Doctype : Transitional DOCTYPEs were used to indicate 
that the HTML document is in a transitional phase, meaning it may contain 
elements and attributes that were deprecated in newer versions of HTML. 
This was particularly relevant during the transition from HTML 4 to XHTML 
or HTML5, where developers were updating their codebases to comply 
with newer standards.
3) Frameset Doctype : Frameset DOCTYPEs were used for HTML 
documents that contained frameset elements, which allowed developers 
to split the browser window into multiple independent frames. Framesetbased layouts were popular in the early days of the web but have since 
fallen out of favor due to accessibility and usability concerns.



### How is Cell Padding different from Cell Spacing? 
Ans : Cell Spacing is the space or gap between two consecutive cells. 
Whereas, Cell Padding is the space or gap between the text/ content of the 
cell and the edge/ border of the cell. Please refer to the above figure 
example to find the difference.


### How can we club two or more rows or columns into a single row or column in an HTML table? 
Ans : HTML provides two table attributes “rowspan” and “colspan” to 
make a cell span to multiple rows and columns respectively.


###  Is it possible to change an inline element into a block level element? 
Ans : Yes, it is possible using the “display” property with its value as 
“block”, to change the inline element into a block-level element.


###  Difference between link tag <link> and anchor tag <a>? 
Ans : The anchor tag <a> is used to create a hyperlink to another webpage 
or to a certain part of the webpage and these links are clickable, whereas, 
link tag <link> defines a link between a document and an external resource 
and these are not clickable.


###  What are the significant goals of the HTML5 specification? 
Ans : These were the target area of the HTML5 specs:
Introduction of new element tags to better structure the web page such 
as <header> tag.
Forming a standard in cross-browser behavior and support for different 
devices and platforms
Backward compatible with the older version HTML web pages
Introduction of basic interactive elements without the dependency of 
plugins such as <video> tag instead of the flash plugin.



###  Explain new input types provided by HTML5 for forms? 
Following are the significant new data types offered by HTML5:
    Date - Only select date by using type = "date"
   Week - Pick a week by using type = "week"
   Month - Only select month by using type = "month"
   Time - Only select time by using type = "time".
   Datetime - Combination of date and time by using type = "datetime"
   Datetime-local - Combination of date and time by using type = 
"datetime-local." but ignoring the timezone
   Color - Accepts multiple colors using type = "color"
   Email - Accepts one or more email addresses using type = "email"
   Number - Accepts a numerical value with additional checks like min 
and max using type = "number"
   Search - Allows searching queries by inputting text using type = 
"search"
   Tel - Allows different phone numbers by using type = "tel"
©Topperworld
Placeholder - To display a short hint in the input fields before entering 
a value using type = "placeholder"
Range - Accepts a numerical value within a specific range using type = 
"range"
Url - Accepts a web address using type = "url”

### What are the New tags in Media Elements in HTML5? 
Ans : 
➢ <audio> - Used for sounds, audio streams, or music, embed audio 
content without any additional plug-in.
➢ <video> - Used for video streams, embed video content etc.
➢ <source> - Used for multiple media resources in media elements, such 
as audio, video, etc.
➢ <embed> - Used for an external application or embedded content.
➢ <track> - Used for subtitles in the media elements such as video or 
audi
. What is the purpose of the method attribute in the <form> tag?

ans. The method attribute specifies the HTTP method used to send form data to the 

server. The most common values are "GET" and "POST".

###  What is the purpose of the action attribute in the <form> tag?

ans. The action attribute specifies the URL or destination where the form data should be 

sent.

###  What is the purpose of the <input> tag in HTML?

ans:The <input> tag is used to create various types of form input fields, such as text 

fields, checkboxes, radio buttons, and submit buttons.

###  What is the purpose of the type attribute in the <input> tag?

ans:The type attribute specifies the type of input field to be created, such as "text", 

"checkbox", "radio", "submit", etc.

###  What is the purpose of the <label> tag in HTML?

ans:The <label> tag is used to associate a text label with a form element. It improves 

accessibility and allows users to click on the label to activate the associated form 

element.

###  What is the purpose of the <select> tag in HTML?

ans:The <select> tag is used to create a dropdown list of options for users to choose 

from.

### What is the purpose of the <option> tag in the <select> tag?

ans:The <option> tag is used to define an option within a dropdown list.

###  What is the purpose of the value attribute in the <option> tag?

ans:The value attribute specifies the value associated with an option. It is sent to the 

server when the form is submitted.

###  What is the purpose of the <textarea> tag in HTML?

ans:The <textarea> tag is used to create a multiline text input field where users can 

enter larger blocks of text.

###  What is the purpose of the <iframe> tag in HTML?

ans:The <iframe> tag is used to embed another web page or document within the 

current HTML document.

###  What is the purpose of the <div> tag in HTML?

ans:The <div> tag is a container used to group and style HTML elements. Itis commonly 

used for layout and organization purposes.

###  What is the purpose of the <span> tag in HTML?

ans:The <span> tag is an inline container used to apply styles or manipulate specific 

portions of text within a larger block of content.