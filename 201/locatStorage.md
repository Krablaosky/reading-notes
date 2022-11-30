# Local Storage and How To Use It On Websites

Local storage is one of the most used pieces of a website that many people don't even realize it's there. This is such a useful tool for improving the function of our websites and saving user data locally.

1. Why would a developer use local storage for a web application?

Developers use local storage to save a users settings from their local device. So think about shopping on a website and you hit refresh, how annoying would it be if everytime you added something to your cart it reset when the page reloaded. Building local storage will save that data and use it on page reload so that the user can pick back up where they left off. Or think of your favorite settings for a website, keeping it in light or dark mode and when you come back to the website you don't want to have to select it every time. Local storage will save that data.

2. What information should not be stored in local storage?

The type of data we wouldn't want to save or store would be sensitive information. That sort of data is better stored on the back end server so that people can't steal sensitive data from a local device.

3. Local storage can store what type of data? How would you convert it to that type before storing?

Local Storage stores the datatype `string` and is usually stored via the command `stringify`. That is the easiest way to store data as a string inside of your local storage. If we try storing these variables as `objects` though, then an interesting thing happens and we store the object which can be referenced by it's corresponding key to be `parsed` later and retrieved.