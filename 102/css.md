# CSS

## What is CSS

CSS stands for Cascading Style sheets which is the backbone to making a beautiful website. Using CSS is where you can really specify what details you want to use and how you want them implemented for different sections of your website. By standard default your browser will style your page with HTML using a n internal style sheet, but you can replace it with a CSS sheet to really make it pop.

### How to use CSS

CSS is really a rule-based language that you specify groups of styles that should have specific rules applied to them. This way you can have control over different sections of your webpage and make one header’s color, font, size, and alignment different from an almost identical one.

`h1 {`

  `color: red;`

  `font-size: 5em;`

`}`

Take this for instance, we are using the selector h1 to alter heading 1(`<h1>`)

We place all of the details inside curly braces { } to show what belongs inside it.

Then we have our specific elements, color should be red and the font size should be 5em. A cool feature of CSS sheets is that it will try its best to show what you want to someone else, but if those fonts or other styles aren’t available then it will try to find the next best thing that someone’s computer might have so that your webpage doesn’t break.

The key is to try and not remember every rule for CSS styling sheets but focus on knowing the simple basics of how you are assigning element groups their specifications, then have a cheat sheet or google the specifics of what you are trying to do. The real challenge is learning how to google what you want.

## How do we add a CSS sheet

There are 3 ways to add a CSS sheet

* External
* Internal
* Inline

External sheets are defined with the `<link>` elements inside the `<head>` section of an HTML Page. They can be written in any text editor and remember to save it with a .css extension.
 Your external sheet should mot contain any html tags!
For instance

```html
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

Internal CSS
Can be used if a single HTML page has a unique style and you only want to style that one sheet a specific way. We define it with the `<style>` element inside the `<head>` section again but this time we put all the style info inside the html page.
For example

```html
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

Inline CSS

Is for when you want to style a single element inside and HTML page. It is explicitly for that single line.

```html
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```

## Cascading Order

CSS follows the cascading order rule, whatever is the most recent(i.e. last) style to be read will be the style used.

In general CSS will follow this order for style sheets in terms of how it will display.
Inline style (inside an HTML element)
External and internal style sheets (in the head section)
Browser default

For linking multiple style sheets, order is extremely important. Whichever one comes last will be the one the HTML page uses.
If you have an external style sheet and then an internal style sheet after it, the style for that section will go to the internal one because it is specifically overriding the external sheet.

For a comprehensive list of style check out [This Page](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
