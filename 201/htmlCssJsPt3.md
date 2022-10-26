# HTML, CSS, JS Part 3

## Creating links and hyperlinks in HTML

Using links and hyperlinks in HTMl is crucial to having an interactive and usable website. Without it you can't include multi-app functionality or build in things like a google maps section of your business's location.

Here are our HTML questions

1. To create a basic link, we wrap text or other content inside what element?
   
To create this link we need to use the `<a>` element and the `href` attribute to place content inside for a hyperlink

2. The href attribute contains what information?

Our `href` attribute contains all of the hyperlink information we need to be able to navigate to the link. Think of the `href` as the behind the scenes part while the text that goes after is what the link is contained in

3. What are some ways we can ensure links on our pages are accessible to all readers?

To ensure that our hyperlinks are accessable we need to include things like a `title` so that screen readers can try to explain where the hyperlink is going and what it is intended to do.

## CSS Layout

CSS layout is an really useful tool for figuring out how everything should look, what order it needs to go in, and how you can make your website pop.

1. What is meant by “normal flow”?

Normal flow is the basic way that CSS looks before you add any additional styling to it. It takes the basic elements that are most easily read and builds a website that flows in a normal pattern.

2. What are a few differences between block-level and inline elements?

So a block line element's content will fill the available space inside the parent element, making sure that the content will fit the box. Block line elements are flexible and fit to the needed space. Block line elements will follow the inherited parent flow, which starts by default as horizontal, making each new box a new line going down the page.

 Meanwhile inline elements are only the size of the content. With inline elements you are unable to set the width or height because they sit inside the content of the block level elements.Inline elements dont appear on new lines and just fit into the same space with any text content, as long as there is room for them. If not then it will move to a new line when it runs out of space.

3.  positioning is the default for every html element.

Static positioning is the default for every html element

4. Name a few advantages to using absolute positioning on an element.

Absolute positioning creates a few advantages over other positions. When using it, the elements function separately from the rest of the pages normal flow. Now we can create isolated UI features that won't interfere with the layout of other elements on the page. Think of popup boxes as absolute positions. They don't push all the text out of the way to show you what you need.
The absolute positioning also uses rules compared to the whole container of the page not just the individual containers so thats a key consideration.

5. What is a key difference between fixed positioning and absolute positioning?

The key difference between fixed position and absolute position is that absolute positioning is relative to its nearest positioned ancestor, fixes position fixes an element in place relative to the visible part of the page, so a nav bar on the side will always be there and always be visible.

## Continuing JS and Functions

using functions in Javascript is one of the most crucial things we learn. We are discovering how to write less code and have it go further and do more things. Think about just calling a section of code you wrote a hundred times instead of having to write it out each time.

1. Describe the difference between a function declaration and a function invocation.

A function declaration looks like `function hello()` This is letting us know tha the code we are going to look at will be under the function hello(). A function invocation is when you actually call the function to the front line to be used. in this case we would use it like
`hello('Nick')`. Here we are calling the function to be used and feeding it the string `'Nick'`

2. What is the difference between a parameter and an argument?

When we look at it the parameter is often what an argument is assigned to. So if we looked at the example above, if we set `name = 'Nick'` the variable on the left would be our parameter while the content of the variable is the argument. We can use this to pass arguments into functions or pass pre-assigned values into a function, or even assign a parameter a value based on a function.

## Why Pair Programming

Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.

One benefit of pair programming is the efficiency in working with others. Sometimes another person will have a specialty in one field like JS or CSS and it can be helpful to have someone to lend their expertise to something and it goes by much faster. It can also be beneficial to having two people thinking about how something can work rather than when one person get stuck on a problem and can't move past it. The collaboration will be crucial to moving ahead with a lot of programming and efficiency.

The other benefit of pair programming is increasing collaboration through developing crucial social skills necessary to work in teams. Most jobs work in teams and being able to collaborate with others is a crucial part of the field. Learning to collaborate with people who are varied levels of skill can really be integral to simulating the workplace environment as well as your own social skills in those environments. How you work with someone who isn't as skilled as you is just as important as working with someone who is more skilled than you.
