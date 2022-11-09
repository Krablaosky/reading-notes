# CSS Layout

## It's all about the flex-box

1. Flexbox is designed for one-dimensional content. Explain what this means.

This means that it excels at taking a lot of items with differing sizes and find the best layout for them to work together. It's the easiest way to get a bunch of items to fit together on a line, think of a bunch of images next to eachother, all different sizes.

2. Explain the difference between the main axis and cross axis.

The main axis is the primary axis that is being used for these items that are being flexed, this is usually determined by using the row or column `flex-direction`. Whichever you choose will be your main axis. The cross axis is the exact opposite of your main axis. So if your main axis is horizontal then your cross axis will be the vertical axis. 

1. How can using certain properties of flexbox negatively impact accessibility?

If you end up using the `row-reverse` or `column-reverse` values, then you will impact accessibility. It can make the rendered items still appear in the order initially set, even though the images might be entirely different. It's a big consideration when thinking about accessibility.

### CSS Layout - Flexbox

Read up to “Flex-Flow Shorthand”

1. What are some advantages of using flexbox over float?

Using flexbox can be better than using float for a few reasons, first it is more adaptive and can create better looking content than just a float or positon setting. It wouldn't be possible to align the content inside of a parent element or making all columns in a document have the same dimensions even though they contain different amounts of content.

2. How does this topic connect with your long term goals?

I know that I will be using flexboxes in my future, I hope to develop websites and flexboxes seem to be the easiest and most efficient way to make something on a webpage do exactly what you want. I think of a really good nav bar or really good line of buttons that grows or shrinks with the page and how I will use flexboxes to make that happen. I really see a lot of CSS and flexboxes to accomplish my goals of developing websites.
