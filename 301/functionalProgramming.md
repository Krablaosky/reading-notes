# Functional Programming

## [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

1. What is functional programming?

Functional programming is a style of building structure and elements of computer programs that treat computation as the evaluation of mathematical functions and avoids changing state and mutable data -Wikipedia

2. What is a pure function and how do we know if something is a pure function?

a pure function also referred to as deterministic,returns the same result if given the same arguments and it does not cause any observable side effects. In essence a pure function works exactly as expected

3. What are the benefits of a pure function?

The benefits of a pure function are that the past parameters will always be consistent as opposed to having continually changing results, these pure functions are also easier to test so we don't need to mock anything up We can reliably expect the same results

1. What is immutability?

immutability is dated that is unable to be changed after it is created.it can't be edited in any way shape or form and you just have to make a new one if you need new data

5. What is Referential transparency?

Preferential transparency is when a function consistently yields the same result for the same input,that means that the outcome will never change and we can we can always reliably count on that function to provide the same data

## [Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

1. What is a module?

a module is a separate section of code that can be referenced in a centralized place and reused multiple times as many times as it's called. we essentially are sectioning off code to be able to keep it in its own world and modify just that one part.

2. What does the word ‘require’ do?

require pulls in information that we need from another file,and find that data and pulls it into our new page

3. How do we bring another module into the file the we are working in?

To bring in another module we need to set the require to be associated with a variable that. then we can use that variable inside of that module using that name where it's going to pull in the exported data available.

4.What do we have to do to make a module available?

to make a module available we need to use the module.exports, Where we will export our module to be picked up by a require In another module
