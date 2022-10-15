# HTML Continued Review

[Check out lots of info on HTML here](../102/html.md)

## Attributes

An attribute is extra information about an element that don't usually show up. Attributes usually give specific names to things so that they can be referred to back later when doing something like a `CSS` sheet.

### So what should an attribute contain?

An attribute should always have the following:

* A space between it and the element name (or the previous attribute, if the element already has one or more attributes).
* The attribute name is followed by an equal sign.
* The attribute value is wrapped by opening and closing quotation marks.

## Anatomy of an HTML Element

This is what an HTML document is made up of at its core.

```html
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <title>My test page</title>
  </head>
  <body>
    <p>This is my page</p>
  </body>
</html>
```

We need the Doctype to tell us what type of file this is. We can use some shortcuts like `!` in VS code to quick enter the entire code above to save time.

The `html` tags contain all the content of the page and is the entire being.

Meanwhile the `head` element is all of the information that isn't viewer facing and has a lot of hidden info for search terms and what the website does. Think about a google search and you find some weird websites that aren't related because they used a lot of keywords in their header.

The `title` is simply for the title of the page and the `body` is what contains all of the infomration that makes the website look like the website we know.

## Article vs Section

An article en closes a block of related content that exists in it's own bubble, like a blog post. It's a singular item that exists and only needs to exist in that one spot. A section is more for grouping together parts of a page that belong together. These sections can be incorporated into articles and be used to break up an article into sections, but it rarely ever works the opposite way.

## Typical Elements In A Website

`<header>`
* Usually a big strip across the top with a big heading, logo, and perhaps a tagline. This usually stays the same from one webpage to another.
`<navigation bar>`
* usually a lot of buttons or links to the next parts of the website
`<main>`
* Usually where most of the content lives
* `<article> or <section> or < div>` with `div` being one of the most common
Sidebar
* peripheral info like quotes, adds, or sometimes specific sections for websites
* `<aside>` which often lives in `<main>`
`<footer>`
* Strip across the bottom of the page that contains copyright info or contact info etc.

## Metadata

We already covered some parts of the `head` of an HTML document and the metadata that lives within it gives off a lot of information that is extremely helpful.

We've seen this line a few times before, but what does it actually do.
This element tells us that we want to use the universal character set, which works for any character from any human language.

`<meta charset="utf-8" />`

Often the `meta` element contains info that can be helpful and still somewhat hidden. It can have things like `name` and `content` to help get people to your site.

Good metadata clearly gives all the necessary keywords and information about what it does and what people might be looking for. It's important to use keywords that will be commonly used and clearly explain a lot of detail. Think about how you type google questions and use that to configure your metadata.

## Semantics

In programming semantics refer to code that kinda does exactly what it says it does.

In JS we have functions that need to be named aptly. The `Math` function does exactly what is states.
If you write a function think about the readability of it.

Does a function named `makeMeApplesauce()` make more sense than `sauceAttack()`?

Some of the most common ones are little things like `<h1>` and it stands for the first and primary top level heading. You could also use something like `<span>` to float something to the top but then you loose customization and code reusability of a CSS sheet and have to recode it every time. Such a pain!

Why would we use sematic markup in our websites?

* It helps search engines find your site
* It is extremely important for accessability and screen readers.
* It's easier to find meaningful code blocks that describe what they do rather than go on an easter egg hunt
  
### Here's a list of some common semantic elements

* `<article>`
* `<aside>`
* `<details>`
* `<figcaption>`
* `<figure>`
* `<footer>`
* `<header>`
* `<main>`
* `<mark>`
* `<nav>`
* `<section>`
* `<summary>`
* `<time>`

## Website design

Ok so we've talked about HTML a bunch, now we want to build a website so lets get coding right? We aren't quite there. We need to do some work outside of coding to make our coding that much easier and straightforward.

Think about what the point of the website is, what is its primary purpose? What goal will this website help me achieve? Has anyone else done this before and if so what can I learn from them. It is important to create a plan of what you want this all to be so that you can work off it as you move forward. The more work you do in the planning stage the less you will have to do in the building stage.

For instance, I want to make a website that sells my custom spice blends.
I want this website to sell my product and I want users to get some information about spices and some recipes that they can use with them. I would want to write out all of these functionalities and then check against other websites that do similar things. What did they do that looked good or worked really well. It's ok to get inspiration but don't steal from someone.

What would be the goals, those are important things to think about. I want people to be able to do a few things so I need to write out each section and break it into tasks.

I want to sell recipes, I need a shopping cart and item description page.

I want to have a blog, I need content to go over and to keep it organized and themed.

I want to have recipes, how do other recipe sites look, can I make a conversion function for the ingredients?

Once you have this done you can move on to whiteboarding or drawing out your plan. It's much easier to code once you have a whiteboard together and you can see how it should be laid out.

## Ok so why JavaScript for an HTML page

We have a pretty looking webpage using `HTML` and `CSS`, so what do we really need JS for? We kinda covered it earlier but for all user interactions we need 
