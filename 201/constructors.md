# Constructors with JS and HTML

## Domain Modeling

Explain why we need domain modeling.

Domain modeling is important to get a simple message across to all parties involved in the process. We want to create a conceptual model for a very specific problem. You want to think about the most common things we need to communicate and what we use it for. Domain Modeling helps make these things easily understood by people at all levels and builds out the baseline for what programs and constructors do.

## HTML Table Basics

Why should tables not be used for page layouts?

HTMl Tables shouldn't be used for a page layout because they are inneficient in a few things. They are not good for accessibility for visually impaired users and the screen readers output will often not correspond to what the webpage wants to share and make it more confusing. They also require much more complex markup structures and increase complexity for not a lot of gain. They also are not automatically responsive with a lot of CSS and it takes so much more work to get a table to do what you want in terms of style and design.

List and describe 3 different semantic HTML elements used in an HTML `<table>`.

our 3 semantic elements in an HTML `table` are `tr`, `td`, and `th`.

`tr` or table row builds out a row for your table, think about a battleship board. It would be the 1-9 numbers on the lefthand side of the board. `tr`.

`td` is for table data, this is for each of the data points inside the row. Think about A4, B6, C3, F8. Those are all data points inside the tables cells.

`th` stands for table header. This helps build our table header for data and would be the A-Z letters on the top of our battleship board.

## Introducing Constructors

What is a constructor and what are some advantages to using it?

A constructor is like a factory that makes objects. Sure we could type out the code to make a hundred objects by hand, but what if we had a factory where all we told it was the data and it would build us an object. That is why we use constructors. They will make building our objects that much easier and easier to access those objects when we need to add on data to those objects.

How does the term `this` differ when used in an object literal versus when used in a constructor?

The term `this` differs when we are referring to an object literal vs a constructor because when we use `this` on an object literal, it only applies to that one object. When we use `this` to refer to a constructor it will refer to whatever lives inside that constructor as a whole value. It makes it much easier to extract information.

## Object Prototypes Using A Constructor

Explain prototypes and inheritance via an analogy from your previous work experience.
NOTE: This is a very common front end developer interview question

A prototype in the culinary world would be like building a prep sheet that lets people know what they are building. When you add a recipe onto that prep sheet it's like giving a prototype because you are skipping the whole part of having to write out each and every part, because you simplified the whole process into a recipe that they can now use to create a dish.

Inheritance is like when you get a bunch of kitchen equipment from the last owners. You don't always get a say in how the kitchen was built, but now you have to work around what you inherited to do the job. So the prep table in against the left wall, now you need to figure out where everything goes based on the fact that you inherited this workspace.