# Exercise: Build Your Own Virtual Library

## Learning Goals

Upon successful completion of this exercise, you will be proficient in:

- Creating object using constructor functions and prototypes
- Implementing inheritance using the prototype chain
- Building objects to model real-world scenarios

## Introduction

Step into the world of literature and unleash your creativity by building a virtual library using JavaScript’s powerful object-oriented programming capabilities. In this immersive exercise, you’ll become an architect of knowledge, crafting a sophisticated system to manage and organize books of all kinds.

Your mission is to construct a robust foundation with a base `Book` class, serving as the cornerstone of your library empire. From there, you’ll explore the depths of inheritance by introducing specialized book types, each with its own unique characteristics and behaviours. 

But that’s not all! 

You’ll have the opportunity to showcase your ingenuity by designing and implementing your very own custom book type. Whether it’s a captivating comic book series, a mouth-watering collection of culinary mastepieces, or a genre-defying literary marvel, the possibilities are endless.

Prepare to dive deep into the realms of OOP, where you’ll master the art of creating objects, leveraging prototypes, and extending functionality through inheritance. Along the way, you’ll encounter real-world scenarios that will challenge your problem-solving skills and push your programming prowess to new heights. 

Get ready to curate your virtual library with pride, as you organize, manage, and showcase your library treasures. Embrace the power of JavaScript OOP, and let your imagination soar as you bring your literary vision to life!

## Getting Started

Follow the instructions below to get started:

1. Fork this Repository
2. Clone the Repository to your computer
3. Open the Repository in VS Code
4. Start the Live Server in VS Code
5. Follow instructions 

## Instructions

In this exercise, you will create a simple library management system using JavaScript objects. You’ll have a base `Book` class and different book types that inherit from it. You’ll also create your own custom book type by extending the base class or one of the existing book types.

1. Create a `Book` constructor function that takes `title`, `author`, and `publicationYear` as parameters and intialises them as properties on the object.
2. Add a `getDetails` method to the `Book` prototype that returns a string with the book’s title, author, and publication year.
3. Create a `FictionBook` constructor function that inherits from `Book` and takes an additional `genre` parameter. Initialise `genre` as a property on the `FictionBook` object.
4. Add a `getDescription` method to the `FictionBook` prototype that return a string describing the book’s genre.
5. Create a `TechnicalBook`  constructor function that inherits from `Book` and takes an additional `subject` parameter. Initialise `subject` as a property on the `TechnicalBook` object.
6. Add a `getSummary` method to the `TechnicalBook` prototype that returns a string summarising the book’s subject.
7. Create your own custom book type by extending either `Book`, `FictionBook`, or `TechnicalBook`. For example, you could create a `ComicBook`, or a `CookBook`.
8. In your custom book type, add the necessary properties and methods to represent the specific characteristics of that book type.
9. Create instances of `Book`, `FictionBook`, `TechnicalBook`, and your custom book type, and test their methods.

### Example usage

```javascript
// Create a FictionBook instance
const fictionBook = new FictionBook('The Great Gatsby', 'F. Scott Fitzgerald', 1925, 'Literary Fiction');
console.log(fictionBook.getDetails()); // Output: The book "The Great Gatsby" by F. Scott Fitzgerald was published in 1925.
console.log(fictionBook.getDescription()); // Output: This is a Literary Fiction book.

// Create a TechnicalBook instance
const technicalBook = new TechnicalBook('Clean Code', 'Robert C. Martin', 2008, 'Software Engineering');
console.log(technicalBook.getDetails()); // Output: The book "Clean Code" by Robert C. Martin was published in 2008.
console.log(technicalBook.getSummary()); // Output: This book is about Software Engineering.

// Create an instance of your custom book type
const customBook = new CustomBook('Watchmen', 'Alan Moore', 1986, 'Superhero');
console.log(customBook.getDetails()); // Output: The book "Watchmen" by Alan Moore was published in 1986.
console.log(customBook.getCustomDescription()); // Output: This is a Superhero comic book.
```

## Submission

1. When you're finished, run the following commands:

```bash
git add .
git commit -m "done"
git push origin main
```

2. Create a Pull Request and Submit your assignment.

## Bonus
Still got time left, or want to go the extra mile? 

- Add functionality to manage a collection of  books (e.g. adding, removing, searching).
- Add support for different book formats (e.g. hardcover, paperback, ebook).
- Implement a rating system where users can rate and review books.

## Let's Chat About Your Questions

<details close>
<summary>How do I get started with the book classes?</summary>

To begin your literary adventure, lay the foundation by creating the base `Book` Constructor Function. This Constructor Function should encapsulate the core properties and behaviors common to all book types, such as `title`, `author`, and `publicationYear`. From there, you can extend this class to create specialized types like `FictionBook`, and `TechnicalBook`.
</details>

<details close>
<summary>How can I implement inheritance in my book classes?</summary>

Inheritance is the key to unlocking the power of object-oriented programming in your virtual library. We covered in-depth how to implement inheritance correctly in the previous lessons. If you still struggle, we suggest you re-read the lesson again, before you continue on the exercise.
</details>

<details close>
<summary>What are some useful methods to add to my book classes?</summary>

Consider adding methods that provide meaningful information about each book type. For instance, you could have a `getDetails` method that return a summary of the book’s title, author, and publication year. Additionally, you could implement methods like `getDescription` for `FictionBook` to describe the book’s genre, or `getSummary` for `TechnicalBook` to summarize the book’s subject matter.
</details>

<details close>
<summary>How can I create my own custom book type?</summary>

Unleash your creativity by designing your own custom book type! Start by inheriting from either the base `Book` constructor function or one of the existing book types like `FictionBook` or `TechnicalBook`. Then, add any additional properties and method that make your custom book type unique. For example, a `ComicBook` type might have properties like `illustrator` or `publisher`, and methods like `getCharacters` or `getPlotSummary`.
</details>

Remember, every great literary masterpiece started with a single word. Start in the same way. Do one thing after another, and don’t try to tackle every single task at the same time.