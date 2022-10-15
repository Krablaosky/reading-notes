# Recap of Javascript & HTML

## A Poem for HTML

Sending a request

Trying to get a Copy

Past the gatekeeper

Granted gold access, 200 OK

The page displays

Tiny chunks build a whole page

Praise be to HTTP

## How are HTML, CSS and JS parsed in the browser

The order in which the webpage gets parsed is based on the order they are laid out in our coding format. Often towards the top of our HTML page we have a `<link>` to our external `CSS` Sheet(our style sheet) and our external `JavaScript` page with all of our functions.

It follows the link we have laid out and sends the request back to the server to retrieve those external sheets.

Then the browser generates memory of those files from those files in a `CSSOM` stucture and uses that to execute the Javascript and the CSS files.

It first looks at the CSS sheet for the display and style then it goes to the Javascript file for any necessary functionality.

## Back to our JS basics

JS is the main way that we add functionality to our websites, it is usually based on some sort of user interaction and takes some form of input, processes it around a little to give us the result as an output.

It can be used for super simple functions like adding and subtracting, or extremely complex ones that would be used in advanced games.

Some browsers have API's(Application Programming Interfaces) built in while others use third party API's to power functions on a webpage in the background.

It is really important to think about placement of the JS in your code and where it belongs. If it loads before the HTML it is supposed to impact it could cause an error, because the HTML isn't there yet. Sometimes the best practice can be **placing your JS code at the bottom of the page**

### JS variables

variables are things we assign values to, then we can use that value to interact with different functions and manipulate the data inside. If we don't assign variables before we use them in a function then we run into an error. It's like me saying you need to use a `Squeedlyspooch` in tonights class. You have no idea what that is. How can you use a `Squeedlyspooch` if you've never heard of it. If I tell you it's another name for a pen, then you will understand that that's what I want you to have.

`let Squeedlyspooch = "pen";`

There are some restrictions on what variable names you can use in JS, specifically ones for prebuilt functions in JS that are already defined.

Variables can be changed later in time which is great. If I tell you now a `Squeedlyspooch`means laptop, you still might remember from earlier that it was a pen, but now it's a laptop and you need that for the next section.

## Strings vs numbers

when we get into how to write out different variables it's incredibly important to know how to do some simple things like write out numbers.

If we try to write out the number 42 in a JS function, we just write the number as it is with no attachments or anything.

`let number = 42` makes it so this variable number has a value of 42. We could manipulate that information to solve for some of these things.

`number * 2` would give us `84`

if we had it so that

`let name = 'bob'` Then we have assigned the variable name to the string `bob`, and if we tried a similar thing.

`name + name` we would get `bobbob`

Strings will always have either `' '` or `" "` surrounding it and that is how we can identify them quickly.

## Conditionals

we can use these conditional statements to execute a function if something meets our conditions or criteria. For instance, if a is true then run function until a isn't true

We can also use it to test and check users entries and give output based on their responses.

```javascript
let iceCream = "chocolate";
if (iceCream === "chocolate") {
  alert("Yay, I love chocolate ice cream!");
} else {
  alert("Awwww, but chocolate is my favorite…");
}
```

The function exists inside of the `{ }` while the variables are executed withing the `( )` of the function.

## Events

Events are fun things within JS that we use all the time. Everytime you clock your mouse button you are initiating a button click event!

We can use buttons to create events as well, these are clickable or interactable items that can be tied to specific JS functions.

We would use it like this

```javascript
<button> Change User </button>
myButton.onclick = () => {
  setUserName();
};
//this next section goes at the bottom of the page
let myButton = document.querySelector("button");
let myHeading = document.querySelector("h1");
// this section goes inside our JS document
function setUserName() {
  const myName = prompt("Please enter your name.");
  localStorage.setItem("name", myName);
  myHeading.textContent = `Mozilla is cool, ${myName}`;
}

//we would add this conditional block to help, we would call on this during initialization
if (!localStorage.getItem("name")) {
  setUserName();
} else {
  const storedName = localStorage.getItem("name");
  myHeading.textContent = `Mozilla is cool, ${storedName}`;
}
```

## Images

How could we use *events* and images together. Well we could have an image change to another one when the user clicks on it.

When looking to find images for your website you will want to make sure that you find free to use images that don't have copyright and that you aren't plagarizing someone elses work without their permission.

You will want to add these images to your repository in an images folder so that they all live together or can be further separated out. It is extremely important to label them in the clearest way possible. For instance, `Homepage background.jpg` is extremely clear and composed for what you want it to be for.

IF you are trying to use an event to change an image to another you will want both images to be as close in size and shape as possible for a smooth transition.

Here's a great example of a click to change image function

```javascript
const myImage = document.querySelector("img");

myImage.onclick = () => {
  const mySrc = myImage.getAttribute("src");
  if (mySrc === "images/firefox-icon.png") {
    myImage.setAttribute("src", "images/firefox2.png");
  } else {
    myImage.setAttribute("src", "images/firefox-icon.png");
  }
};
```

You can check out some examples of complete code [Here](https://github.com/mdn/beginner-html-site-scripted/blob/gh-pages/scripts/main.js)

[Click Here for HTML & JS Continued](htmlctd201.md)