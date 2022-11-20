# Audio Video & Images

## Video and Audio Content

1. Explain how the ability to use video and audio on the web has evolved since the early 2000s.

When we used to use audio and video back in the early 2000's, we relied heavily on things like `flash` and `silverlight` for plugins. They had their own security risks and were unreliable so now we use the built in `<Video>` and `<audio>` tags in HTML.

2. Describe the use of the src and controls attributes in the `<video>` element.

When using a video in our websites we still need to have a source to lead us to that video. That filesource is key for grabbing the right content. Since it's a video we need to be able to control aspects of the video with ease. You can either use the one provided in the browser or build an interface using JS. The minimum requirements are to be able to start, stop and adjust the volume.

3. Why is it important to have fallback content inside the `<video>` element?

It's important to have fallback in case the users browser won't load the video or support the video element. They need to be able to access the video in other ways so that they can view it outside of the webpage.

4. Write a very short story where `<audio>` and `<video>` are characters.

Audio and Video like spending a lot of time together. Audio like to do it's own thing and is a very free spirit and does not need video to be complete. on the other hand Video is a little more clingy and needs audio to make them feel complete even though the two share a lot in common.

## CSS Grid

1. How does Grid layout differ from Flex?

Grid differs from flex in several ways. Grid layout works really well for a grid structure but misses some of the flexbox functionality of centering or using a lot of the flexbox features. The grid feature is often more rigid and requires a lot of specific direction, while a flexbox is more, well, flexible. While they are very different they work together really well and can build something really cool.

2. Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

A grid container is the box that houses all of the grid items within it. Grid items are the individual elements that we want to show off as data and are housed inside the grid container. The grid line makes up the dividing lines of the grid and usually refer to horizontal(row) or vertical(column). These dividers help show off the grid items and make up the separation in the grid container.

## Responsive Images

1. Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

Aside from the obvious, responsive images can help reduce bandwidth use and use less data. There is a really good chance that the way the images would load could be impacted without them being responsive and they could hide or cover important information.

2. Define the following `<img>` attributes `srcset` and `sizes`. Write an example of how they are used.

the `img` attribute is usually for pointing the browser in the direction of a very specific image and uses exactly what we need it to. You would use this if you wanted to display your logo on a website. Your `srcset` helps to let your browser to choose which image should be used based on what will fit our criteria. So for instance if our page is a certain size we might want to display one image, and then if is shrinks down we would want to use a more compact image. We use this with the `sizes` attribute to help set the different sizes of our images. This allows us to set the best sized image based on certain conditions so that the website knows which one to use.

3. How is `srcset` more helpful for responsive images than CSS or JavaScript?

`srcset` is more helpful for responsive images because it allows us to properly utilize the correct size and scale images based on what screen size we are using.
Think about a website and why it wouldn't look good on your phone screen. The images would be too large or take up too much of the screen. they might even be too small to see in detail. It's much better to have a specifically customized image and scale for a smaller screen so that the webpage can look really good in different sizes and still communicate the same information.