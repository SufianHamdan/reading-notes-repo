# CSS

CSS allows you to create rules that specify how the content of an element should appear.
For example, you can specify that the background of the page is cream, all paragraphs should
appear in gray using the Arial typeface, or that all level one
headings should be in a blue, italic, Times typeface.

The key to understanding how CSS works is toimagine that there is an invisible box around
every HTML element.

---

### Block and Inline element 

Block level elements look like they start on a new line.
Examples include the `<h1>` `<h6>` `<p>` and `<div>` elements.

Inline elements flow within the text and do not start on a new line.
 Examples include `<b>` `<i>` `<img>` `<em>` and `<span>`.

---

### Example Styles
CSS allows you to create rules that control the way that each individual box (and the contents
of that box) is presented.

**Boxes**
Width and height Borders (color, width, and style) Background color and images
Position in the browser window.

**Text**
Typeface
Size
Color
Italics, bold, uppercase,
lowercase, small-caps.

**Specific**
There are also specific ways
in which you can style certain
elements such as lists, tables,
and forms.


---

**CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration.**

```
Selector
{
    font-family: Arial;
}
```

**CSS declarations sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.**

```
h1, h2, h3 {
font-family: Arial;
color: yellow;}

```

---

### Using External CSS 

**`<link>`**
The `<link>` element can be used in an HTML document to tell the browser where to find the CSS
file used to style the page. 
It is an empty element (meaning it does not need a closing tag), and it lives inside the `<head>` element.
It should use three attributes:

**href**
This specifies the path to the CSS file (which is often placed in a folder called css or styles).

**type**
This attribute specifies the type of document being linked to. The
value should be text/css.

**rel**
This specifies the relationship between the HTML page and the file it is linked to.
The value should be stylesheet when linking to a CSS file.

---

### Inheritance

* If you specify the font-family or color properties on the `<body>` element, they will apply
to most child elements. This is because the value of the font-family property is inherited by child elements. It saves you from having to apply these properties to as many elements (and results in simpler style sheets).

* You can compare this with the background-color or border properties; they are not
inherited by child elements. 
If these were inherited by all child elements then the page could look quite messy.

* You can force a lot of properties to inherit values from their parent elements by using inherit for the     value of the properties. In this example, the `<div>` element with a class called page inherits the padding
size from the CSS rule that applies to the `<body>` element.

---

### Why use External Style Sheets?

* When building a website there are several advantages to placing your
CSS rules in a separate style sheet.

* All of your web pages can share the same style sheet. This is achieved by using the `<link>` element on each HTML page of your site to link to the same CSS document. This means that the same code does not need to be
repeated in every page (which results in less code and smaller HTML pages).

Therefore, once the user has downloaded the CSS stylesheet, the rest of the site will load faster. If you want to make a change to how your site appears, you only need to edit the one CSS file and all of your pages
will be updated. For example, you can change the style of every `<h1>` element by altering the one CSS style sheet, rather than changing the CSS rules on every page. The HTML code will be easier to read and edit
because it does not have lots of CSS rules in the same document. It is generally considered good
practice to have the content of the site separated from the rules that determine how it appears.

**Sometimes you might consider placing CSS rules in the same page as
your HTML code if your creating a single page**