## 1. What is the meaning of term casecading in css?

**Answer:** In CSS, the term "cascading" refers to the way styles are applied to HTML elements in a hierarchical manner. The "Cascading" part of Cascading Style Sheets (CSS) means that the final style of an element is determined by multiple rules or styles that can apply to it, with a hierarchy determining which style has the highest priority. The key aspects of cascading in CSS include:

- Inheritance: Some CSS properties are inherited from parent elements to their children. For example, text-related properties like font-family and color are typically inherited.

- Specificity: CSS rules have different levels of specificity. More specific rules override less specific ones. Specificity is calculated based on the type of selectors used (e.g., ID selectors, class selectors, and element selectors).

- Source Order: When two or more rules have the same specificity, the rule that appears later in the CSS will take precedence. This is known as the "last rule wins" principle.

- Importance: The !important declaration can be used to make a particular CSS rule take precedence over all others. Rules with !important will override any other declarations, regardless of specificity or order.

For example, consider the following CSS:

```html
/* General style for all paragraphs */
p {
  color: black;
}

/* More specific style for paragraphs with a class of 'highlight' */
p.highlight {
  color: red;
}

/* Inline style in the HTML */
<p style="color: blue;">This is a paragraph.</p>

/* Important rule */
p {
  color: green !important;
}

```

## 2. What is selector. how many type of selector are available in css?


**Answer:** A CSS selector is a pattern that is used to select the elements you want to style in an HTML document. Selectors are a crucial part of CSS as they determine which HTML elements will be affected by the CSS rules.

### Types of CSS Selectors
There are several types of CSS selectors, each serving different purposes:

- Universal Selector (*):

Selects all elements on the page.
Example:` * { margin: 0; padding: 0; }`

Type Selector (Element Selector):

- Selects all elements of a given type.
Example: `p { color: blue; }`

Class Selector (`.classname`):

Selects elements with a specific class attribute.
Example: .intro { font-size: 16px; }

- ID Selector (#idname):

Selects an element with a specific ID attribute.
Example: `#header { background-color: grey; }`

### Attribute Selector:

Selects elements based on an attribute or attribute value.
Examples:
```css
[type="text"] { border: 1px solid black; } 
 [title] { color: red; }
 ```

### Pseudo-class Selector:

- Selects elements based on their state.
Examples:
```css
a:hover { color: green; }
:first-child { font-weight: bold; }
```
### Pseudo-element Selector:

- Selects and styles parts of an element.
Examples:
```css
p::first-line { font-size: 1.2em; }
::before { content: "Note: "; color: red; }
```

### Descendant Selector:

- Selects elements that are descendants of another element.
Example:
```css
 div p { color: blue; }
 ```

### Child Selector (>):

- Selects direct child elements of a specified element.
Example: 
```css
ul > li { list-style-type: none; }
```

### Adjacent Sibling Selector (+):

- Selects an element that is immediately preceded by another element.
Example: `h1 + p { margin-top: 0; }`

### General Sibling Selector (~):

- Selects all elements that are siblings of a specified element.
Example: h1 ~ p { color: grey; }
Example of Using Different Selectors
```html
<!DOCTYPE html>
<html>
<head>
<style>
  /* Universal Selector */
  * {
    box-sizing: border-box;
  }

  /* Type Selector */
  body {
    font-family: Arial, sans-serif;
  }

  /* Class Selector */
  .intro {
    color: blue;
  }

  /* ID Selector */
  #main {
    background-color: lightgrey;
  }

  /* Attribute Selector */
  [type="text"] {
    border: 2px solid red;
  }

  /* Pseudo-class Selector */
  a:hover {
    color: green;
  }

  /* Pseudo-element Selector */
  p::first-line {
    font-weight: bold;
  }

  /* Descendant Selector */
  div p {
    color: purple;
  }

  /* Child Selector */
  ul > li {
    margin-bottom: 10px;
  }

  /* Adjacent Sibling Selector */
  h1 + p {
    margin-top: 0;
  }

  /* General Sibling Selector */
  h1 ~ p {
    color: grey;
  }
</style>
</head>
<body>

<h1>My Heading</h1>
<p>This is a paragraph.</p>
<p class="intro">This is another paragraph with a class.</p>
<p id="main">This paragraph has an ID.</p>
<input type="text" value="Text input">

<div>
  <p>Paragraph inside a div.</p>
</div>

<ul>
  <li>List item 1</li>
  <li>List item 2</li>
</ul>

</body>
</html>
```

Using the different types of selectors allows for precise and efficient targeting of HTML elements to apply styles.


## 3. Differentiate between CSS3 and CSS2.
**Answer:** The main difference between CSS3 and CSS2 is that CSS divides different sections into modules and supports many browsers. It also contains new General Sibling Combinators responsible for matching similar elements. 

## 4. Explain a few advantages of CSS. 
**Answer:** With CSS, different documents can be controlled using a single site, styles can be grouped in complex situations using selectors and grouping methods, and multiple HTML elements can have classes.

## 5. What is meant by RGB stream?
**Answer:** RGB represents colors in CSS. The three streams are namely Red, Green, and Blue. The intensity of colors is represented using numbers 0 to 256. This allows CSS to have a spectrum of visible colors. 

## 6. What was the purpose of developing CSS?
**Answer:** CSS was developed to define the visual appearances of websites. It allows developers to separate the structure and content of a website that was not possible before. 

## 7. How can you target h3 and h2 with the same styling?
**Answer:** Multiple elements can be targeted by separating with a comma:

h2, h3 {color: red;}

## 8. Tell us about the property used for image scroll controlling?
**Answer:** The background-attachment property is used to set whether the background image is fixed or it scrolls with the rest of the page. Example for a fixed background-image:

body {

  background-image: url(‘url_of_image’);

  background-repeat: no-repeat;

  background-attachment: fixed;

}

## 9. Difference between reset vs normalize CSS? How do they differ?
**Answer:** Reset CSS is used to remove all built-in styles in the browser such as paddings, margins, and font sizes, and can be reset using all the elements.
Normalize CSS is used to make all built-in styles in the browser consistent and correct bugs as per varying browsers.

## 10.  What are Pseudo classes?
**Answer:** Pseudo-classes are the type of pseudo-elements that don’t exist in a normal document tree. It allows selecting the regular elements under certain conditions especially when we try to hover over the link; the anchor tags are :link, :visited, :hover, :active, :focus

In this example, the color will be red on the anchor tag when it’s hovered.

/* mouse over link */

a:hover {

color: #FFOOFF;

}

## 11. What do you understand by pseudo-elements?
**Answer:** Pseudo-elements provide special effects to some selectors. CSS finds use in applying styles in HTML markups. If additional markup or style is not feasible for a document, the pseudo-elements help by allowing extra markup without interfering with the original document. 