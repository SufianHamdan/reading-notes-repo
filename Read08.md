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

### color
The color property allows you to specify the color of text inside an element. You can specify any
color in CSS in one of three ways:

**rgb values**
These express colors in terms of how much red, green and blue are used to make it up. 
For example: rgb(100,100,90)
**hex codes**
These are six-digit codes that represent the amount of red, green and blue in a color, 
preceded by a pound or hash # sign. For example: #ee3e80
**color names**
There are 147 predefined color names that are recognizedby browsers. For example:
DarkCyan We look at these three different ways of specifying colors on the
next double-page spread.

### background-color
CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box. You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values, hex codes, and color names (covered on the next page).
If you do not specify a background color, then the background is transparent. By default, most browser
windows have a white background, but browser users can set a background color for their windows, so if you want
to be sure that the background is white you can use the background-color property on the `<body>` element.
We have also used the padding property to separate the text from the edges of the boxes.

---

### Cloring 

**RGB Values**
Values for red, green, and blue are expressed as numbers between 0 and 255.

**Hex Codes**
Hex values represent values for red, green, and blue in hexadecimal code.

**Color Names**
Colors are represented by predefined names. However, they are very limited in number.

**Hue**
Hue is near to the colloquial idea of color. Technically speaking however, a color can also have
saturation and brightness as well as hue.

**Saturation**
Saturation refers to the amountof gray in a color. At maximum saturation, there would be no
gray in the color. At minimum saturation, the color would be mostly gray.

**Brigh tness**
Brightness (or "value") refers to how much black is in a color. At maximum brightness, there
would be no black in the color. At minimum brightness, the color would be very dark.

**Contrast**
When picking foreground and background colors, it is important to ensure that there is
enough contrast for the text to be legible.

**opacity, rgba**
CSS3 introduces the opacity property which allows you to specify the opacity of an element
and any of its child elements.  The value is a number between 0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15% opacity). The CSS3 rgba property allows you to specify a color, just like
you would with an RGB value, but adds a fourth value to indicate opacity. This value is
known as an alpha value and is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity
and 0.15 is 15% opacity). The rgba value will only affect the element on which it is applied (not child elements).

### HSL, HSLA color
CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation,
and lightness values.

**hue**
This is expressed as an angle (between 0 and 360 degrees).

**saturation**
This is expressed as apercentage.
**lightness**
This is expressed as a percentage with 0% being white, 50% being normal, and 100% being black. The hsla color property allows you to specify color properties using hue, saturation, and lightness as above, and adds a
fourth value which represents transparency (just like the rgba property). The a stands for:

**alpha**
This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75
represents 75% transparency.