# Front-End Development Libraries (v9): Comprehensive Curriculum

Welcome to your compiled Master Document. This reference textbook seamlessly glues together core fundamentals, stylesheets, application layout logic, typed compilation patterns, runtime profiling, and system architecture verification testing.

---

## Module 1: Introduction to Web Libraries, Frameworks & Build Tools

### Lecture 1.1: What Is The Role Of Js Libraries And Frameworks And Why Are They Used In The Industry

# What Is the Role of JS Libraries and Frameworks, and Why Are They Used in the Industry?

JavaScript libraries and frameworks provide pre-built code that streamlines the development process. While both libraries and frameworks serve to improve productivity and standardize coding practices, they differ in their approach and level of control they provide to developers.

Libraries are generally more focused on providing solutions to specific tasks, such as manipulating the DOM, handling events, or managing AJAX requests.

An example of a JavaScript library is jQuery.

jQuery became very popular in the early 2010s and was widely used to simplify DOM manipulation, event handling, animations, effects, and more. This library also offered a rich ecosystem of plugins, which made it easy to build common web components like date pickers, sliders, and modal dialogs.

Although jQuery is no longer as widely used as it once was, it significantly helped developers by making tasks that were complex in vanilla JavaScript much easier to implement.

Frameworks, on the other hand, provide a more defined structure for building applications. They often come with a set of rules and conventions that developers need to follow.

For example, Angular encourages a component-based architecture with a set of conventions and tools that provide a structured approach to organizing and building applications. Angular gives developers clear guidelines on how to structure components, manage state, handle routing, and interact with services, making it a more opinionated framework.

Other examples of frameworks include Remix and Next.js.

In contrast, React, a UI library, is more flexible and doesn't enforce any particular architectural pattern. React focuses primarily on the view layer and leaves a lot of the choices on application design up to the developers.

Although libraries and frameworks are used across projects of all sizes, the choice between using them often depends on the project's requirements. Libraries offer flexibility for specific functionalities, while frameworks provide a structured approach towards complex applications.

In the industry, libraries and frameworks are widely used for several reasons. They significantly speed up development by providing quick solutions for common problems.

One common problem in JavaScript is working with dates and timezones. But there are libraries out there with built-in solutions to help you with date manipulation, time zones, parsing and formatting of dates.

A lot of popular libraries and frameworks are well-tested and maintained by large communities. This means they're often more practical than building the same thing from scratch.

Libraries and frameworks follow best practices and patterns that have been proven effective in real life scenarios. This can lead to more robust and scalable applications.

In conclusion, libraries and frameworks offer quick solutions to common problems, speed up development, and promote best practices. Understanding the differences between libraries and frameworks, and knowing when to use them is a valuable skill for any JavaScript developer.

---

### Lecture 1.2: What Is React And What Is It Commonly Used For

# What Is React, and What Is It Commonly Used For?

React is one of the most popular JavaScript libraries for building user interfaces and web applications. Originally developed and maintained by Facebook, React has gained huge popularity in web development due to its efficiency, flexibility, and features.

A fundamental concept in React is the creation of reusable UI components. These components, such as buttons, cards, and avatar components, can be easily reused throughout your application. You can nest these components inside each other to build more complex, dynamic interfaces.

One of the key advantages of React is that these custom components can update and render independently as data changes.

Unlike traditional JavaScript, which requires direct manipulation of the DOM (Document Object Model), React uses a virtual DOM, which improves performance and efficiency. You’ll learn more about the virtual DOM and how it works in upcoming lessons.

In addition to reusable components, React also provides a powerful way to manage the state of your application. State refers to the data that determines how a component renders and behaves.

With React, you can easily track and update the state of components, ensuring that the UI reflects the most current data. You will learn more about working with state in future lessons.

While there are many libraries within the JavaScript ecosystem, freeCodeCamp will mainly be focused on teaching React because of its widespread use and demand in the industry.

Our next few lessons will dive deeper into building custom components, managing state, and more.

---

### Lecture 1.3: What Are Single Page Applications And What Are Some Issues Surrounding Them

# What Are Single Page Applications, and What Are Some Issues Surrounding Them?

Unlike traditional multi-page websites, single page applications (SPAs) load only one HTML page and dynamically update the content as the user interacts with the app, without reloading the entire page. This approach can lead to faster, more responsive applications, but it also comes with a set of challenges and considerations.

SPAs heavily use JavaScript to manage the application's state and render content. Instead of requesting new HTML pages from the server, SPAs use JavaScript to manipulate the DOM and fetch data asynchronously. This is often done using libraries and frameworks like React, Vue, or Angular, which provide great tools for building complex user interfaces.

SPAs have some common issues. One significant issue is that screen readers may struggle with dynamically updated content. When content changes without a page reload/refresh, screen readers might not notify these changes, which makes our users unaware of updates on our web app.

Another challenge with SPAs is with navigation and browser history. Users expect the back and forward buttons to work as they do on traditional websites. This might not work properly in SPAs because technically, the URL of the web app doesn’t change. Since the URL of the web app doesn’t change, they can’t bookmark any specific page. Refreshing the page might reset the application to its initial state, rather than maintaining the current view.

SPAs can pose challenges for SEO optimization. Search engines like Google can have difficulty indexing dynamically loaded content because they may not execute JavaScript properly or may miss content that isn’t included in the initial HTML page. This can lead to pages not being indexed correctly.

However, modern search engines have improved their ability to crawl SPAs, and there are techniques such as server-side rendering (SSR), pre-rendering, and the use of SEO-friendly URLs that can help mitigate these issues and improve SEO for SPAs.

Performance is another consideration. SPAs load the entire application in one go, which means that if the loading time increases, users will be seeing a blank screen for a longer period of time. Now consider the scenario of users with slower internet speeds. Overall, the user experience will not be very pleasant.

In conclusion, while Single Page Applications offer many benefits, they also present unique challenges. Developers need to be careful of accessibility, usability, SEO, and performance considerations when building SPAs. By addressing these issues, it's possible to create SPAs that are fast, responsive, and accessible to all users.

---

### Lecture 1.4: What Is Vite And How Can It Be Used To Set Up A New React Project

# What is Vite, and How Can It Be Used to Set Up a New React Project?

Unlike working with smaller vanilla HTML, CSS, and JavaScript projects, starting a new React project includes a few more steps to ensure that everything runs correctly. Instead of trying to set up all of the necessary configurations by yourself, there are tools that will do that for you.

One of the most popular tools for setting up projects is Vite. Vite, which means "fast" in French, is a build tool that aims to provide a faster development experience for modern web projects. Vite can be used with React, as well as with other libraries and frameworks like Vue or Svelte. You can even use it with vanilla JavaScript projects.

To create a new project with Vite, you will need to use the command line. If you are using Windows machine, then you can use the Command Prompt or Windows PowerShell. If you are using a Mac, then you can use the Terminal app.

In case you don't have Node.js installed, which is needed for npm to work, here is a link for the official Node.js webpage: https://nodejs.org. Follow the installation instructions then come back here to resume your React installation.

Once you have the command line open, you can use the following command:

```
npm create vite@latest my-react-app -- --template react
```

This command creates a new React project named `my-react-app` using Vite's React template.

You can then open up the new project and see the React boilerplate code that Vite has provided for you.

The great thing about Vite is that it will only provide the files that are absolutely necessary to get started with your React project.

To actually run the project as-is, you will need to install the dependencies using the following commands in the command line:

```bash
cd my-react-app
npm install
```

The `cd my-react-app` command ensures that you change to the correct directory where your project is located.

The `npm install` command is used to install the dependencies needed to properly run your React project. Dependencies are libraries or packages that your React project requires in order to function correctly, such as React itself, ReactDOM, or other third-party packages that provide additional functionality.

Running `npm install` will read the `package.json` file in your project directory and install all the dependencies listed there, allowing you to build and run your React app without missing any necessary components.

The `package.json` file is a key configuration file in projects that contains metadata about your project, including its name, version, and dependencies. It also defines scripts, licensing information, and other settings that help manage the project and its dependencies.

Once the dependencies are installed, you should notice a new folder in your project called `node_modules`.

The `node_modules` folder is where all the packages and libraries required by your project are stored. This folder contains the actual code for the dependencies listed in your `package.json` file, including both your project's direct dependencies and any dependencies of those dependencies.

To run your project, run the `npm run dev` command and open up a new browser tab at `http://localhost:5173/`.

You should see the starter template that Vite has provided for you.

If you need to stop the local server, press `CTRL + C` in the command line.

To actually see the code for this starter template, you can go into your project inside the `src` folder and you should see the `App.jsx` file.

From there you can start to modify the file, save your changes and see the new changes display in the browser.

And with that, you're ready to begin building your React application!

---

### Lecture 1.5: What Are Components In React And How Do They Work

# What Are Components in React, and How Do They Work?

Components are the building blocks of React applications that allow developers to break down complex user interfaces into smaller, manageable pieces, making it easier to develop and maintain large-scale applications.

The two types of components in React are functional and class-based components. In modern React, developers will use functional components and all of the examples we look at today will be functional components.

At a higher level, you can think of components like JavaScript functions that return elements describing the UI.

This UI is described using JSX, a syntax extension for JavaScript that looks similar to HTML but allows you to write UI elements in a more declarative way.

Let's look at an example of a React component:

```
function Greeting() {
  const name = "John"
  {/* The result will be Hello John*/}
  return <h1 className="title">Hello {name}</h1>;
}
```

In this example, we've defined a component called `Greeting`. The curly braces `{}` inside the `h1` tags enable us to embed JavaScript expressions, allowing us to access the `name` variable within the `h1` element.

We are also applying a `className` called `title` to the `h1` element.

But why are we using `className` instead of `class` like with regular HTML elements?

Well, this is because in JavaScript, `class` is a reserved name. So, we need to use `className` instead.

We are also using a comment in JSX showing what the result will be. It is important to note that you can use regular comment syntax like this but it needs to be wrapped in curly braces in order for it to work:

```
{/* Block Comments */}
```

Another thing you might have noticed is that we are using a capital letter at the beginning of the component name. But why can’t we use all lower case letters?

This is because React treats components with a capital letter as custom components, while elements with lowercase letters are considered built-in HTML elements.

When React encounters a lowercase tag, like `<div>` or `<span>`, it assumes it's a standard HTML element. However, if the component name starts with a capital letter, React will treat it as a user-defined component and render it accordingly. This distinction helps React differentiate between native HTML tags and components that you create.

To use this `Greeting` component in our application, we would write something like this:

```
<Greeting />
```

This would render an `h1` element with the text `Hello John` to the page. But take a closer look at the syntax here. When we use the component, it ends with a forward slash and then the greater than symbol.

When working with JSX, all tags and uses of components need to be explicitly closed. So if the component or tag does not have any children, then you need to explicitly close it like shown here:

```
<Greeting /> {/* /> is required */}
```

So far we have only been looking at how to render a single `h1` element. But you can actually render multiple elements.

Let’s take a look at the following example code here:

```
function Greeting() {
  const name = "John";
  {/* This will throw an error */}
  return <h1>Hello {name}</h1> 
  <p>Nice to meet you.</p>
}
```

We are trying to add another sentence of `Nice to meet you` but it is not rendering on the page correctly.

There seems to be an error message instead. The error message says `Adjacent JSX elements must be wrapped in an enclosing tag.`

The reason why you are getting that error message is because multiple sibling elements need to be wrapped in a parent element. While you could wrap the `h1` and `p` elements in a simple `div`, there is another way to silence the error.

React fragments are used to group elements together. Here is what the revised example will look like:

```
function Greeting() {
  const name = "John";
  return (
    <Fragment>
      <h1>Hello {name}</h1>
      <p>Nice to meet you.</p>
    </Fragment>
  );
}
```

You can also choose to use empty JSX tags which can serve as shorthand for fragments:

```
function Greeting() {
  const name = "John";
  return (
    <>
      <h1>Hello {name}</h1>
      <p>Nice to meet you.</p>
    </>
  );
}
```

In future lessons, we will continue to learn more about how to work with components and JSX. But for now, you've gained a solid introduction to building user interfaces with components, setting a strong foundation for what's to come.

---

### Lecture 1.6: How Can You Import And Export Components In React

# How Do Default and Named Exports Work in React Components?

In earlier lessons, you learned how to work with imports and exports in JavaScript. In this lesson, we will take a look at how to import and export components in React.

An export makes a component available to other files. An import allows a file to use a component that was exported elsewhere. In React projects, this is how components are reused and combined to build user interfaces.

In this lesson, you will learn how to export React components using default exports and named exports, and how to import them where they are needed.

In this example, we have a `Cat` component that belongs in a file called `Cat.jsx`. For the file extension, we are using the `.jsx` file extension because this file is mainly working with JSX.

This `Cat` component returns a JSX markup with a title and image for a cat called Mr. Whiskers:

```
function Cat() {
  return (
    <div className="card">
      <h2>Mr. Whiskers</h2>
      <img
        src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg"
        alt="Tuxedo cats running on dirt ground."
      />
    </div>
  );
}
```

If we want to use our `Cat` component in another file, we need to first export it like this:

```
function Cat() {
  return (
    <div className="card">
      <h2>Mr. Whiskers</h2>
      <img
        src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg"
        alt="Tuxedo cats running on dirt ground."
      />
    </div>
  );
}

export default Cat;
```

We are using the `default` keyword because this will be the default export from the module. You can also choose to export the component on the same line as the component definition like this:

```
export default function Cat() {
  return (
    <div className="card">
      <h2>Mr. Whiskers</h2>
      <img
        src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg"
        alt="Tuxedo cats running on dirt ground."
      />
    </div>
  );
}
```

You can choose to import child components in other parent component files, or import them in the root component file. For this example, we will import the `Cat` component inside the root component file.

Every React project will have a top-level component, typically called `App.jsx`:

```
export default function App() {
  return (
    // return component here
  );
}
```

This file is usually located in the `src` directory of your project. You’ll learn more about common project layouts in a future lesson.

To use the `Cat` component inside the root `App` component, you will need to import it like this:

```
import Cat from "./Cat";

export default function App() {
  return (
    // return component here
  );
}
```

Now, you can return the `Cat` component inside the `App` component like this:

```
import Cat from "./Cat";

export default function App() {
  return (
    <Cat />
  );
}
```

This approach works well when a file is responsible for exporting a single main component, keeping the import syntax simple and easy to read. Remember, a file can only have one default export, which makes it ideal for a file that primarily contains a single component.

Now that you know how to use default exports, let's look at named exports. Named exports allow a file to share multiple components or functions. Unlike default exports, these must be imported using the exact name they were exported with (unless you rename them using `as` term).

This is useful when a file serves as a library of components. For example, here is a file containing two components, Cat and Dog:

```
// Animals.jsx
export function Cat() {
  return <h2>Mr. Whiskers</h2>;
}

export function Dog() {
  return <h2>Fido</h2>;
}
```

We use the export keyword individually on each component. To use these in another file, we import them using curly braces:

```
import { Cat, Dog } from "./Animals";

export default function App() {
  return (
    <div>
      <Cat />
      <Dog />
    </div>
  );
}
```

The `{ Cat, Dog }` syntax tells JavaScript to import the specific named exports from the `Animals.jsx` file. The names inside the curly braces must match the exported names exactly. If you need to avoid naming conflicts, or if you prefer a different name in the current file, you can rename a component during import using the as keyword.

```
import { Cat as Kitty } from "./Animals";

export default function App() {
  return <Kitty />;
}
```

Finally, a file can have one default export and multiple named exports.

```
// Animals.jsx
export default function Cat() {
  return <h2>Mr. Whiskers</h2>;
}

export function Dog() {
  return <h2>Fido</h2>;
}
```

When importing mixed exports, the default export comes first (without braces), followed by the named exports (inside braces):

```
// App.jsx
import Cat, { Dog } from "./Animals";

export default function App() {
  return (
    <div>
      <Cat />
      <Dog />
    </div>
  );
}
```

In this example, `Cat` is the default export, so it does not use curly braces. `Dog` is a named export, so it requires them.

By understanding how default and named exports work, you can organize React components across multiple files and reuse them where needed. As you build larger applications, choosing the right export style will help keep your code clear and maintainable, and make it easier to work with components created by others.

---

### React Basics

# React Basics Review

JavaScript Libraries and Frameworks
-----------------------------------

* JavaScript libraries and frameworks offer quick solutions to common problems and speed up development by providing pre-built code.
* Libraries are generally more focused on providing solutions to specific tasks, such as manipulating the DOM, handling events, or managing AJAX requests.
* A couple of examples of JavaScript libraries are jQuery and React.
* Frameworks, on the other hand, provide a more defined structure for building applications. They often come with a set of rules and conventions that developers need to follow.
* Examples of frameworks include Angular and Next.js, a meta framework for React.
* **Single page applications** (SPAs) are web applications that load a single HTML page and dynamically update that page as the user interacts with the application without reloading the entire page.
* SPAs use JavaScript to manage the application's state and render content. This is often done using frameworks which provide great tools for building complex user interfaces.
* Some issues surrounding SPAs include:

  + Screen readers struggle with dynamically updated content.
  + The URL does not change when the user navigates within the application, which can make it difficult to bookmark, backtrack or share specific pages.
  + Initial load time can be slow if the application is large as all the assets need to be loaded upfront.

React
-----

* React is a popular JavaScript library for building user interfaces and web applications.
* A core concept of React is the creation of reusable UI components that can update and render independently as data changes.
* React allows developers to describe how the UI should look like based on the application state. React then updates and renders the right components when the data or the state changes.

React Components
----------------

* Components are the building blocks of React applications that allow developers to break down complex user interfaces into smaller, manageable pieces.
* The UI is described using JSX, an extension of JavaScript's syntax, that allows developers to write HTML-like code within JavaScript.
* Components are basically JS functions or classes that return a piece of UI.

Here is an example of a simple React component that renders a greeting message:

```
function Greeting() {
  const name = 'Anna';
  return <h1>Welcome, {name}!</h1>;
}
```

To use the component, you can simply call:

```
  <Greeting />
```

Importing and Exporting React components
----------------------------------------

* An export makes a component available to other files. An import allows a file to use a component that was exported elsewhere.
* There are two types of exports in React: default exports and named exports.

**Default Exports**

* A file can only have one default export. It is ideal for a file that primarily contains a single component.
* You can export a component as a default export like this:

```
// City.js
function City() {
  return <p>New York</p>;
}

export default City;
```

* You can also export on the same line as the component definition:

```
export default function City() {
  return <p>New York</p>;
}
```

* To import a default export, use the `import` keyword without curly braces:

```
// App.js
import City from './City';

function App() {
  return (
    <div>
      <h1>My favorite city is:</h1>
      <City />
    </div>
  );
}
```

**Named Exports**

* Named exports allow a file to share multiple components. Unlike default exports, they must be imported using the exact name they were exported with.
* You can export multiple components from the same file like this:

```
// Animals.jsx
export function Cat() {
  return <h2>Mr. Whiskers</h2>;
}

export function Dog() {
  return <h2>Fido</h2>;
}
```

* To import named exports, use curly braces with the exact exported names:

```
import { Cat, Dog } from './Animals';
```

* You can rename a named export during import using the `as` keyword:

```
import { Cat as Kitty } from './Animals';
```

**Mixed Default and Named Exports**

* A file can have one default export and multiple named exports at the same time:

```
// Animals.jsx
export default function Cat() {
  return <h2>Mr. Whiskers</h2>;
}

export function Dog() {
  return <h2>Fido</h2>;
}
```

* When importing mixed exports, the default export comes first (without braces), followed by named exports (inside braces):

```
import Cat, { Dog } from './Animals';
```

Setting up a React project using Vite
-------------------------------------

* Project setup tools and CLIs provide a quick & easy way to start new projects, allowing developers to focus on writing code rather than dealing with configuration.
* Vite is a popular project setup tool and can be used with React.
* To create a new project with Vite, you can use the following command in your terminal:

```
npm create vite@latest my-react-app -- --template react
```

This command creates a new React project named `my-react-app` using Vite's React template. In the project directory, you will see a `package.json` file with the project dependencies and commands listed in it.

* To run the project, navigate to the project directory and run the following commands:

```
cd my-react-app # path to the project directory
npm install # installs the dependencies listed in the package.json file
```

* Once the dependencies are installed, you should notice a new folder in your project called `node_modules`.
* The `node_modules` folder is where all the packages and libraries required by your project are stored.
* To run your project, use the following command:

```
npm run dev
```

* After that, open your browser and navigate to `http://localhost:5173` to see your React application running.
* To actually see the code for the starter template, you can go into your project inside the `src` folder and you should see the `App.jsx` file.

Passing props in React components
---------------------------------

* In React, props (short for properties) are a way to pass data from a parent component to a child component. This mechanism is needed to create reusable and dynamic UI elements.
* Props can be any JavaScript value. To pass props from a parent to a child component, you add the props as attributes when you use the child component in the parent's JSX. Here's a simple example:

```
// Parent component
function Parent() {
  const name = 'Anna';
  return <Child name={name} />;
}

// Child component
function Child(props) {
  return <h1>Hello, {props.name}!</h1>;
}
```

You can pass multiple props using the spread operator `(...)`, after converting them to an object. Here's an example:

```
// Parent component
function Parent() {
  const person = {
    name: 'Anna',
    age: 25,
    city: 'New York'
  };
  return <Child {...person} />;
}
```

In this code, the spread operator `{...person}` converts the person object into individual props that are passed to the Child component.

Conditional rendering in React
------------------------------

* Conditional rendering in React allows you to create dynamic user interfaces. It is used to show different content based on certain conditions or states within your application.
* There are several ways to conditionally render content in React. One common approach is to use the ternary operator. Here's an example:

```
function Greeting({ isLoggedIn }) {
  return (
    <div>
      {isLoggedIn ? <h1>Welcome back!</h1> : <h1>Please log in</h1>}
    </div>
  );
}
```

* Another way to conditionally render content is to use the logical AND (`&&`) operator. This is useful when you want to render content only if a certain condition is met. Here's an example:

```
function Greeting({ user }) {
  return (
    <div>
      {user && <h1>Welcome, {user.name}!</h1>}
    </div>
  );
}
```

In the code above, the `h1` element is only rendered if the user object is truthy.

You can also use a direct `if` statement this way:

```
function Greeting({ isLoggedIn }) {
  if (isLoggedIn) {
    return <h1>Welcome back!</h1>;
  }
  return <h1>Please sign in</h1>;
}
```

Rendering lists in React
------------------------

* Rendering lists in React is a common task when building user interfaces.
* Lists can be rendered using the JS array `map()` method to iterate over an array of items and return a new array of JSX elements.
* For example, if you have an array of names that you want to render as a list, you can do the following:

```
function NameList({ names }) {
  return (
    <ul>
      {names.map((name, index) => (
        <li key={`${name}-${index}`}>{name}</li>
      ))}
    </ul>
  );
}
```

* Always remember to provide a unique key for each list item to help React manage the updating and rendering roles. With these techniques, you can create flexible, efficient, and dynamic lists in your React applications.

Inline styles in React
----------------------

* Inline styles in React allow you to apply CSS styles directly to JSX elements using JavaScript objects.
* To apply inline styles in React, you can use the style attribute on JSX elements. The style attribute takes an object where the keys are CSS properties in camelCase and the values are the corresponding values. Here's an example:

```
function Greeting() {
  return (
    <h1
      style={{ color: 'blue', fontSize: '24px', backgroundColor: 'lightgray' }}
    >
      Hello, world!
    </h1>
  );
}

export default Greeting;
```

You can also extract the styles into a separate object and reference it in the `style` attribute this way:

```
function Greeting() {
  const styles = {
    color: 'blue',
    fontSize: '24px',
    backgroundColor: 'lightgray'
  };

  return <h1 style={styles}>Hello, world!</h1>;
}

export default Greeting;
```

* Inline styles support dynamic styling by allowing you to conditionally apply styles based on props or state. Here is an example of how you can conditionally apply styles based on a prop:

```
function Greeting({ isImportant }) {
  const styles = {
    color: isImportant ? 'red' : 'black',
    fontSize: isImportant ? '24px' : '16px'
  };

  return <h1 style={styles}>Hello, world!</h1>;
}

export default Greeting;
```

* In the code above, the `color` and `fontSize` styles are conditionally set based on the `isImportant` prop.

---

## Module 2: Styling and Styling Architecture

### Lecture 2.1: What Is A Css Framework And What Are Some Advantages And Disadvantages Of Using It

# What Is a CSS Framework, and What Are Some Advantages and Disadvantages of Using It?

As you work CSS, you may experience certain challenges, such as keeping the styles consistent and compatible across browsers, avoiding repetition, and handling the growing complexity and number of CSS files across your project. CSS frameworks are very helpful to prevent these issues from the start.

A CSS framework consists of pre-written CSS code that you can use to style your HTML elements.

By using a CSS framework, you can speed up your workflow, create a uniform visual style across the website, make your design look consistent across multiple browsers, and overall keep your CSS code more organized.

You can think of a CSS framework as toolbox, where you can quickly find a style or component that fits your needs and use it right away, without having to specify it yourself using CSS properties. These frameworks often include pre-defined styles and components that you can use very easily, including styles for creating responsive layouts.

Some of the most popular CSS frameworks are Tailwind CSS, Bootstrap, Materialize, and Foundation.

Let's talk a little bit about the two types of CSS frameworks: utility-first CSS frameworks, and component-based CSS frameworks.

Tailwind CSS is a utility-first CSS framework. This means that it has small classes with very specific purposes, like setting the margin, padding, or background color. You can usually assign these small classes directly to the HTML elements.

For example:

```
<button class="bg-blue-500 text-white font-bold py-2 px-4 rounded-full hover:bg-blue-700">
  Button
</button>
```

This button will have a blue background with white and bold text, a vertical padding of 2 rem, a horizontal padding of 4 rem, and rounded borders. The class `hover:bg-blue-700` will turn the background dark blue when the user hovers over it with the mouse.

As you can see, Tailwind CSS classes are very granular, so they can be applied to individual HTML elements as needed.

In contrast, Bootstrap is a component-based CSS framework. It has pre-built components with pre-defined styles that you can easily add to your website. These components are usually available in the official documentation of the CSS framework, where you can copy and paste them quickly into your project.

For example, if you want to create a list group in Bootstrap, you would write something like this in HTML:

```
<div class="card" style="width: 25rem;">
  <ul class="list-group list-group-flush">
    <li class="list-group-item">HTML</li>
    <li class="list-group-item">CSS</li>
    <li class="list-group-item">JavaScript</li>
  </ul>
</div>
```

These pre-defined classes will automatically apply standard styles to the card, list group, and list group items.

Notice that here, instead of adding small and general classes, we are adding the entire component, including the HTML structure. This is why Bootstrap is component-based.

```
<div class="card" style="width: 25rem;">
  <ul class="list-group list-group-flush">
    <li class="list-group-item">HTML</li>
    <li class="list-group-item">CSS</li>
    <li class="list-group-item">JavaScript</li>
  </ul>
</div>
```

While CSS frameworks have many advantages, they also have certain disadvantages. It's important that you know both of them to make an informed decision.

Since CSS frameworks rely on pre-defined styles, if you try to add custom CSS on top them, specificity issues may arise. The selectors used by the framework may have a higher specificity than the selectors that you use in your custom CSS, so the correct style may not be displayed. To solve this, you will need to use a more specific CSS selector, so this may bring some additional challenges.

They can also limit uniqueness to a certain extent because their standard styles are used widely across many websites. However, this can be addressed by customizing the CSS with your unique styles.

And finally, you should consider potential performance issues that CSS frameworks might introduce. Some frameworks are quite large, and may take some time to load.

As a developer, you will decide if using a CSS framework is helpful for your project, if using entirely custom CSS is better, or perhaps a mix of both.

---

### Lecture 2.2: What Is The Value Of Using A Css Preprocessor And What Are Some Disadvantages

# What Is the Value of Using a CSS Preprocessor, and What Are Some Disadvantages?

A CSS preprocessor is a tool that extends standard CSS with powerful features like variables, mixins, nesting, and selector inheritance.

Some of these features, like variables and nesting, are now supported or are getting more support in native CSS, and this trend is very likely to continue. However, earlier versions of native CSS did not support these features.

That is why CSS preprocessors became so widely used in the first place. They take the CSS rules and styles you write, along with their extended syntax, and compile them into a native CSS file that browsers can understand.

By using a CSS preprocessor, you can structure your CSS code in a more reusable and logical way. You will also have access to powerful features, like mixins, that are not directly supported by CSS.

Some of the most popular CSS preprocessors are Sass, Less, and Stylus.

Let's talk about Sass.

Sass stands for "Syntactically Awesome Style Sheets." It's compatible with all versions of CSS and maintained by a large community of developers.

Sass supports features like:

* Variables, so you can store and reuse values throughout the spreadsheet.
* Nested CSS rules, so you can create a visual hierarchy in your file.
* Modules, so you can split your styles into multiple stylesheets.
* Mixins, so you can reuse CSS declarations throughout your site.
* Inheritance, so multiple CSS selectors can share properties.
* And operators, for basic mathematical operations.

Sass also supports two syntaxes.

The SCSS syntax stands for Sassy CSS, which is a superset of CSS. This means that SCSS expands the basic syntax of CSS.

SCSS is the most common syntax that you'll use and find when working with Sass. It requires the use of curly braces (`{` and `}`) around CSS properties and semicolons (`;`) at the end of CSS declarations, just like native CSS.

These files have a `.scss` extension. Here is an example:

```
$primary-color: #3498eb;

header {
  background-color: $primary-color;
}
```

What you see here, at the top, is a variable defined in SCSS. This variable is used in the CSS rule below.

Let's compare SCSS with a less-frequently used syntax, the indented syntax. This is also known as the "Sass syntax" since it was Sass's original syntax.

This syntax relies on indentation to define the rules. Here is an example:

```
$primary-color: #3498eb

header
  background-color: $primary-color
```

Notice that there are no curly braces around the CSS rule, or semi-colons at the end of CSS declarations. At the top, you can also see a variable. Notice that its name starts with a dollar sign (`$`) in this syntax, which is different than native CSS variables, but works very similarly.

Sass also supports a powerful feature, called mixins.

Mixins allow you to group multiple CSS properties and their values under the name and reuse that block of CSS code throughout your stylesheet.

This makes your CSS code less repetitive and easier to maintain because, if you change something in that block, the change is applied everywhere you use the mixin.

Since mixins can have custom and descriptive names, they can be helpful to understand what each block of CSS code does, which can make your stylesheets easier to understand.

And mixins also promote consistency in stylesheets by applying uniform styles.

This is an example of a mixin in SCSS syntax:

```
@mixin center-flex {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

To define a mixin, you start by writing the `@mixin` at-rule, followed by the name of the mixin. In this case, the mixin is called `center-flex`. It has three CSS properties to center elements using Flexbox.

Then, once you have your mixin defined, you would use the `@include` at-rule to include those properties in a CSS rule. You just need to write `@include` followed by the name of the mixin. In this case, the name is `center-flex`:

```
section {
  @include center-flex;
  height: 500px;
  background-color: #3289a8;
}
```

This is the full code with the mixin and the CSS rule:

```
@mixin center-flex {
  display: flex;
  justify-content: center;
  align-items: center;
}

section {
  @include center-flex;
  height: 500px;
  background-color: #3289a8;
}
```

You can include the mixin in as many CSS rules as needed. If you need to make any changes, you would only need to change the mixin itself and the changes would be applied everywhere automatically. This example is in SCSS syntax. Notice that it has the curly braces and the semicolons.

Here is the equivalent in indented syntax, also known as Sass syntax, without the curly braces or semicolons:

```
@mixin center-flex
  display: flex
  justify-content: center
  align-items: center

section
  @include center-flex
  height: 500px
  background-color: #3289a8
```

And this is the compiled CSS code, what the browser will actually interpret after the file is compiled into native CSS:

```
section {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 500px;
  background-color: #3289a8;
}
```

Notice that it includes the three mixin properties at the top: `display`, `justify-content`, and `align-items`.

This is only a simple example of what CSS preprocessors are capable of. They have many powerful features that are worth learning and applying in your daily workflow.

However, they do have potential disadvantages that you should be aware of.

First, CSS preprocessors have to compile the CSS rules into standard CSS. While the potential overhead of this compilation process is often minimal in terms of time and resources, it is something that you should consider for real-world projects.

Next, they can create debugging challenges, since browsers use the compiled CSS directly. Finding out what is generating a problematic style from the extended syntax can take a few extra steps when compared to standard CSS.

However, the advantages of CSS preprocessors usually outweigh their disadvantages, especially for complex projects. They can be very helpful for writing cleaner, reusable, less repetitive, and scalable CSS.

---

### Css Libraries And Frameworks

# CSS Libraries and Frameworks Review

CSS Frameworks
--------------

* **CSS frameworks**: CSS frameworks can speed up your workflow, create a uniform visual style across a website, make your design look consistent across multiple browsers, and keep your CSS code more organized.
* **Popular CSS frameworks**: Some of the popular CSS frameworks are Tailwind CSS, Bootstrap, Materialize, and Foundation.
* **Potential disadvantages**:
  + The CSS provided by the framework might conflict with your custom CSS.
  + Your website might look similar to other websites using the same framework.
  + Large frameworks might cause performance issues.

Two Types of CSS Frameworks
---------------------------

* **Utility-first CSS frameworks**: These frameworks have small classes with specific purposes, like setting the margin, padding, or background color. You can assign these small classes directly to the HTML elements as needed. Tailwind CSS is categorized as a utility-first CSS framework.

Here is an example of using Tailwind CSS to style a button.

```
<button class="bg-blue-500 text-white font-bold py-2 px-4 rounded-full hover:bg-blue-700">
  Button
</button>
```

* **Component-based CSS frameworks**: These frameworks have pre-built components with pre-defined styles that you can add to your website. The components are available in the official documentation of the CSS framework, and you can copy and paste them into your project. Bootstrap is categorized as a component-based CSS framework.

Here is an example of using Bootstrap to create a list group. Instead of applying small classes to your HTML elements, you will add the entire component, including the HTML structure.

```
<div class="card" style="width: 25rem;">
  <ul class="list-group list-group-flush">
    <li class="list-group-item">HTML</li>
    <li class="list-group-item">CSS</li>
    <li class="list-group-item">JavaScript</li>
  </ul>
</div>
```

Tailwind CSS
------------

Tailwind is a utility-first CSS framework. Instead of writing custom CSS rules, you build your designs by combining small utility classes directly in your HTML.

### Responsive Design Utilities

Tailwind uses prefixes such as `sm:`, `md:`, and `lg:` to apply styles at different screen sizes.

```
<div class="w-full md:w-1/2 lg:flex-row">Responsive layout</div>
```

### Flexbox Utilities

Classes like `flex`, `flex-col`, `justify-around`, and `items-center` make it easy to create flexible layouts.

```
<div class="flex flex-col md:flex-row justify-around items-center">
  <p>Column on small screens</p>
  <p>Row on medium and larger screens</p>
</div>
```

### Grid Utilities

Tailwind includes utilities for CSS Grid, like `grid`, `grid-cols-1`, and `md:grid-cols-3`.

```
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
  <div class="bg-gray-100 p-4">Column 1</div>
  <div class="bg-gray-100 p-4">Column 2</div>
  <div class="bg-gray-100 p-4">Column 3</div>
</div>
```

### Spacing Utilities

Utilities like `mt-8`, `mx-auto`, `p-4`, and `gap-4` help create consistent spacing without writing CSS.

```
<div class="mt-8 p-4 bg-indigo-600 text-white">Spaced content</div>
```

### Typography Utilities

Utilities like `uppercase`, `font-bold`, `font-semibold`, and `text-4xl` control text appearance.

You can set font sizes that adjust at breakpoints, such as `text-3xl` `md:text-5xl`.

```
<h1 class="text-3xl md:text-5xl font-semibold text-center">Responsive Heading
</h1>
```

### Colors and Hover States

Tailwind provides a wide color palette, such as `text-red-700`, `bg-indigo-600`, and `bg-gray-100`.

Classes like `hover:bg-pink-600` make interactive effects simple.

```
<a href="#" class="bg-pink-500 hover:bg-pink-600 text-white px-4 py-2 rounded-md">
  Hover Me
</a>
```

### Borders, Rings, and Effects

* **Borders**: `border-2 border-red-300` adds borders with specified thickness and colors.
* **Rings**: `ring-1 ring-gray-300` creates outline-like effects often used for focus or cards.
* **Rounded corners and scaling**: Classes like `rounded-md`, `rounded-xl`, and `scale-105` add polish.

```
<div class="p-6 rounded-xl ring-2 ring-fuchsia-500 scale-105">
  Highlighted card
</div>
```

### Gradients

Tailwind supports gradient utilities like `bg-gradient-to-r from-fuchsia-500 to-indigo-600`.

```
<div class="p-4 text-white bg-gradient-to-r from-fuchsia-500 to-indigo-600">
  Gradient background
</div>
```

CSS Preprocessors
-----------------

* **CSS preprocessor**: A CSS preprocessor is a tool that extends standard CSS. It compiles the code with extended syntax into a native CSS file. It can be helpful for writing cleaner, reusable, less repetitive, and scalable CSS for complex projects.
* **Features**: Some of the features that can be provided by CSS preprocessors are variables, mixins, nesting, and selector inheritance.
* **Popular CSS preprocessors**: Some of the popular CSS preprocessors are Sass, Less, and Stylus.
* **Potential disadvantages**:
  + Compiling the CSS rules into standard CSS might cause overhead.
  + The compiled code may be difficult to debug.

Sass
----

* **Sass**: It is one of the most popular CSS preprocessors. Sass stands for "Syntactically Awesome Style Sheets."
* **Features supported by Sass**: Sass supports features like variables, nested CSS rules, modules, mixins, inheritance, and operators for basic mathematical operations

Two Syntaxes Supported by Sass
------------------------------

* **SCSS syntax**: The SCSS (Sassy CSS) expands the basic syntax of CSS. It is the most widely used syntax for Sass. SCSS files have an `.scss` extension.

Here is an example of defining and using a variable in SCSS.

```
$primary-color: #3498eb;

header {
  background-color: $primary-color;
}
```

* **Indented syntax**: The indented syntax was Sass's original syntax and is also known as the "Sass syntax."

Here is an example of defining and using a variable in the indented syntax.

```
$primary-color: #3498eb

header
  background-color: $primary-color
```

### Mixins

* **Mixins**: Mixins allow you to group multiple CSS properties and their values under the name and reuse that block of CSS code throughout your stylesheet.

Here is an example of defining a mixin in SCSS syntax. In this case, the mixin is called `center-flex`. It has three CSS properties to center elements using flexbox.

```
@mixin center-flex {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

Here is an example of using the mixin you defined.

```
section {
  @include center-flex;
  height: 500px;
  background-color: #3289a8;
}
```

---

## Module 3: Core React Elements - Data, State, Rendering & Forms

### Lecture 3.1: How Do Inline Styles Work In React

# How Do Inline Styles Work in React?

In React, inline styles are used to apply CSS styles directly to React elements within your JSX code instead of defining them in separate CSS files.

React's approach to inline styles involves using JavaScript objects to define styles, rather than traditional CSS strings. This means that instead of writing styles as you would in a CSS file, you create a JavaScript object where the keys are camel cased versions of CSS property names, and the values are the strings of CSS values.

Here is an example of how you can use inline styles for a `Button` component:

```
function Button({ buttonText }) {
  const defaultStyles = {
    backgroundColor: "#007BFF",
    color: "white",
    border: "none",
    borderRadius: "4px",
    padding: "10px 20px",
    fontSize: "16px",
    fontWeight: "bold",
    cursor: "pointer",
    transition: "background-color 0.3s ease",
  };

  return <button style={defaultStyles}>{buttonText}</button>;
}
```

In this example, we define a style object called `defaultStyles`. We then apply these styles to a button element using the `style` attribute. React takes care of applying these styles to the element when it renders.

You can also choose to pass in an object directly to the `style` attribute. Here is what a revised example would look like:

```
function Button({ buttonText }) {
  return (
    <button
      style={{
        backgroundColor: "#007BFF",
        color: "white",
      }}
    >
      {buttonText}
    </button>
  );
}
```

Notice the double curly braces `{{}}` in the `style` attribute. The outer braces indicate a JavaScript expression in JSX, while the inner braces define a JavaScript object literal. This syntax allows you to embed JavaScript objects directly in JSX attributes.

Sometimes you might want to pass in an object directly if there are only a few properties like shown here. Otherwise, passing in a name to an object would be better like in the first example.

It's important to note that while CSS property names are typically written in kebab case, like `font-size`, in React's inline styles, we use camel case, like `fontSize`. This is because the style object is a JavaScript object, and kebab case names are not valid as object keys in JavaScript without using quotes.

A great advantage of inline styles in React is that they support dynamic styling based on a component state or props. For example:

```
function DynamicButton({ isActive }) {
  const buttonStyles = {
    backgroundColor: isActive ? "green" : "red",
    color: "white",
    padding: "10px 15px",
    border: "none",
    cursor: "pointer",
  };

  return <button style={buttonStyles}>Login</button>;
}
```

In this example, the button's background color changes based on the `isActive` prop. This kind of dynamic styling can be powerful for creating interactive and responsive user interfaces.

In summary, inline styles in React provide a powerful way to apply and manipulate styles directly within your components. They use JavaScript objects instead of CSS strings, require camel cased property names, and can easily incorporate dynamic values. They're an essential tool in a React developer's toolkit, especially for creating highly customized and interactive user interfaces.

---

### Lecture 3.2: How Do You Pass Props From A Parent Component To A Child Component In React

# How Do You Pass Props from a Parent Component to a Child Component in React?

In the previous lessons, we learned how to build small components in React like this:

```
function Greeting() {
  const developerName = "Jessica";
  return <h1>Hi {developerName}!</h1>;
}
```

We can choose to nest this component inside another parent component or the root component like this:

```
function App() {
  return <Greeting />;
}

function Greeting() {
  const developerName = "Jessica";
  return <h1>Hi {developerName}!</h1>;
}
```

While this code will run fine and display the result of `Hi Jessica!` on the screen, it is not that flexible of a component.

What if we wanted to display a different name like Naomi, Tom, or Oliver? This is where React props comes in. Props, which is short for properties, is the way for parent components to pass data down to the child component. Props can be of any type: strings, numbers, booleans, objects, or arrays.

Let's update our example from earlier to now accept a `name` prop:

```
function App() {
  return <Greeting name="Jessica" />;
}

export default App;

function Greeting(props) {
  console.log(props);
  return <h1>Hi {props.name}!</h1>;
}
```

For the child component called `Greeting` we are now using `props.name` instead of hardcoding the name `"Jessica"`. We are also logging `props` to the console which is showing as an object.

Then, inside of the parent `App` component, we are passing the value to the `name` prop so it can be passed down to the child. The result will be the same on the screen like earlier, but now we have created a more flexible component.

Now we have the ability to reuse the child component several times and pass in different names each time:

```
function App() {
  return (
    <>
      <Greeting name="Naomi" />
      <Greeting name="Tom" />
      <Greeting name="Jessica" />
      <Greeting name="Oliver" />
    </>
  );
}
```

You can also choose to use object destructuring in the props to make it more readable. Here's how you could rewrite the `Greeting` component:

```
function Greeting({ name }) {
  return <h1>Hi {name}!</h1>;
}
```

This code achieves the same result but makes it clearer which props the component is expecting to receive.

React also provides a special prop called `children`. Any JSX you place between a component's opening and closing tags is passed to the component as `children`.

For example:

```
function Card({ children }) {
  return <div className="card">{children}</div>;
}

function App() {
  return (
    <Card>
      <h2>Hello</h2>
    </Card>
  );
}
```

In this case, the JSX inside `<Card>...</Card>` becomes the `children` prop. The rendered output in the DOM will be:

```
<div class="card">
  <h2>Hello</h2>
</div>
```

This pattern is often used for component composition, where a component wraps other UI elements.

Sometimes, you can have a lot of properties that you have to pass as props. Instead of passing them one by one, you can use the spread operator (`...`), after converting them to an object.

Here is an example of a new child component called `DeveloperCard`:

```
function DeveloperCard({ name, age, country }) {
  return (
    <div className="developer-card">
      <h1>Developer: {name}</h1>
      <p>Age: {age}</p>
      <p>Country: {country}</p>
    </div>
  );
}
```

This `DeveloperCard` component accepts three props: `name`, `age`, and `country`.

In the parent `App` component, we can use the spread syntax to pass all the properties from an object as individual props to the child component:

```
function App() {
  const developerObj = {
    name: "Alice",
    age: 30,
    country: "USA",
  };

  return (
    <div className="App">
      <DeveloperCard {...developerObj} />
    </div>
  );
}
```

This is particularly useful when working with arrays of objects and passing multiple sets of properties to child components. For example, you might have a list of developers where each object in the array has the same structure but represents a different person.

You will learn more about how to render lists in arrays in future lessons.

Using props in React makes your components more flexible and reusable, allowing you to build more complex UIs. However, it's important to note that props are immutable, meaning they cannot be changed once passed to a component. If you need to handle user input and modify data, you should use state instead. You'll learn more about managing state in future lessons.

---

### Lecture 3.3: How Do You Render Lists In React

# How Do You Render Lists in React?

Rendering lists is a fundamental task in React web apps, and is used for displaying data to users. In React, the `map` method is used to transform an array of data into an array of JSX elements that can be rendered in the UI.

Here is an example of a component called `FruitList` that displays a list of fruits:

```
function FruitList() {
  const fruits = ['Apple', 'Banana', 'Cherry', 'Date'];
  return (
    <ul>
      {fruits.map(fruit => <li>{fruit}</li>)}
    </ul>
  );
}
```

In this example, the `map` function iterates over each item in the `fruits` array. For each fruit, it creates a new `li` element containing the fruit's name. The newly created array of `li` elements is then displayed inside the `ul` parent tags.

However, when rendering lists in React, it is important not to forget the `key` prop for each element in the list. The key must always be unique and it helps React identify which items have changed, been added, or been removed, which is essential for efficient rendering and updating the list.

If you forget the key, React will show a warning in the console, but it will not throw a fatal error. The application might still render and function, but you may encounter subtle bugs, especially when the list changes. These bugs can be difficult to debug because the UI might look correct initially.

A common mistake is to use the array index as the key, like this:

```
{fruits.map((fruit, index) => <li key={index}>{fruit}</li>)}
```

While this silences the warning, it is generally considered an anti-pattern. Using the index as a key can cause issues when the list is reordered, sorted, or filtered. React uses the key to track elements. If the list order changes, React might incorrectly reuse component state or fail to update the DOM efficiently because the keys (indexes) stay the same even if the content at that index has changed.

The best practice is to use a stable, unique identifier for each item. This is typically an ID from your database, like a UUID or a database ID.

If your data doesn't have a unique ID, you can generate one when the data is created (e.g., using `crypto.randomUUID()` or a library like `uuid`), or use a combination of fields that are guaranteed to be unique. However, you should avoid generating keys on the fly during rendering (e.g., `key={Math.random()}`), as this will cause React to recreate the DOM elements on every render and reset their state.

Let's modify our example to include keys:

```
function FruitList() {
  const fruits = ["Apple", "Banana", "Cherry", "Date"];
  return (
    <ul>
      {fruits.map((fruit, index) => (
        <li key={`${fruit}-${index}`}>{fruit}</li>
      ))}
    </ul>
  );
}
```

In this refactored example, we are creating a unique key for each list item by concatenating the fruit name with its index. This ensures that each list item has a distinct key, which helps React efficiently manage and update the list when items are added, removed, or reordered.

React also allows you to render more complex structures. For instance, you might have an array of objects representing users, each with multiple properties that you want to display:

```
function UserList() {
  const users = [
    { id: "user-001-employee", name: "Alice", email: "alice@example.com" },
    { id: "user-002-employee", name: "Bob", email: "bob@example.com" },
    { id: "user-003-employee", name: "John", email: "john@example.com" },
  ];
  return (
    <div>
      {users.map((user) => (
        <div key={user.id}>
          <h3>{user.name}</h3>
          <p>{user.email}</p>
        </div>
      ))}
    </div>
  );
}
```

In this example, we're creating a more complex JSX structure for each user, displaying both their name and email address. We're using the user's `id` as the `key`, which is a good practice.

In conclusion, rendering lists in React involves converting arrays of data into JSX elements, typically using the `map` function.

---

### Lecture 3.4: How Does Conditional Rendering Work In React Components

# How Does Conditional Rendering Work in React Components?

Conditional rendering in React allows you to create dynamic user interfaces. It is used to show different content based on certain conditions or states within your application.

The most common approaches of using conditional rendering includes using `if` statements, the ternary (`?:`) operator, and logical AND (`&&`) operator.

The simplest form of conditional rendering uses an `if` statement. Here's an example:

```
function Greeting({ isLoggedIn }) {
  if (isLoggedIn) {
    return <h1>Welcome back!</h1>;
  }
  return <h1>Please sign in</h1>;
}
```

In this example, the `Greeting` component checks the `isLoggedIn` prop. If it's `true`, it returns a welcome message, otherwise, it prompts the user to sign in.

Here is an example using the `Greeting` component inside of the parent `App` component:

```
function App() {
  return (
    <div className="App">
      <Greeting isLoggedIn={false} />
    </div>
  );
}
```

For simpler conditions, the ternary operator (`?:`) is often used directly within JSX. It allows for inline conditional rendering, which can make your code more concise:

```
function Greeting({ isLoggedIn }) {
  return <h1>{isLoggedIn ? "Welcome back!" : "Please sign in."}</h1>;
}
```

This code achieves the same result as the previous example but in a more compact form. The ternary operator checks `isLoggedIn` and renders the appropriate message.

Another common pattern for conditional rendering is using the logical AND (`&&`) operator. This is particularly useful when you want to render something, or nothing, based on a condition:

```
function Notification({ message }) {
  return (
    <div>
      {message && <p>{message}</p>}
    </div>
  );
}
```

In this example, the paragraph element with the message is only rendered if the `message` prop is truthy. If `message` is falsy - meaning it is an empty string, `null`, or `undefined`, nothing is rendered to the screen.

By mastering these techniques of conditional rendering, you can build more interactive and user-friendly applications that adapt to changing data and user interactions.

---

### Lecture 3.5: What Is Rendering In React And How Are Components Displayed On The Screen

# What Is Rendering in React, and How Are Components Displayed on the Screen?

In React, rendering is the process by which components appear in the user interface (UI), usually the browser.

React takes all your JavaScript, JSX, and CSS code, figures out how it should look, and then displays it in the user interface.

The rendering process consists of three stages: trigger, render, and commit. Let's take a look at these in more detail.

The trigger stage occurs when React detects that something has changed and that the user interface might need to be updated. This change is often due to an update in the state or props.

For instance, noticing that it's time for dinner can trigger you to go into the kitchen to start cooking.

In the `Counter` example below, clicking the increment or decrement button triggers React to show the new `count` value:

```
import { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <h1>{count}</h1>
      <button onClick={() => setCount(count - 1)}>Decrement</button>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </div>
  );
}

export default Counter;
```

Once the trigger happens, React enters the render stage. Here, React re-evaluates your components and figures out what to display.

To do this, React uses a lightweight copy of the "real" DOM. This is called the virtual DOM. With the virtual DOM, React can quickly check what needs to change in the component.

Think of this stage as the point where you're in the kitchen, you've gathered your ingredients, and you cook your dinner.

For the `Counter` component, the render stage is the point where React runs the functions again with the new `count` value. React recalculates what the `<h1>{count}</h1>` part of the component should look like based on the updated `count` value, but you won't see any changes on the screen until the next stage – commit.

The commit stage is where React takes the prepared changes from the virtual DOM and applies them to the real DOM. In other words, this is the stage where you see the final result on the screen.

To make this happen, React compares the virtual DOM to the actual DOM, identifies only the parts that need updates, and applies those changes to the real DOM to update the user interface.

You can think of this stage as the point where you serve the food you cooked, making it visible just like React does when it commits updates to the actual DOM.

As for the `Counter` component, the commit stage is the point in which the new `count` value is applied to the `h1` element, and you can see the change on the page.

These three processes are extremely fast because React minimizes direct DOM manipulation by calculating changes in the virtual DOM first, then it updates only the parts that need to change in the real DOM.

---

### Lecture 3.6: What Is State And How Does The Usestate Hook Work

# What is State, and How Does the useState Hook Work?

State is one of the most important fundamentals of React and other front-end frameworks. It's like the brain of a component, meaning it holds information that can change over time and controls how the components behave and look.

Let's look into what state is and how the `useState` hook lets you work with it.

State represents the dynamic data in your React component, like the value from a user input, data fetched from an API, or an item in a to-do list.

Whenever the state changes, React re-renders the component without reloading the page to reflect those changes in the user interface. This reactivity makes your app interactive.

The `useState` hook is a function that lets you declare state variables in functional components.

Before hooks, you could only use state in class components. But with the introduction of hooks since React 16.8, you can use state in functional components by using the `useState` hook.

To use the `useState` hook, you need to import it from React:

```
import { useState } from "react";
```

You can also import React itself and get access to the `useState` hook as a property:

```
import React from "react";
```

Here's how you can declare a state variable when you import `useState`:

```
const [stateVariable, setStateFunction] = useState(initialValue);
```

And here's how you can declare a state variable when you import React:

```
const [stateVariable, setStateFunction] = React.useState(initialValue);
```

In the state variable you have the following:

* `stateVariable` holds the current state value
* `setStateFunction` (the setter function) updates the state variable
* `initialValue` sets the initial state

Note that the state in a React component is private, and is isolated to each component instance. This means that, if you render the same component twice, the state component of one does not affect the other. This also means that, if you'd like to share state between components, then you'd need to lift the state up to a common parent and pass it down as props.

Another thing is that hooks must be called at the top level of a component, just before the `return` keyword, to keep the state and effects consistent across renders. This means you can't use state inside loops, conditions, or nested functions.

Here's an example of managing state with the `useState` hook in a `Counter` component:

```
// Importing the useState hook
import { useState } from "react";

function Counter() {
  const initialValue = 0;

  // The state variable and setter function
  const [count, setCount] = useState(initialValue);

  return (
    <div>
      {/* Display current state value */}
      <h2>{count}</h2>

      <button onClick={() => setCount(count - 1)}>Decrement</button>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </div>
  );
}

export default Counter;
```

In the code above, we have the `useState` hook imported from React. In the `Counter` component, the `count` represents the current state while `setCount` is the set function responsible for updating state. The current state value is `0`. The `return` statement contains the count and two buttons to decrement and increment the count by `1`.

You can manage multiple pieces of state by calling the `useState` hook multiple times. This is especially important when you have unrelated state variables:

```
function UserProfile() {
  const [isOnline, setIsOnline] = useState(false);
  const [notifications, setNotifications] = useState(0);

  // The rest of the component logic
}
```

You can also call the `useState` hook multiple times when managing multiple states that update separately, like form fields:

```
function SignUpForm() {
  const [name, setName] = useState("");
  const [username, setUsername] = useState("");
  const [email, setEmail] = useState("");

  // The rest of the component logic
}
```

But in this case, it's best to combine the states since they're all part of the same form:

```
function SignUpForm() {
  const [formData, setFormData] = useState({
    name: "",
    username: "",
    email: "",
  });

  // The rest of the component logic
}
```

That's what state is and how you can use the `useState` hook.

---

### Lecture 3.7: How Do Events Work In React

# How Do Events Work in React?

Event handling is an essential part of every interactive website.

React provides a powerful and consistent way to handle events through its Synthetic Event System, which is a wrapper around native events like `click`, `keydown`, and `submit` you learned about in earlier lessons.

This cross-browser wrapper ensures that events work the same across all browsers so there are no inconsistencies.

Let's see how events work in React so you can start using them in your projects.

In React, event handlers work in a similar way to native browser events, but with a few tweaks.

Instead of using lowercase event attribute names like `onclick` and `onsubmit`, React uses camelCase, like `onClick` and `onSubmit`.

In addition, instead of using strings to specify the kind of event, React expects a function for the event handler.

The event handler function is passed to the element as a prop, and the event type like `onClick` or `onSubmit` is used as an attribute in JSX.

Here is a reminder of how to work with a click event in regular HTML:

```
<button onclick="alert('Button clicked!')">Click Me</button>
```

And here is how you do the same in React:

```
function handleClick() {
  console.log("Button clicked!");
}

<button onClick={handleClick}>Click Me</button>;
```

In this example, `handleClick` logs a message to the console when the user clicks the button.

Note that you don't need parentheses after `handleClick` in the `onClick` attribute, as you're passing a reference to the function, not calling it.

In React, event handler functions usually start with the prefix `handle` to indicate they are responsible for handling events, like `handleClick` or `handleSubmit`.

When a user action triggers an event, React passes a Synthetic Event object to your handler. This object behaves much like the native event object in vanilla JavaScript, providing properties like `type`, `target`, and `currentTarget`.

You can pass `event` as a parameter to the handler function and log it to the console to take a look at its structure:

```
function handleClick(event) {
  console.log(event);
}
```

To prevent default behaviors like browser refresh during an `onSubmit` event, for example, you can call the `preventDefault()` method:

```
function handleSubmit(event) {
  event.preventDefault();
  console.log("Form submitted!");
}

<form onSubmit={handleSubmit}>
  <input type="text" />
  <button>Submit</button>
</form>;
```

You can also stop an event from bubbling up to parent elements by calling `event.stopPropagation()`.

Sometimes, while handling special cases like delete and edit features, you might want to pass extra data to an event handler. You can do this by wrapping the handler in an inline arrow function:

```
function handleDelete(id) {
  console.log("Deleting item:", id);
}

<button onClick={() => handleDelete(1)}>Delete Item</button>;
```

It's fine to use inline event handlers in React because React efficiently manages re-renders and avoids performance issues.

In vanilla JavaScript, inline event handlers can lead to performance issues by creating new functions on every render, as there is no virtual DOM to optimize the process.

---

### Lecture 3.8: How Do You Update Objects In State

# How Do You Update Objects in State?

Updating objects in state in React can be tricky if you're used to changing object property values directly.

React treats state as immutable, meaning you should not modify it directly.

Let's look at what happens if you try to change objects in React state directly, and then dive into the correct way to do it.

Let's say you have an object in your component state that represents a user's profile, and you want the user to update their age:

```
import { useState } from "react";

function Profile() {
  const [user, setUser] = useState({
    name: "John Doe",
    age: 31,
    city: "LA",
  });

  // Change user age directly
  const handleAgeChange = (e) => {
    user.age = e.target.value;
    console.log(user);
  };

  return (
    <div>
      <h1>User Profile</h1>
      <p>Name: {user.name}</p>
      <p>Age: {user.age}</p>
      <p>City: {user.city}</p>

      <h2>Update User Age </h2>
      <input type="number" value={user.age} onChange={handleAgeChange} />
    </div>
  );
}

export default Profile;
```

This code will not work because you're directly modifying the `user.age` property.

Even though `console.log(user)` will show the new age in the console, React won't re-render the component to show it in the user interface because you didn't use the setter function, `setUser`.

To update an object directly in the state, you need to use the setter function to create a new object with the updated value. For example:

```
const handleAgeChange = (e) => {
  setUser({
    age: e.target.value,
  });
};
```

That works. But if you look at the page now, the user's age gets updated, but the values for the name and city are lost.

This is because the new object you passed to the setter function only contained a key/value pair for `age`.

To prevent this from happening, you can copy the existing object first, then update only the property you want to update, in this case, `age`.

To do this, you can pass a special function called an updater function to your setter function, `setUser`. The updater function takes the pending state as an argument, here, called `prevUser`, and should return the next state:

```
const handleAgeChange = (e) => {
  setUser((prevUser) => {
    const updatedUser = { ...prevUser, age: e.target.value };
    console.log('Previous State:', prevUser);
    console.log('Updated State:', updatedUser);
    return updatedUser;
  });
};
```

As you can see, we create a new user object called `updatedUser` by using the spread syntax to copy the pending user object, `...prevUser`. We then update the age based on the form input and return `updatedUser` at the bottom of the function as the next state.

Now your project works as expected, and updates to the age input don't affect the user's name or city name. You can also see the previous and updated states in the console.

This is the ideal way to update an object in state, especially when you're not updating all the properties.

To update the remaining `name` and `city` properties, you can write them as separate setting functions and connect them to their respective inputs:

```
const handleNameChange = (e) => {
  setUser((prevUser) => ({
    ...prevUser,
    name: e.target.value,
  }));
};

const handleCityChange = (e) => {
  setUser((prevUser) => ({
    ...prevUser,
    city: e.target.value,
  }));
};
```

Or you can combine them into a single setter function like this:

```
const handleChange = (e) => {
  const { name, value } = e.target;
  setUser((prevUser) => ({
    ...prevUser,
    [name]: value,
  }));
};
```

To make this work, each input field has to have a `name` attribute.

Here's the full code now:

```
import { useState } from "react";

function Profile() {
  const [user, setUser] = useState({ name: "John Doe", age: 31, city: "LA" });

  const handleChange = (e) => {
    const { name, value } = e.target;

    setUser((prevUser) => ({...prevUser, [name]: value}));
  };

  return (
    <div>
      <h1>User Profile</h1>
      <p>Name: {user.name}</p>
      <p>Age: {user.age}</p>
      <p>City: {user.city}</p>

      <h2>Update User Age </h2>
      <input type="number" name="age" value={user.age} onChange={handleChange} />

      <h2>Update User Name </h2>
      <input type="text" name="name" value={user.name} onChange={handleChange} />

      <h2>Update User City </h2>
      <input type="text" name="city" value={user.city} onChange={handleChange} />
    </div>
  );
}

export default Profile;
```

---

### Lecture 3.9: How Do You Update Arrays In State

# How Do You Update Arrays in State?

In React, updating arrays in state is quite straightforward, but it can be easy to make a mistake, especially if you're coming from vanilla JavaScript where you can modify arrays directly.

In React, state is treated as immutable so it can recognize changes and make the proper updates to the user interface.

Let's look at how you can update arrays held in state in React.

One of the most common mistakes when updating arrays in a React state is to directly modify the array using methods like `push()`, `pop()`, or `splice()`. These methods mutate the original array, and React does not allow that.

React relies on a new array reference to detect changes, so directly modifying the array can prevent the component from re-rendering as expected.

Here's an example of using the `push()` method to add to an array in state, which won't work:

```
import { useState } from "react";

function ItemsList() {
  const [items, setItems] = useState([
    { id: 0, name: "Item 1" },
    { id: 1, name: "Item 2" },
    { id: 2, name: "Item 3" },
  ]);

  const addItem = () => {
    const newItem = { id: items.length + 1, name: `Item ${items.length + 1}` };
    items.push(newItem); // This modifies the original array
    setItems(items); // React will not detect this change
  };

  return (
    <div>
      <button onClick={addItem}>Add Item</button>
      <ul>
        {items.map((item) => (
          <li key={item.id}>{item.name}</li>
        ))}
      </ul>
    </div>
  );
}

export default ItemsList;
```

If you click the `Add Item` button, nothing happens in the user interface.

It might also be tempting to remove items from the array with the `pop()` method:

```
const removeItem = () => {
  items.pop(); // Modifies the original array
  setItems(items); // React will not detect this change, either
};
```

To update an array in state, the key is to create a new array, do your operations, and pass that to React, rather than mutate the existing array.

Because it's a new array, React will know that the state has been changed, and trigger a re-render.

Here's how you can add to the `items` array using the spread operator:

```
const addItem = () => {
  const newItem = {
    id: items.length + 1,
    name: `Item ${items.length + 1}`,
  };

  // Creates a new array
  setItems((prevItems) => [...prevItems, newItem]);
};
```

`[...prevItems, newItem]` creates a new array by copying all items in the existing `items` array held in state, then adds `newItem` at the end, which increments the `id` and the item number.

If you want to remove something from the array, you can use the `filter()` method, which returns a new array after filtering out whatever you want to remove:

```
const removeItem = (id) => {
  setItems((prevItems) => prevItems.filter((item) => item.id !== id));
};
```

Here's the full code:

```
import { useState } from "react";

function ItemsList() {
  const [items, setItems] = useState([
    { id: 0, name: "Item 1" },
    { id: 1, name: "Item 2" },
    { id: 2, name: "Item 3" },
  ]);

  const addItem = () => {
    const newItem = { id: items.length + 1, name: `Item ${items.length + 1}` };
    setItems((prevItems) => [...prevItems, newItem]); // Creates a new array
  };

  const removeItem = (id) => {
    setItems((prevItems) => prevItems.filter((item) => item.id !== id)); // Creates a new array
  };

  return (
    <div>
      <button onClick={addItem}>Add Item</button>
      <ul>
        {items.map((item) => (
          <li key={item.id}>
            {item.name}{" "}
            <button onClick={() => removeItem(item.id)}>Remove</button>
          </li>
        ))}
      </ul>
    </div>
  );
}

export default ItemsList;
```

Those are some common ways you can update an array in state.

---

### Lecture 3.10: How Do Forms Work In React

# How Do Forms Work in React?

Forms are fundamental to every web application because they let you handle user input, collect data, and trigger actions.

In React, forms are managed using state or refs, giving you full control over their behavior and validation. These two ways to manage forms are called "controlled" and "uncontrolled" input.

Let's look at what controlled and uncontrolled inputs are.

Controlled input is the most "React-like" way to handle form inputs. With controlled inputs, you store the input field value in state and update it through `onChange` events. This gives you complete control over the form data and allows instant validation and conditional rendering.

The process works like this: React maintains the form state with the `useState` hook, and you update it on every change. When a user types in an input field, the `onChange` event fires, updates the state, and React re-renders the component with the new value.

```
import { useState } from "react";

function App() {
  const [name, setName] = useState("");

  const handleChange = (e) => {
    setName(e.target.value);
  };

  const handleSubmit = (e) => {
    e.preventDefault();
    console.log(name);
  };

  return (
    <>
      <form onSubmit={handleSubmit}>
        <label htmlFor="name">Your name</label> <br />
        <input value={name} id="name" onChange={handleChange} type="text" />
        <button type="submit">Submit</button>
      </form> 
    </>
  );
}

export default App;
```

The benefits of controlled inputs include the following:

* Immediate access to the form data.
* You can implement instant validation.
* You can conditionally disable the submit button.
* You can control the input value programmatically.

Uncontrolled inputs on the other hand are seen more in traditional HTML forms. So, instead of handling the inputs through the `useState` hook, uncontrolled inputs in HTML maintain their own internal state with the help of the DOM.

Since the DOM controls the input values, what you need is to pull in the values of the input fields with ref. This approach requires less code and performs better because refs do not make React re-render.

Here's an example of uncontrolled inputs:

```
import { useRef } from "react";

function App() {
  const nameRef = useRef();

  const handleSubmit = (e) => {
    e.preventDefault();
    console.log(nameRef.current.value);
  };

  return (
    <form onSubmit={handleSubmit}>
      <label htmlFor="name">Your</label>{" "}
      <input type="text" ref={nameRef} id="name" />
      <button type="submit">Submit</button>
    </form>
  );
}

export default App;
```

One very noticeable advantage of uncontrolled inputs is that they require less code. They also perform better and feel more natural to React beginners who are familiar with HTML.

So, which should you use between controlled and uncontrolled inputs?

Use controlled inputs when you need dynamic form updates, real-time validation, or when you want to sync input values with state. They provide better control but require more re-renders.

Use uncontrolled inputs when you need simpler forms, want to access values only on submission, or when you're working with non-React code.

Regardless of which you use between controlled and uncontrolled inputs, here are some best practices you should adhere to while making forms in React:

* Always prevent the default form submission.
* Ensure you validate inputs before submission.
* Always provide clear feedback to users with loading, validation errors or other related states.

---

### Lecture 3.11: What Is The Useactionstate Hook And How Does It Work

# What Is the useActionState Hook, and How Does It Work?

React 19 came with two notable new features called server components and server actions.

From that version onwards, server components became the default in frameworks like Next.js that readily support them.

Server actions on the other hand, are functions that run on the server to allow form handling right on the server without the need for API endpoints.

A server action looks like this:

```
"use server";

async function submitForm(formData) {
  const name = formData.get("name");
  return { message: `Hello, ${name}!` };
}
```

This server action extracts a `name` field from a form and returns a string greeting that name.

To simplify state management for server actions and remove the need for client-side JavaScript for simple forms, the React team introduced the `useActionState` hook in version 19.

Let's take a closer look at this hook and see how it works.

The React documentation describes the `useActionState` hook as a hook that "allows you to update state based on the result of a form action."

But this doesn't mean that you can only use the `useActionState` hook with forms. You can also use it to manage button clicks and other events, as long as you have an action in place.

And keep in mind that, since `useActionState` is a hook, you cannot use it inside a server component.

Here's the basic syntax of the `useActionState` hook:

```
const [state, action, isPending] = useActionState(actionFunction, initialState, permalink);
```

* `state` is the current state the action returns.
* `action` is the function that triggers the server action.
* `isPending` is a boolean that indicates whether the action is currently running or not.
* The `actionFunction` parameter is the server action itself.
* `initialState` is the parameter that represents the starting point for the state before the action runs.
* `permalink` is an optional string that contains the unique page URL the form modifies.

To use the `useActionState` hook, make sure you have an action in place first. Let's use the action from the previous example for this, with a bit of a twist:

```
"use server";

export async function submitForm(_, formData) {
  const name = formData.get("name");

  const hour = new Date().getHours();
  let greeting;

  if (hour < 12) {
    greeting = "Good morning";
  } else if (hour < 18) {
    greeting = "Good afternoon";
  } else {
    greeting = "Good evening";
  }

  return { message: `${greeting}, ${name}` };
}
```

In your component, you then need to import the `useActionState` hook and call it at the top level of the component body (before the return statement) just like other hooks. You should also import the action:

```
"use client";

// Import the useActionState hook
import { useActionState } from "react";

// Import the submitForm action
import { submitForm } from "./actions/submitForm";

const Greeter = () => {

 // Initialize the hook
 const [state, submit, isPending] = useActionState(submitForm, {
   message: "",
 });

  return (
    <div className="flex flex-col items-center justify-center min-h-screen bg-gray-100 p-6">
      {/* Rest of component */}
    </div>
  );
};

export default Greeter;
```

Here's what the full code looks like with a bit of styling:

```
"use client";

import { useActionState } from "react";
import { submitForm } from "./actions/submitForm";

const Greeter = () => {
  const [state, submit, isPending] = useActionState(submitForm, {
    message: "",
  });

  return (
    <div className="flex flex-col items-center justify-center min-h-screen bg-gray-100 p-6">
      <form
        action={submit}
        className="bg-white p-6 rounded-2xl shadow-md w-full max-w-md"
      >
        <h2 className="text-2xl text-center font-semibold text-gray-700 mb-4">
          Greet Someone
        </h2>

        <input
          type="text"
          name="name"
          placeholder="Enter your name"
          required
          className="w-full p-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-green-400"
        />

        <button
          type="submit"
          disabled={isPending}
          className="w-full mt-4 p-3 bg-green-500 text-white font-semibold rounded-lg hover:bg-green-600 disabled:bg-gray-400 transition-all"
        >
          {isPending ? "Greeting..." : "Greet"}
        </button>

        {state.message && (
          <p className="mt-4 text-green-600 text-center font-medium">
            {state.message}
          </p>
        )}
      </form>
    </div>
  );
};

export default Greeter;
```

In the browser, you would see your form button change from `Greet` to `Greeting...` while the action `isPending` - and the greeting would show `Good morning, {name}`, `Good afternoon, {name}`, or `Good evening, {name}`, depending on what time of day the form was submitted.

Remember how we mentioned that you can also use the `useActionState` hook outside of a form?

In this example, we'll fetch five users from JSONPlaceholder with a button click:

```
"use server";

export async function getUsers() {
  const res = await fetch(
    "https://jsonplaceholder.typicode.com/users?_start=0&_limit=5/"
  );
  return await res.json();
}
```

Here's the styled UI:

```
"use client";

import { useActionState } from "react";
import { getUsers } from "./actions/getUsers";

export default function FetchUsers() {
  const [users, fetchAction, isPending] = useActionState(getUsers, []);

  return (
    <div className="p-6 max-w-lg mx-auto">
      <button
        onClick={fetchAction}
        disabled={isPending}
        className="px-4 py-2 cursor-pointer bg-green-500 text-white rounded-lg hover:bg-green-600 disabled:bg-gray-400 font-bold"
      >
        {isPending ? "Fetching Users..." : "Fetch Users"}
      </button>

      <ul className="mt-4 space-y-2">
        {users.map((user) => (
          <li key={user.id} className="p-3 bg-gray-100 rounded-lg">
            <p className="font-semibold">{user.name}</p>
            <p className="text-sm text-gray-600">{user.email}</p>
          </li>
        ))}
      </ul>
    </div>
  );
}
```

In the browser, you would see that the button text is never updated to `Fetching Users...` after it's clicked.

This happens because React treats data fetching and rendering as a higher priority than the `isPending` state, which blocks `isPending` in the process and throws an error.

To fix this issue, you need to wrap the action in `startTransition`:

```
"use client";

// import startTransition from React
import { useActionState, startTransition } from "react";
import { getUsers } from "./actions/getUsers";

export default function FetchUsers() {
  const [users, fetchAction, isPending] = useActionState(getUsers, []);

  return (
    <div className="p-6 max-w-lg mx-auto">
      <button
        {/* wrap fetchAction in startTransition */}
        onClick={() => startTransition(() => fetchAction())}
        disabled={isPending}
        className="px-4 py-2 bg-green-500 font-bold cursor-pointer text-white rounded-lg hover:bg-green-600 disabled:bg-gray-400"
      >
        {isPending ? 'Fetching Users...' : 'Fetch Users'}
      </button>

      <ul className="mt-4 space-y-2">
        {users.map((user) => (
          <li key={user.id} className="p-3 bg-gray-100 rounded-lg">
            <p className="font-semibold">{user.name}</p>
            <p className="text-sm text-gray-600">{user.email}</p>
          </li>
        ))}
      </ul>
    </div>
  );
}
```

If you're wondering what `startTransition` is, it's a function that tells React that a state update is of low-priority and can be interrupted. This keeps the UI responsive while handling asynchronous updates like server actions.

That's how to use the `useActionState` hook inside and outside a form.

---

### React State And Hooks

# React State and Hooks Review

Working with Events in React
----------------------------

* **Synthetic Event System**: This is React's way of handling events. It serves as a wrapper around the native events like the `click`, `keydown`, and `submit` events. Event handlers in React use the camel casing naming convention. (Ex. `onClick`, `onSubmit`, etc)

Here is an example of using the `onClick` attribute for a `button` element in React:

```
function handleClick() {
  console.log("Button clicked!");
}

<button onClick={handleClick}>Click Me</button>;
```

In React, event handler functions usually start with the prefix `handle` to indicate they are responsible for handling events, like `handleClick` or `handleSubmit`.

When a user action triggers an event, React passes a Synthetic Event object to your handler. This object behaves much like the native Event object in vanilla JavaScript, providing properties like `type`, `target`, and `currentTarget`.

To prevent default behaviors like browser refresh during an `onSubmit` event, for example, you can call the `preventDefault()` method:

```
function handleSubmit(event) {
  event.preventDefault();
  console.log("Form submitted!");
}

<form onSubmit={handleSubmit}>
  <input type="text" />
  <button>Submit</button>
</form>;
```

You can also wrap a handler function in an arrow function like this:

```
function handleDelete(id) {
  console.log("Deleting item:", id);
}

<button onClick={() => handleDelete(1)}>Delete Item</button>;
```

Working with State and the `useState` Hook
------------------------------------------

* **Definition for state**: In React, state is an object that contains data for a component. When the state updates the component will re-render. React treats state as immutable, meaning you should not modify it directly.
* **`useState()` Hook**: The `useState` hook is a function that lets you declare state variables in functional components. Here is the basic syntax:

```
const [stateVariable, setStateFunction] = useState(initialValue);
```

In the state variable you have the following:

* `stateVariable` holds the current state value
* `setStateFunction` (the setter function) updates the state variable
* `initialValue` sets the initial state

Here is a complete example for a `Counter` component:

```
import { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <h2>{count}</h2>

      <button onClick={() => setCount(count - 1)}>Decrement</button>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </div>
  );
}

export default Counter;
```

Rendering and React Components
------------------------------

* **Definition**: In React, rendering is the process by which components appear in the user interface (UI), usually the browser. The rendering process consists of three stages: trigger, render, and commit.

The trigger stage occurs when React detects that something has changed and the user interface (UI) might need to be updated. This change is often due to an update in state or props.

Once the trigger happens, React enters the render stage. Here, React re-evaluates your components and figures out what to display. To do this, React uses a lightweight copy of the "real" DOM called the virtual DOM. With the virtual DOM, React can quickly check what needs to change in the component.

The commit stage is where React takes the prepared changes from the virtual DOM and applies them to the real DOM. In other words, this is the stage where you see the final result on the screen.

Updating Objects and Arrays in State
------------------------------------

* **Updating Objects in State**: If you need to update an object in state, then you should make a new object or copy an existing object first, then set the state for that new object. Any object put into state should be considered as read-only. Here is an example of setting a user's name, age and city. The `handleChange` function is used to handle updates to the user's information:

```
import { useState } from "react";

function Profile() {
  const [user, setUser] = useState({ name: "John Doe", age: 31, city: "LA" });

  const handleChange = (e) => {
    const { name, value } = e.target;

    setUser((prevUser) => ({...prevUser, [name]: value}));
  };

  return (
    <div>
      <h1>User Profile</h1>
      <p>Name: {user.name}</p>
      <p>Age: {user.age}</p>
      <p>City: {user.city}</p>

      <h2>Update User Age </h2>
      <input type="number" name="age" value={user.age} onChange={handleChange} />

      <h2>Update User Name </h2>
      <input type="text" name="name" value={user.name} onChange={handleChange} />

      <h2>Update User City </h2>
      <input type="text" name="city" value={user.city} onChange={handleChange} />
    </div>
  );
}

export default Profile;
```

* **Updating Arrays in State**: When updating arrays in state, it is important not to directly modify the array using methods like `push()` or `pop()`. Instead you should create a new array when updating state:

```
const addItem = () => {
  const newItem = {
    id: items.length + 1,
    name: `Item ${items.length + 1}`,
  };

  // Creates a new array
  setItems((prevItems) => [...prevItems, newItem]);
};
```

If you want to remove items from an array, you should use the `filter()` method, which returns a new array after filtering out whatever you want to remove:

```
const removeItem = (id) => {
  setItems((prevItems) => prevItems.filter((item) => item.id !== id));
};
```

Referencing Values Using Refs
-----------------------------

* **`ref` Attribute**: You can access a DOM node in React by using the `ref` attribute. Here is an example to showcase a `ref` to focus an `input` element. The `current` property is used to access the current value of that `ref`:

```
import { useRef } from "react";

const Focus = () => {
  const inputRef = useRef(null);

  const handleFocus = () => {
    if (inputRef.current) {
      inputRef.current.focus();
    }
  };

  return (
    <div>
      <input ref={inputRef} type="text" placeholder="Enter text" />
      <button onClick={handleFocus}>Focus Input</button>
    </div>
  );
};

export default Focus;
```

Working with the `useEffect` Hook
---------------------------------

* **`useEffect()` Hook**: In React, an effect is anything that happens outside the component rendering process. That is, anything React does not handle directly as part of rendering the UI. Common examples include fetching data, updating the browser tab's title, reading from or writing to the browser's local storage, getting the user's location, and much more. These operations interact with the outside world and are known as side effects. React provides the `useEffect` hook to let you handle those side effects. `useEffect` lets you run a function after the component renders or updates.

```
import { useEffect } from "react";

useEffect(() => {
 // Your side effect logic (usually a function) goes here
}, [dependencies]);
```

The effect function runs after the component renders, while the optional `dependencies` argument controls when the effect runs.

Note that `dependencies` can be an array of "reactive values" (state, props, functions, variables, and so on), an empty array, or omitted entirely. Here's how all of those options control how `useEffect` works:

* If `dependencies` is an array that includes one or more reactive values, the effect will run whenever they change.
* If `dependencies` is an empty array, `useEffect` runs only once when the component first renders.
* If you omit `dependencies`, the effect runs every time the component renders or updates.

How to Create Custom Hooks
--------------------------

* **Custom Hooks**: A custom hook allows you to extract reusable logic from components, such as data fetching, state management, toggling, and side effects like tracking online status. In React, all built-in hooks start with the word `use`, so your custom hook should follow the same convention.

Here is an example of creating a `useDebounce` hook:

```
function useDebounce(value, delay) {
  const [debouncedValue, setDebouncedValue] = useState(value);

  useEffect(() => {
    const handler = setTimeout(() => {
      setDebouncedValue(value);
    }, delay);

    return () => {
      clearTimeout(handler);
    };
  }, [value, delay]);

  return debouncedValue;
}

export { useDebounce };
```

---

## Module 4: Advanced React & State Management Strategies

### Lecture 4.1: What Are Effects In React And How Does The Useeffect Hook Work

# What Are Effects in React, and How Does the useEffect Hook Work?

In React, an effect is anything that happens outside the component rendering process. That is, anything React does not handle directly as part of rendering the UI.

Common examples include fetching data, updating the browser tab's title, reading from or writing to the browser's local storage, getting the user's location, and much more. These operations interact with the outside world and are known as side effects.

React provides the `useEffect` hook to let you handle those side effects. `useEffect` lets you run a function after the component renders or updates.

Let's see how the `useEffect` hook works and why it's essential for modern React development.

To use the `useEffect` hook, you first need to import it:

```
import { useEffect } from "react";
```

Then you use it as a function, like this:

```
useEffect(() => {
  // Your side effect logic (usually a function) here
}, [dependencies]);
```

The effect function runs after the component renders, while the optional `dependencies` argument controls when the effect runs.

Note that `dependencies` can be an array of "reactive values" (state, props, functions, variables, and so on), an empty array, or omitted entirely. Here's how all of those options control how `useEffect` works:

* If `dependencies` is an array that includes one or more reactive values, the effect will run whenever they change.
* If `dependencies` is an empty array, `useEffect` runs only once when the component first renders.
* If you omit `dependencies`, the effect runs every time the component renders or updates.

For example, in this `Counter` application, we don't pass in a `dependencies` argument, so the effect runs when the component renders and every time it updates:

```
import { useState, useEffect } from "react";

const Counter = () => {
  const [count, setCount] = useState(0);

  useEffect(() => {
    console.log("Component renders");
  });

  return (
    <div
      style={{
        display: "flex",
        alignItems: "center",
        flexDirection: "column",
      }}
    >
      <h2>{count}</h2>
      <div>
        <button onClick={() => setCount(count + 1)}>Increase</button>
        <button onClick={() => setCount(count - 1)}>Decrease</button>
      </div>
    </div>
  );
};

export default Counter;
```

But if we pass in an empty array as a dependency, the effect only runs on the first render:

```
useEffect(() => {
  console.log('Component renders');
}, []);
```

If you pass in the `count` state as a dependency, the effect runs when the component first renders, and when `count` changes:

```
useEffect(() => {
  document.title = `The current count is ${count}`;
  console.log('component renders');
}, [count]);
```

Note that, if the effect you set up persists beyond the component's rendering lifecycle, you might need another function to "clean up" that function after the component renders or updates.

For example, if your effect function uses `setInterval()`, sets an event listener like `window.addEventListener()`, or connects to a server, you'll need a cleanup function to run `clearInterval()`, `window.removeEventListener()`, and disconnect from the server, respectively.

Here's the syntax for returning a cleanup function from the `useEffect` hook:

```
useEffect(() => {
  // Your side effect logic here
  return () => {
    // Cleanup logic here (optional)
  };
}, [dependencies]);
```

For instance, if you add a scroll event listener, you can clean it up by removing it in your cleanup function:

```
useEffect(() => {
  const handleScroll = () => {
    // Handle scroll logic
  };
  window.addEventListener("scroll", handleScroll);

  return () => {
    window.removeEventListener("scroll", handleScroll);
  };
}, []);
```

---

### Lecture 4.2: How Do You Reference Values Using Refs

# How Do You Reference Values Using Refs?

In React, there may be situations where you need direct access to a DOM element. That's where "refs" come in handy. Refs can also store mutable values, but state is a better choice for that.

In vanilla JavaScript, you used the `getElementById()` and `querySelector()` methods to access DOM elements. But in React, you use refs to access elements in the DOM.

One of the main differences is that, with refs, you don't need identifiers like IDs and classes to reference elements.

So, how can you create and use refs? React provides a `useRef()` hook that lets you do just that.

The first step is to import the hook from React:

```
import { useRef } from "react";
```

Next, you need to create a variable that holds the ref with the initial value of the ref inside the `useRef` hook, say a `sectionRef` initialized to `null`:

```
const sectionRef = useRef(null);
```

The final thing to do is to attach the ref variable to the element in your JSX by using the `ref` attribute:

```
<section ref={sectionRef}>
  {/* Section content */}
</section>
```

If you log the ref to the console, you'll see it's an object with the current value, in this case, `null`:

```
console.log(sectionRef); // { current: null }
```

You can also log the current value to the console with the `current` property so you can see the value directly:

```
console.log(sectionRef.current); // null
```

The subsequent values of the ref depend on the component lifecycle.

For example, the initial value of `sectionRef` will always be `null` because that's what it was initialized to. After the component is mounted, the value of the ref will be the `section` element the ref is attached to.

If the component is unmounted, the ref's value goes back to the initial value of `null`.

A typical example to showcase a ref is to focus an input element on render, or by clicking a button.

Here's how to do that when you click a button:

```
import { useRef } from "react";

const Focus = () => {
  const inputRef = useRef(null);

  const handleFocus = () => {
    if (inputRef.current) {
      inputRef.current.focus();
    }
  };

  return (
    <div>
      <input ref={inputRef} type="text" placeholder="Enter text" />
      <button onClick={handleFocus}>Focus Input</button>
    </div>
  );
};

export default Focus;
```

In the code above, the `inputRef` is created and attached to the `input` element. There's also a button with an `onClick` event that calls a `handleFocus` function.

All the `handleFocus` function does is call the `focus()` method on the `input` element. Note that, because `input` is a built-in component that comes with React, the actual `input` DOM element is set to the `current` property of the ref. So you call the `focus()` method with `input.current.focus()`.

Here are some best practices you should be aware of while working with refs:

* Use refs mainly to interact with the DOM. You can also use them for mutable data, but state is a better choice for that.
* Don't use refs for basic state management – that is what `useState` is for.
* Make sure you check that `ref.current` exists before accessing its properties. Here's how to do that again:

```
const handleFocus = () => {
  if (inputRef.current) {
    inputRef.current.focus();
  }
};
```

This prevents errors in case the ref is accessed before it is attached to the DOM or after it is removed.

---

### Lecture 4.3: How Can You Create Custom Hooks In React

# How Can You Create Custom Hooks in React?

React provides many built-in hooks that let you implement different features in your projects. These include `useState`, `useEffect`, `useContext`, and others.

But sometimes, you'll need to add a feature that none of the built-in hooks can help with. Fortunately, you can create your own custom hooks in React.

Custom hooks are not as complicated as they might seem. They're just reusable functions that let you share logic across multiple components. That means reusability is another reason why you would want to build your own hook.

With a custom hook, you can extract logic away from any components that use them, like data fetching, state management, toggling, side effects like checking for the online or offline status of users, and so on.

You can then import the hook to use in any component, so you can focus on rendering and presentation within those components. That means fewer repetitions and less duplication, which means fewer places to make changes when you want to make any updates.

Now, let's take a look at how you can make your own custom hook.

In React, all built-in hooks start with the word `use`, so your custom hook should follow the same convention. Your custom hook's name should also clearly communicate what it does.

So, if your custom hook…

* fetches data, you can call it `useFetch`
* toggles something on and off, you can call it `useToggle`
* or if it implements debouncing, `useDebounce` is a good name

Let's say you want to build a custom hook to add debouncing to your app.

Debouncing is a programming technique that limits how often a function runs. It works by waiting until a user stops performing an action for a specified period of time before executing the function. For example, in a search box, instead of making an API call for every keystroke, debouncing waits until the user pauses typing for, say, 500 milliseconds.

To create a debouncing custom hook, you first need to create a `useDebounce.jsx` or `useDebounce.js` file. Conventionally, files for any custom hooks you create are saved to a `hooks` folder.

You can use some built-in hooks within your own custom hook. For debouncing, you need the `useState` and `useEffect` hooks, so import them at the top of your file:

```
import { useState, useEffect } from "react";
```

Next, create a `useDebounce` function that takes `value` and `delay` as parameters. `value` is the resource you want to wait for, and `delay` is the period of time you want to wait for. Since you want to wait for some period of time, the `setTimeout` and `clearTimeout` functions would be useful:

```
function useDebounce(value, delay) {
  const [debouncedValue, setDebouncedValue] = useState(value);

  useEffect(() => {
    const handler = setTimeout(() => {
      setDebouncedValue(value);
    }, delay);

    return () => {
      clearTimeout(handler);
    };
  }, [value, delay]);

  return debouncedValue;
}

export { useDebounce };
```

The `debouncedValue` state holds and returns the delayed value, which only updates after the specified timeout period.

`useEffect` is where the magic really happens. If you recall from the previous lesson, anything that exists outside the React rendering cycle, like setting and clearing a timer, is a side effect, and you should use the `useEffect` hook to handle them.

Within the `useEffect` hook here, you use `setTimeout` to set the `debouncedValue`. You then return a cleanup function that uses `clearTimeout` to clear the previous timeout whenever `value` or `delay` changes, or the component unmounts.

To use this hook, we've prepared a `footballers` array to filter through with a simple search bar:

```
const footballers = [
  'Lionel Messi', 'Cristiano Ronaldo', 'Neymar Jr',
  'Kylian Mbappe', 'Mohamed Salah', 'Sadio Mane',
  'Kevin De Bruyne', 'Robert Lewandowski', 'Harry Kane',
  'Sergio Ramos', 'Virgil van Dijk', 'Alisson Becker', 
  'Joshua Kimmich', 'Manuel Neuer', 'Karim Benzema', 
  'Thibaut Courtois', 'Eden Hazard', 'Raheem Sterling',
  'Bruno Fernandes', 'Trent Alexander-Arnold', 'Son Heung-min',
  'Pierre-Emerick Aubameyang','Sergio Aguero', 'Luis Suarez', 
  'Luka Modric', 'Casemiro', 'Frenkie de Jong', 'Gerard Pique',
  'Marc-Andre ter Stegen', 'Keylor Navas', 'Angel Di Maria', 
  "N'Golo Kante", 'Kai Havertz', 'Timo Werner', 'Hakim Ziyech', 
  'Christian Pulisic', 'Mason Mount', 'Olivier Giroud', 'Tammy Abraham', 
  'Kepa Arrizabalaga', 'Ben Chilwell', 'Thiago Silva', 'Kurt Zouma', 
  'John Terry', 'Didier Drogba', 'Frank Lampard', 'Ashley Cole', 'Petr Cech',
];

export default footballers;
```

And here's a `FootballerSearch` component that uses the `useDebounce` hook to delay searching for 1 second after the user stops typing:

```
import { useState, useEffect } from "react";
import { useDebounce } from "./hooks/useDebounce";
import footballers from "./footballers";

const FootballerSearch = () => {
  const [query, setQuery] = useState("");
  const debouncedQuery = useDebounce(query, 1000); // Start searching 1 second after the user stops typing

  useEffect(() => {
    if (debouncedQuery) {
      const results = footballers.filter((footballer) =>
        footballer.toLowerCase().includes(debouncedQuery.toLowerCase()),
      );
      console.log("Search results:", results);
    } else {
      console.log("Search results: []");
    }
  }, [debouncedQuery]);

  return (
    <>
      <h1 style={{ textAlign: "center" }}>Footballer Search App</h1>
      <div style={{ textAlign: "center" }}>
        <input
          style={{ padding: "0.5rem", width: "30%" }}
          type="text"
          value={query}
          onChange={(e) => setQuery(e.target.value)}
          placeholder="Search for a footballer..."
        />
      </div>
    </>
  );
};

export default FootballerSearch;
```

As you can see, the `debouncedQuery` variable is what initializes the `useDebounce` hook with the query state (what the user types), and the delay for 1,000 milliseconds, or 1 second. The search itself is handled inside the `useEffect` hook, and search results are logged to the console.

---

### Lecture 4.4: What Is Prop Drilling

# What Is Prop Drilling?

Prop drilling is the most basic approach to state management in React applications. It looks simple, but can get messy quickly, and is very hard to scale.

Let's look at what prop drilling is, why it's a problem, and a good replacement for it as an application grows.

Prop drilling is the process of passing props from a parent component to deeply nested child components, even when some of the child components don't need the props.

For example, say you have three components named `Parent`, `Child`, and `Grandchild`. If you want to use some data in the `Grandchild` component, but it's in the `Parent` component, you'd need to pass it from the `Parent` to the `Child` component, then from the `Child` to the `Grandchild` component.

Or if the data is even further up the chain, the data might have to be passed to the `Parent` component, too.

Here, the data I want to display is the string `Hello, Prop Drilling!`. It's assigned to the `greeting` variable in the root `App` component:

```
import "./App.css";
import Parent from "./Parent";

function App() {
  const greeting = "Hello, Prop Drilling!";

  return <Parent greeting={greeting} />;
}

export default App;
```

You can see the `Parent` component is also receiving the `greeting` variable as the value of a `greeting` prop. Here's the `Parent` component passing it into the `Child` component as the value of another `greeting` prop in the `Child`:

```
import Child from "./Child";

const Parent = ({ greeting }) => {
  return <Child greeting={greeting} />;
};

export default Parent;
```

And here's the `Child` component that passes it to the `Grandchild` component:

```
import Grandchild from "./Grandchild";

const Child = ({ greeting }) => {
  return <Grandchild greeting={greeting} />;
};

export default Child;
```

And finally the `Grandchild` component receives the greeting and uses it as the content of an `h1` element:

```
const Grandchild = ({ greeting }) => {
  return <h1>{greeting}</h1>;
};

export default Grandchild;
```

In the browser, you'll see a page with a single `h1` element that has the text `Hello, Prop Drilling!`.

At first, prop drilling might not seem like such a big deal. But as your app grows, it gets harder to understand, debug, and maintain.

If you need to pass props around, try to keep them all in a single parent component. This approach of centralizing all necessary data is called the "single source of truth".

For instance, say you want to add a new `response` to go with your `greeting`, and that you want to use both of them in the `Grandchild` component. Since `greeting` is already in the `App` component, it makes sense to put `response` there, too, and pass both of them down the chain:

```
function App() {
  const greeting = "Hello, Prop Drilling!";
  const response = "I'm not here to play!";

  return <Parent greeting={greeting} response={response} />;
}

const Parent = ({ greeting, response }) => {
  return <Child greeting={greeting} response={response} />;
};

const Child = ({ greeting, response }) => {
  return <Grandchild greeting={greeting} response={response} />;
};

const Grandchild = ({ greeting, response }) => {
  return (
    <>
      <h1>{greeting}</h1>
      <h2>{response}</h2>
    </>
  );
};

export default App;
```

In the browser, you'll see a page with an `h1` element that has the text `Hello, Prop Drilling!` and an `h2` element that has the text `I'm not here to play!`.

To avoid prop drilling, especially in large, complex applications, consider using the Context API or state management libraries like Redux and Redux Toolkit, Zustand, Recoil, and others.

You'll learn more about these in the coming lessons.

---

### Lecture 4.5: What Are State Management Libraries And When Should You Use Them

# What Are State Management Libraries, and When Should You Use Them?

As your app grows, managing how data flows between components can become complex.

When starting out, React's `useState` hook might be sufficient, but as you add features, you might encounter issues with:

* Passing props through components that don't need them, also known as prop drilling
* Keeping data in sync across different parts of your app
* Handling complex updates that affect multiple components simultaneously

These and other challenges may arise, which can lead to a codebase that's harder to maintain, debug, and test. That's where state management libraries come in – they provide a centralized place where components can get or update the data they need.

Let's take a look at a few different state management options you have, and when to use them.

The Context API is a state manager built into React that lets you share state across components without using a third-party library. It's a well-established upgrade over the `useState` hook, so it is perfect for cases like theme toggling or user authentication status.

However, the Context API does not handle frequent updates well, and can cause unnecessary re-renders, making it less suitable for complex state needs in applications like eCommerce and social media platforms.

Here's a counter component that demonstrates the basic usage of the Context API:

```
import { useState, createContext } from 'react';

const CounterContext = createContext();

const CounterProvider = ({ children }) => {
  const [count, setCount] = useState(0);

  return (
    <CounterContext.Provider value={{ count, setCount }}>
      {children}
    </CounterContext.Provider>
  );
};

export { CounterContext, CounterProvider };
```

This code creates a context and a provider to share a `count` state across the application.

`CounterProvider` uses the `useState` hook to initialize and manage the `count` state and its setter. Both are then passed into child components through the `Provider`.

So, when you wrap your whole app with the `CounterProvider`, the `count` state is available everywhere in your application.

Here's how you can wrap `CounterProvider` around your application:

```
import { CounterProvider } from './context/CounterContext';

function App() {
  return (
    <CounterProvider>
        {/* App components */}
    </CounterProvider>
  );
}

export default App;
```

And here's how you can use the `count` state:

```
import React, { useContext } from 'react';
import { CounterContext } from '../context/CounterContext';

const Counter = () => {
  const { count, setCount } = useContext(CounterContext);

  return (
    <>
      <div style={{ textAlign: 'center' }}>
        <h1>Context API Counter</h1>
        <button style={{ marginRight: '5px' }} onClick={() => setCount(count - 1)}>
          Decrease
        </button>
        <span>{count}</span>
        <button style={{ marginLeft: '5px' }} onClick={() => setCount(count + 1)}>
          Increase
        </button>
      </div>
    </>
  );
};

export default Counter;
```

As you can see, the `count` and its setter function, `setCount`, are initialized through the `useContext` function.

The current `count` state is then displayed, and `setCount` is used to increase and decrease the `count` state when the user clicks the decrement and increment buttons respectively.

Another popular state management library is Redux, which is one of the most popular state management libraries to use with React. It's been around for a long time, and is ideal for larger applications like eCommerce and social media platforms, forums, and so on.

Redux handles state management by providing a central store and strict control over state updates. It uses a predictable pattern with actions, reducers, and middleware.

Actions are payloads of information that send data from your application to the Redux store, often triggered by user interactions.

Reducers are functions that specify how the state should change in response to those actions, ensuring the state is updated in an immutable way.

Middleware, on the other hand, acts as a bridge between the action dispatching and the reducer, allowing you to extend Redux's functionality (for example, logging, handling async operations) without modifying the core flow.

The most common complaint about Redux is with all the boilerplate code you need to get started. In response, the Redux team introduced "Redux Toolkit" and "RTK Query", which simplify the setup process quite a bit.

You typically define both actions and reducers in a single file using the `createSlice()` function. It's common to name the file so it ends with the word `Slice`, for example, `productSlice`, `userSlice`, `counterSlice`, and so on.

Here's a `counterSlice` file to show you the basics:

```
import { createSlice } from '@reduxjs/toolkit';

const counterSlice = createSlice({
  name: 'counter',

  initialState: { count: 0 },

  reducers: {
    increment: (state) => {
      state.count += 1;
    },
    decrement: (state) => {
      state.count -= 1;
    },
  },
});

export const { increment, decrement } = counterSlice.actions;

export default counterSlice.reducer;
```

From here, you then need to wrap the entire app with the `Provider`, select a piece of state from the slice with `useSelector()`, then use `useDispatch()` to make the state active.

Another option to consider is Zustand.

Zustand is a lightweight state management library with a simple API. It is based on hooks, so there's less boilerplate compared to Redux, making it easier and quicker to set up.

Zustand is ideal for small to medium-scale applications. It works by using a `useStore` hook to access state directly in components and pages. This lets you modify and access data without needing actions, reducers, or a provider.

Here's a `useCounterStore` that implements another counter functionality:

```
import { create } from 'zustand';

const useCounterStore = create((set) => ({
  count: 0,
  increment: () => set((state) => ({ count: state.count + 1 })),
  decrement: () => set((state) => ({ count: state.count - 1 })),
}));

export default useCounterStore;
```

And here's how to initialize and use the states in your app:

```
// Import the useCounterStore (it's just a hook)
import useCounterStore from '../useCounterStore';

const Counter = () => {
  // Initialize the states with the useCounterStore hook
  const { count, increment, decrement } = useCounterStore();

  return (
    <>
      <div style={{ textAlign: 'center' }}>
        <h1>Zustand Counter</h1>
        <button style={{ marginRight: '5px' }} onClick={() => decrement()}>
          Decrease
        </button>
        <span>{count}</span>
        <button style={{ marginLeft: '5px' }} onClick={() => increment()}>
          Increase
        </button>
      </div>
    </>
  );
};

export default Counter;
```

Even though the front-end ecosystem is constantly evolving and new state management libraries regularly emerge, the ones we've discussed are widely used in the industry.

---

### Lecture 4.6: How Can You Debug Your React Components Using React Devtools

# How Can You Debug Your React Components Using the React DevTools?

The browser has built-in developer tools you can use to debug HTML, CSS, and JavaScript.

However, they're not great for finding and fixing bugs in React apps. So the React team developed a tool called "React Developer Tools" (AKA React DevTools) so you can inspect, debug, and profile React apps.

React DevTools is available as a browser extension for Chrome, Edge, and Firefox. If you're on Chrome or Edge, head over to the Chrome web store, search for "React Developer Tools”, and add it to your browser.

And if you use Firefox, head over to the Firefox Add-ons page, search for the tool, and add it to your browser.

If you use Safari, you can install React DevTools from npm by running `npm install -g react-devtools` or `yarn global add react-devtools`.

After installing and enabling React DevTools, if you open a React app in your browser, then open your browser's developer tools, you should see two extra tabs: Components and Profiler.

The Components tab displays each component for you in a tree view format. With it, you can:

* View the app's component hierarchy.
* Check and modify props, states, and context values in real time.
* Check the source code for each selected component.
* Log the component data to the console.
* Inspect the DOM elements for the component.

On the other hand, the Profiler tab helps you record and analyze component performance so you can identify unnecessary re-renders, view commit durations, and things you can optimize.

Here's a simple app to show you how you can inspect components and any props and state they have. This is similar to the code we used in a previous lesson on prop drilling:

```
import { useState } from "react";

export default function App() {
  const greeting = "Hello, Prop Drilling!";
  const response = "I'm not here to play!";

  return <Parent greeting={greeting} response={response} />;
}

const Parent = ({ greeting, response }) => {
  return <Child greeting={greeting} response={response} />;
};

const Child = ({ greeting, response }) => {
  return <Grandchild greeting={greeting} response={response} />;
};

const Grandchild = ({ greeting, response }) => {
  const [count, setCount] = useState(0);

  return (
    <>
      <h1>{greeting}</h1>
      <h2>{response}</h2>

      <button onClick={() => setCount(count + 1)}>Increase Count</button>
      <h2>Count: {count}</h2>
      <button onClick={() => setCount(count - 1)}>Decrease Count</button>
    </>
  );
};
```

If you look in the Components tab in React DevTools, you can see the tree view of the components. The `App` component is at the top, followed by the `Parent`, `Child`, and `Grandchild` components.

If you select any of these components, you can see the props and state in them. If you select the `Parent` component, you can see the `greeting` and `response` props, which are `Hello, Prop Drilling!` and `I'm not here to play!`, respectively.

You can see the props and update state in real-time, and change them if necessary. For instance, you can select the `Grandchild` component and change the `greeting` prop from `Hello, Prop Drilling!` to `Hello, Welcome to Prop Drilling!`, and see it reflected on the page immediately.

To log data in a component to the console, inspect the matching DOM elements and view the source code of the component. The icons in the top right corner let you do that. If you select the `Grandchild` component and click the `Log the component data to the console` button, it will log the props, state, hooks, nodes, and other data in the console.

A common bug you might encounter in React is called props mismatch.

For example, say that for the `Child` component, you mistakenly pass in `reply` as the prop instead of `response`:

```
const Child = ({ greeting, response }) => {
  return <Grandchild greeting={greeting} reply={response} />;
};
```

Remember that `Grandchild` expects a `response` prop. Because the component receives a different prop, it can't display that text on the page, and just adds and empty `h2` to the DOM. Instead, you'll just see the `h1` element with the text `Hello, Prop Drilling!`, along with the other buttons and text already on the page. The empty `h2` element is still there, but because it's empty, you can't see it without inspecting the DOM.

To fix this, you can inspect the prop progression from the `Parent` component down to the `Child` and edit the prop name directly. If you go to the Components tab, select the `Child` component, and change the `reply` prop to `response`, you'll see the `h2` element on the page with the text `I'm not here to play!`.

---

### Lecture 4.7: What Is Dependency Management And How Does It Work With Libraries Like React

# What Is Dependency Management, and How Does It Work with Libraries Like React?

In software, a dependency is where one component or module in an application relies on another to function properly. Dependencies are common in software applications because it allows developers to use pre-built functions or tools created by others.

If you want to build out a React application, you will need to install the React dependencies. Without these dependencies, none of your code will work correctly and the application will display a list of errors.

When you are working with more complex projects, you will often need to rely on many dependencies. If a set of dependencies is not well managed or defined in a project, then that will lead to what is known as dependency hell.

To manage software dependencies in a project, you will need to use a package manager. A package manager is a tool used for installation, updates, and removal of dependencies. Many popular programming languages like JavaScript, Python, Ruby and Java, all use package managers.

In an earlier lesson, you were briefly introduced to one popular package manager called npm.

To create a new React project using Vite and npm you can run the following command:

```
npm create vite@latest my-react-app -- --template react
```

As you recall from the prior lessons, this will create all of the necessary boilerplate code needed to launch a new React application. Before you can launch the application, you will need to install the dependencies by running `npm install` or `npm i` for short.

You can view all of the dependencies in the `package.json` file which is located in the root directory of your project.

The `package.json` file is a key configuration file in projects that contains metadata about your project, including its name, version, and dependencies. It also defines scripts, licensing information, and other settings that help manage the project and its dependencies.

When you install dependencies, a `node_modules` folder will be added to your project.

The `node_modules` folder is where all the packages and libraries required by your project are stored. This folder contains the actual code for the dependencies listed in the `package.json` file, including both your project's direct dependencies and any dependencies of those dependencies.

The two core dependencies needed for a React project will be the `react` and `react-dom` packages:

```
"dependencies": {
  "react": "^18.3.1",
  "react-dom": "^18.3.1"
}
```

The `package.json` will list the current versions you are using for those packages. If you need to update any packages locally, you can run the `npm update` command. Or you can update all packages globally by running the `npm update -g` command.

In addition to the `package.json` file, you will also have a `package-lock.json` file. This file will lock down the exact versions of all packages that your project is using. When you update a package, then the new versions will be updated in the lock file as well.

Another important aspect of the `package.json` file are the dev dependencies:

```
"devDependencies": {
  "@eslint/js": "^9.17.0",
  "@types/react": "^18.3.18",
  "@types/react-dom": "^18.3.5",
  "@vitejs/plugin-react": "^4.3.4",
  "eslint": "^9.17.0",
  "eslint-plugin-react": "^7.37.2",
  "eslint-plugin-react-hooks": "^5.0.0",
  "eslint-plugin-react-refresh": "^0.4.16",
  "globals": "^15.14.0",
  "vite": "^6.0.5"
}
```

Dev dependencies are packages that are only used for development and not in production. An example of this would be a testing library like Jest. You would install Jest as a dev dependency because you only use it to test your project locally, and isn't needed for the application to run in production.

For the majority of this lesson, we have been focusing on npm. But there are other package managers like yarn and pnpm. So which package manager should you use for your project?

Well, the short answer is it depends.

If you are joining an existing project with a team, then all of those decisions will be made for you and you will use the existing package manager. If you are building out a project from scratch, then you will need to research the pros and cons of each manager and decide which one will better suit your needs.

---

### Lecture 4.8: How Does Routing Work In React

# How Does Routing Work in React?

In earlier lessons, you learned that React is a single page application. Single page applications are applications that contain one HTML file and use JavaScript to dynamically update any content on the page.

So what happens when you need to add multiple "pages" to your React application? How would you go about navigating to those different views?

Well, that is where React Router comes in.

React Router is a third party library that allows you to add routing to your React applications. To begin, you will need to install React Router in an existing React project like this:

```
npm i react-router
```

If you check the `package.json` file, you will see that `react-router` was added to the list of dependencies:

```
"dependencies": {
  "react": "^18.3.1",
  "react-dom": "^18.3.1",
  "react-router": "^7.2.0"
}
```

Then inside of your `main.jsx` or `index.jsx` file, you will need to import `BrowserRouter` and render `BrowserRouter` around your `App` component:

```
import { StrictMode } from "react";
import { createRoot } from "react-dom/client";
import { BrowserRouter } from "react-router";
import App from "./App.jsx";

import "./index.css";

createRoot(document.getElementById("root")).render(
  <StrictMode>
    <BrowserRouter>
      <App />
    </BrowserRouter>
  </StrictMode>
);
```

To enable routes in your application, you will need to update your `import` statement to include the `Routes` and `Route` components like this:

```
import { BrowserRouter, Routes, Route } from "react-router";
```

Then inside of the `BrowserRouter`, add the `Routes` and `Route` components:

```
createRoot(document.getElementById("root")).render(
  <StrictMode>
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<App />} />
      </Routes>
    </BrowserRouter>
  </StrictMode>
);
```

The `path` and `element` are used to couple the URL and UI components together. In this case, we are setting up a route for the homepage that points to the `App` component.

It is common in larger applications to have multiple views and routes setup like this:

```
<Routes>
  <Route index element={<Home />} />
  <Route path="about" element={<About />} />

  <Route path="products">
    <Route index element={<ProductsHome />} />
    <Route path=":category" element={<Category />} />
    <Route path=":category/:productId" element={<ProductDetail />} />
    <Route path="trending" element={<Trending />} />
  </Route>
</Routes>
```

The `index` prop in these examples is meant to represent the default route for a given path segment. So the `Home` component will be shown at the root path (`/`) while the `ProductsHome` component will be shown at the `products` path.

You may have also noticed that we are nesting a few routes inside another route like this:

```
<Route path="products">
  <Route path="trending" element={<Trending />} />
</Route>
```

This means that the path of the child route will be appended to the parent route's path. So in this example, the `path` for the trending products will be `products/trending`.

If the `path` begins with a colon (`:`) then that represents a dynamic segment in the route:

```
<Route path=":category" element={<Category />} />
```

In this example we have a dynamic segment called `category`. When a user navigates to a URL like `products/brass-instruments`, then the view will change to the `Category` component and you can dynamically fetch the appropriate data based on the segment.

You can access the value of the dynamic segment by using the `useParams` hook inside the child component like this:

```
import { useParams } from "react-router";

export default function Category() {
  let params = useParams();
   {/* Accessing the category param: params.category */}
   {/* rest of code goes here */}
}
```

Dynamic routes are helpful because they allow you to create flexible and reusable components that can render different content based on the parameters in the URL. Instead of defining a fixed list of paths for every possible route, you can use dynamic segments to render various content based on what the user has requested.

---

### Lecture 4.9: What Are React Frameworks And Why Are They Commonly Used In The Industry

# What Are React Frameworks, and Why Are They Commonly Used in the Industry?

Up until this point, you have been using React to build out user interfaces. If you needed additional features like routing, then you had to import a third party library like React Router to be able to switch between the different views.

But what happens when you need to build out a full-stack web application? Well you could use React for the front-end and use Node and Express for the back-end logic if you just want to stick with JavaScript. Or you could use other languages like Go, Python, or Java for your back-end.

While all of these are viable options, there are times where you might want to use a React framework instead. React frameworks provide features like routing, image optimizations, data fetching, authentication and more. This means that you might not need to set up separate front-end and back-end applications for certain use cases.

Let's take a closer look at Next.js which is a popular React framework. One of the main features for Next.js is the file-system based router. This routing system includes support for dynamic routes, parallel routes, route handlers, redirects, internalization and more.

Here is an example of creating a custom request handler:

```
export async function GET() {
  const res = await fetch("https://example-api.com");
  const data = await res.json();

  return Response.json({ data });
}
```

You can define route handlers like GET or POST requests in a file called `route.js` inside the `app/api` directory.

Another feature of Next.js are the automatic image and font optimizations.

Here is an example of working with the `Image` component inside a `page.js` file:

```
import Image from "next/image";

export default function Page() {
  return (
    <Image src="link-to-image-goes-here" alt="descriptive-title-goes-here" />
  );
}
```

The `Image` component extends the native HTML `img` element and allows for faster page loads and size optimizations. This means that images will only load when they enter the viewport and the `Image` component will automatically serve correctly sized images for each device.

While those are just a few features of Next.js, there are many more features that you can use to build robust full-stack web applications. There are also other React frameworks like Remix that will provide the same ability to build out modern full-stack web applications.

Even though the JavaScript library and framework landscape is constantly changing, it is important to be aware of the available options to you and learn about each framework's pros and cons.

---

### Lecture 4.10: How Does Data Fetching Work In React

# How Does Data Fetching Work in React?

React apps often rely on external APIs and databases for dynamic content. To access the data from those APIs and databases, you need to use some data fetching techniques.

Let's take a look at how data fetching works in React and the different options available to you for fetching data.

React is not opinionated about how you fetch your data, this means on a basic level, you can use the built-in Fetch API, which all modern browsers support.

You can also use Axios and SWR. Axios is promise-based HTTP request library built on top of the XMLHttpRequest object, and SWR is a React hook for data fetching created by the Vercel team.

Let's start with an example. You first need to import the `useState` and `useEffect` hooks:

```
import { useState, useEffect } from "react";
```

Then you will need to create three state variables called `loading`, `data`, and `error`:

```
const [data, setData] = useState(null);
const [loading, setLoading] = useState(true);
const [error, setError] = useState(null);
```

The `loading` variable will track whether the data is still being fetched. The `data` variable represents the data itself, and the `error` variable will capture any errors that might occur during the data fetching process.

Since data fetching is a side effect, it's best to use the Fetch API inside of a `useEffect` hook.

Here's an example of that:

```
useEffect(() => {
  fetch("https://jsonplaceholder.typicode.com/posts")
    .then((res) => res.json())
    .then((data) => {
      setData(data);
      setLoading(false);
    })
    .catch((err) => {
      setError(err);
      setLoading(false);
    });
}, []);
```

This `useEffect` fetches the data with the Fetch API and sets all the states.

You can make things better by using `async`/`await` instead of the `.then()` syntax. That means you have to have a separate function inside the `useEffect` because you cannot prefix `useEffect` with the `async` keyword:

```
useEffect(() => {
  const fetchData = async () => {
    try {
      const res = await fetch("https://jsonplaceholder.typicode.com/posts");
       
      if (!res.ok) {
        throw new Error("Network response was not ok");
      }

      const data = await res.json();
      setData(data);
    } catch (err) {
      setError(err);
    } finally {
      setLoading(false);
    }
  };

  fetchData();
}, []);
```

You can then go ahead and use all of those states to render the data from the API.

Here's the full code:

```
import { useState, useEffect } from "react";

const FetchPosts = () => {
  const [data, setData] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchData = async () => {
      try {
        const res = await fetch("https://jsonplaceholder.typicode.com/posts");
       
        if (!res.ok) {
          throw new Error("Network response was not ok");
        }

        const data = await res.json();
        setData(data);
      } catch (err) {
        setError(err);
      } finally {
        setLoading(false);
      }
    };

    fetchData();
  }, []);

  if (loading) {
    return <p>Loading...</p>;
  }

  if (error) {
    return <p>{error.message}</p>;
  }

  return (
    <ul>
      {data.map((post) => (
        <li key={post.id}>{post.title}</li>
      ))}
    </ul>
  );
};

export default FetchPosts;
```

In the UI, you would see `Loading...` on the screen when the data is being fetched, and then the data or error would show depending on if the data fetch was successful.

Remember we talked about data fetching with Axios and SWR too. Let's take a look at an example using Axios.

You will first need to install Axios from the command line like this:

```
npm i axios
```

Then you will need to import Axios like this:

```
import axios from "axios";
```

Then you can use the same state variables from earlier and fetch data from the API using `axios.get`:

```
const [data, setData] = useState(null);
const [loading, setLoading] = useState(true);
const [error, setError] = useState(null);

useEffect(() => {
  const fetchData = async () => {
    try {
      const res = await axios.get(
        "https://jsonplaceholder.typicode.com/users"
      );
      setData(res.data);
    } catch (err) {
      setError(err);
    } finally {
      setLoading(false);
    }
  };

  fetchData();
}, []);
```

You might have noticed that there is no `await res.json()` line in this example. That's because Axios automatically parses JSON, so there's no need for that.

The last example we will look at is to use the `useSWR` hook to fetch data.

Just like with Axios, you will need to install SWR like this:

```
npm install swr
```

Then you will need to import the `useSWR` hook into the file like this:

```
import useSWR from "swr";
```

In comparison to the previous examples, the SWR syntax is way shorter. What you need to do is to create a fetcher function and pass it into the `useSWR` hook as its second parameter (the endpoint is the first parameter).

You also get to destructure both the data and error states from the `useSWR` hook, so you don't need the `useState` hook.

Here is the syntax:

```
const fetcher = (url) => fetch(url).then((res) => res.json());
const { data, error } = useSWR(endpoint, fetcher);
```

Note that the "fetcher" name here is only a convention, so you're free to name the variable whatever you want.

Here's a component fetching todos from the JSON Placeholder API:

```
import useSWR from "swr";

const fetcher = (url) => fetch(url).then((res) => res.json());

const FetchTodos = () => {
  const { data, error } = useSWR(
    "https://jsonplaceholder.typicode.com/todos",
    fetcher
  );

  if (!data) {
    return <h2>Loading...</h2>;
  }
  if (error) {
    return <h2>Error: {error.message}</h2>;
  }

  return (
    <>
      <h2>Todos</h2>
      <div>
        {data.map((todo) => (
          <h3 key={todo.id}>{todo.title}</h3>
        ))}
      </div>
    </>
  );
};

export default FetchTodos;
```

As you learned in a previous lesson on custom hooks, data fetching is a logic you can extract into a custom hook. So, if you're fetching data in multiple components and pages, it is best to create a `useFetch` hook.

Here's a `useFetch` hook that uses SWR for data fetching:

```
import useSWR from "swr";

const fetcher = (url) => fetch(url).then((res) => res.json());

const useFetch = (url) => {
  const { data, error } = useSWR(url, fetcher);

  return {
    data,
    loading: !data && !error,
    error,
  };
};

export default useFetch;
```

And here's how to use the `useFetch` hook to rewrite the first example that fetches posts from the JSON Placeholder API:

```
import useFetch from "./useFetch";

const FetchPosts = () => {
  const { data, loading, error } = useFetch(
    "https://jsonplaceholder.typicode.com/posts"
  );

  if (loading) {
    return <h2>Loading...</h2>;
  }

  if (error) {
    return <h2>{error.message}</h2>;
  }

  return (
    <>
      <h2>Posts</h2>
      <ul>
        {data.map((post) => (
          <li key={post.id}>{post.title}</li>
        ))}
      </ul>
    </>
  );
};

export default FetchPosts;
```

---

### Lecture 4.11: What Is Memoization And How Does The Usememo Hook Work

# What Is Memoization, and How Does the useMemo Hook Work?

As your React app gets larger, unnecessary re-renders and expensive calculations can slow down performance, leading to slow UI updates and increased resource usage.

This can be especially problematic in apps with complex state management, large lists, functions that require heavy computations, and many components with a single parent.

This gives rise to the need to optimize your React app for better performance by minimizing redundant computations and ensuring smoother interactions.

React solves this problem with a process called memoization, a technique which caches values and functions to prevent unnecessary recalculations, so your app can be faster and more responsive.

By definition, memoization is an optimization technique in which the result of expensive function calls are cached (remembered) based on specific arguments. When the same arguments are provided again, the cached result is returned instead of re-computing the function.

The memoization process happens this way:

* Store the results of function calls along with their input arguments.
* Before executing the function, check if the result for the current arguments already exists in the cache.
* If it exists, return the cached result instead of running the computation again.
* If it doesn't exist, compute the result, store it in the cache, and then return it.

To improve developer experience with memoization, React provides three tools – `React.memo` (or `memo`), `useMemo` and `useCallback`.

As you might guess, both `useMemo` and `useCallback` are hooks, but `React.memo` is a component wrapper, a higher-order component (HOC).

In the next lesson, we will take a look at how the `useCallback` hook and `React.memo` work.

`useMemo` lets you memoize computed values while `useCallback` does the same for function references.

If you're wondering what computed values and function references are, computed values refer to the result of executing a function, while function references are the pointers to functions – the function object in memory.

Let's see how to use the `useMemo` hook first. Here's the basic syntax of the `useMemo` hook:

```
const memoizedValue = useMemo(
  function () {
    return computeExpensiveValue(a, b);
  },
  [a, b]
);
```

You can see all that's needed is to wrap the `useMemo` hook around the function.

This `ExpensiveSquare` component will receive a `num` prop which it will use to calculate the square:

```
function ExpensiveSquare({ num }) {
  function calculateSquare(n) {
    console.log("Calculating square...");
    return n * n;
  }

  const squared = calculateSquare(num);
  return (
    <p>
      Square of {num}: {squared}
    </p>
  );
}
export default ExpensiveSquare;
```

Here's the `App` component where the `ExpensiveSquare` is being used:

```
import { useState, useEffect } from "react";
import ExpensiveSquare from "./components/ExpensiveSquare";

function App() {
 const [timer, setTimer] = useState(0);
 const [num, setNum] = useState(0);

 useEffect(() => {
   const interval = setInterval(() => setTimer((c) => c + 1), 1000);
   return () => clearInterval(interval);
 }, []);

 return (
   <div>
     <h1>Timer: {timer} seconds gone</h1>
     <ExpensiveSquare num={num} />
     <button onClick={() => setNum((n) => n + 1)}>Increase Number</button>
   </div>
 );
}

export default App;
```

The `timer` in the `useEffect`, running every second, will make the `calculateSquare` function run any time it runs, even when you don't increase the `num` state variable.

To solve this problem, we can use the `useMemo` hook by wrapping the function call in it and specifying the `num` variable as the dependency:

```
// import the useMemo hook
import { useMemo } from "react";

function ExpensiveSquare({ num }) {
  function calculateSquare(n) {
    console.log("Calculating square...");
    return n * n;
  }

  // const squared = calculateSquare(num);
  // Wrap the function call in useMemo instead
  const squared = useMemo(() => calculateSquare(num), [num]);

  return (
    <p>
      Square of {num}: {squared}
    </p>
  );
}

export default ExpensiveSquare;
```

This will make sure the function is memoized by caching the result. Even though the `ExpensiveSquare` component still re-renders every time the parent's `timer` state updates, the `calculateSquare` computation only re-runs on the initial render and when `num` changes.

---

### Lecture 4.12: How Do The Usecallback Hook And React Memo Work

# How Do the useCallback Hook and React.memo Work?

In the last lesson, you learned about memoization and how the `useMemo` hook works.

In this lesson, you'll learn how the `useCallback` hook and `React.memo` work.

In the last lesson, we also mentioned that `useCallback` is for memoizing function references.

For `React.memo`, it lets you memoize a component to prevent it from unnecessary re-renders when its prop has not changed.

Here's the basic syntax of the `useCallback` hook:

```
const handleClick = useCallback(() => {
  // code goes here
}, [dependency]);
```

And here's the basic syntax of `React.memo`:

```
const MemoizedComponent = React.memo(({ prop }) => {
  return (
    <>
      {/* Presentation */}
    </>
  )
});
```

Let's look at an example of the `useCallback` hook:

```
import { useState, useEffect } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  const handleClick = () => {
    setCount((prevCount) => prevCount + 1);
  };

  useEffect(() => {
    console.log("useEffect runs");
  }, [handleClick]);

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={handleClick}>Increment</button>
    </div>
  );
}

export default Counter;
```

In the component, the effect runs any time `handleClick` changes because the `handleClick` function is being recreated on every render.

To fix this, you need to tell React to treat the `handleClick` function as the same thing across renders by memoizing it with the `useCallback` hook, so it doesn't get recreated:

```
import { useState, useEffect, useCallback } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  // Memoize the handleClick function with useCallback
  const handleClick = useCallback(() => {
    setCount((prevCount) => prevCount + 1);
  }, []);

  useEffect(() => {
    console.log("useEffect runs");
  }, [handleClick]);

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={handleClick}>Increment</button>
    </div>
  );
}

export default Counter;
```

Now the `handleClick` function is not being recreated on every render.

To show you how the `React.memo` (or `memo`) higher-order function works and the `useCallback` hook work in tandem, here's a `Counter` component with a `handleClick` function that needs `useCallback` but is currently not using it:

```
import { useState, useEffect, useCallback } from "react";
import CounterChild from "./CounterChild";

function Counter() {
  const [count, setCount] = useState(0);
  const [timer, setTimer] = useState(new Date().toLocaleTimeString());

  const handleClick = () => {
    setCount(count + 1);
  };

  useEffect(() => {
    const interval = setInterval(() => {
      setTimer(new Date().toLocaleTimeString());
    }, 1000);

    return () => clearInterval(interval);
  }, []);

  return (
    <div>
      <h1>Time: {timer}</h1>
      <p>Count: {count}</p>
      <button onClick={handleClick}>Increment</button>
      <CounterChild onClick={handleClick} />
    </div>
  );
}

export default Counter;
```

This function also has a timer in state that updates every second. This makes the component re-render every time the `timer` changes, making the `handleClick` function get recreated on every render.

That's why the `handleClick` needs to be memoized with `useCallback`.

Here's the `CounterChild` component:

```
const CounterChild = ({ onClick }) => {
  console.log("CounterChild component rendered");
  return <button onClick={onClick}>Increment from Child</button>;
};

export default CounterChild;
```

This `CounterChild` component takes an `onClick` prop, giving you the ability to also increment the counter from it.

Since the `CounterChild` component is a child of the `Counter` component, it will also render any time the `Counter` re-renders due to the changing timer. So, the `CounterChild` also needs to be memoized.

Without memoization, because as the component re-renders due to the timer updating every second, the `CounterChild` component is also re-rendered.

To prevent this, you need to memoize the `CounterChild` component with `React.memo`:

```
import React from "react";

const CounterChild = React.memo(({ onClick }) => {
  console.log("CounterChild component rendered");
  return <button onClick={onClick}>Increment from Child</button>;
});

export default CounterChild;
```

Things do not work optimally yet even after memoizing the `CounterChild` with `React.memo`.

This happens because the `handleClick` function is being recreated on every render, so it also needs to be memoized with `useCallback`, in order to tell React that you need the function to stay the same across renders:

```
const handleClick = useCallback(() => {
  setCount((prevCount) => prevCount + 1);
}, [count]);
```

Now, the component only re-renders when the `count` state changes.

---

### Lecture 4.13: What Is The Useoptimistic Hook And How Does It Work

# What Is the useOptimistic Hook, and How Does It Work?

Recent versions of React introduced server components and server actions to shift some of the rendering and logic responsibilities to the server.

Along with those updates, React added a new hook called `useOptimistic` to keep UIs responsive while waiting for an async action to complete in the background.

While this is often used for fetching data from a server, it's not limited to that. The hook is generally useful for handling async operations, ensuring the UI remains smooth and interactive while the action runs.

Let's take a look at what the `useOptimistic` hook is and how it contributes to making snappy and responsive UIs.

The `useOptimistic` hook helps manage "optimistic updates" in the UI, a strategy in which you provide immediate updates to the UI based on the expected outcome of an action, like waiting for a server response.

Here's the basic syntax of the `useOptimistic` hook:

```
const [optimisticState, addOptimistic] = useOptimistic(actualState, updateFunction);
```

* `optimisticState` is the temporary state that updates right away for a better user experience.
* `addOptimistic` is the function that applies the optimistic update before the actual state changes.
* `actualState` is the real state value that comes from the result of an action, like fetching data from a server.
* `updateFunction` is the function that determines how the optimistic state should update when called.

At first glance, it might seem like the `useOptimistic` hook is just another way to handle loading states in React. But it's more than that.

A loading state controls whether you see a spinner, message, or some other indicator in the UI while something happens in the background.

However, the `useOptimistic` hook updates the UI instantaneously based on an expected outcome, even before you, say, make a call to an API. This hook gives you a chance to show a loading indicator or message, handle potential errors gracefully, and show instant feedback to make the UI feel snappy.

This will become clearer as we go through some examples showing how the `useOptimistic` hook works.

Here's an action that simulates saving a task to a server. It returns the task after a 1 second delay, as it could happen with a real-world API request:

```
export async function saveTask(task) {
  await new Promise((res) => setTimeout(res, 1000));

  return task;
}
```

Here's the code that sets up the `useOptimistic` hook by importing and initializing it, with an `handleSubmit` function that sends an input to the action:

```
"use client";

import { useOptimistic } from "react";

export default function TaskList({ tasks, addTask }) {
  const [optimisticTasks, addOptimisticTask] = useOptimistic(
    tasks,
    (state, newTask) => [...state, { text: newTask, pending: true }]
  );

  async function handleSubmit(e) {
    e.preventDefault();
    const formData = new FormData(e.target);

    addOptimisticTask(formData.get("task"));

    addTask(formData);
    e.target.reset();
  }

  return <>{/* UI */}</>;
}
```

In the code, the `useOptimistic` hook keeps a temporary list of tasks that updates immediately when you add a new task.

The line, `(state, newTask) => [...state, { text: newTask, pending: true }]` ensures that a new task appears with a pending status even before the server confirms something is coming from the form.

When the form is submitted, the `handleSubmit` function extracts the task and adds it "optimistically" with the `addOptimisticTask` parameter. Then `addTask` is passed as a prop which sends the task to the server. Finally, the form is reset by calling `e.target.reset()`.

Here's the `TaskList` component:

```
"use client";
import { useOptimistic, startTransition } from "react";

export default function TaskList({ tasks, addTask }) {
  const [optimisticTasks, addOptimisticTask] = useOptimistic(
    tasks,
    (state, newTask) => [...state, { text: newTask, pending: true }]
  );

  async function handleSubmit(e) {
    e.preventDefault();
    const formData = new FormData(e.target);

    startTransition(() => {
      addOptimisticTask(formData.get("task"));
    });

    addTask(formData);
    e.target.reset();
  }

  return (
    <div className="max-w-md mx-auto p-4">
      <h3 className="text-xl font-medium mb-3">Tasks</h3>

      <ul className="space-y-2 mb-4">
        {optimisticTasks.map((task, index) => (
          <li key={index} className="p-2 border-b">
            {task.text}
            {task.pending && (
              <small className="ml-2 text-gray-500 text-sm">
                Adding Task...
              </small>
            )}
          </li>
        ))}
      </ul>

      <form onSubmit={handleSubmit} className="flex gap-2">
        <input
          type="text"
          name="task"
          placeholder="Type in a task..."
          className="flex-1 p-2 border"
        />
        <button type="submit" className="bg-gray-200 px-3 py-2 cursor-pointer">
          Submit
        </button>
      </form>
    </div>
  );
}
```

Here, we are looping through the `optimisticTask` parameter to display the task. When `task.pending` is `true`, the text `Adding Task...` is displayed next to the task, confirming that the task has been added optimistically before the server confirms it.

Here's the `Task` component that manages the state for the form. It calls the `saveTask` function from the action so it can add the task, and appends the new task once it is received by the server:

```
"use client";

import { useState } from "react";
import TaskList from "./TaskList";
import { saveTask } from "./actions";

export default function Tasks() {
  const [tasks, setTasks] = useState([]);

  async function addTask(formData) {
    const newTaskText = formData.get("task");

    const savedTask = await saveTask(newTaskText);
    setTasks((prev) => [...prev, { text: savedTask, pending: false }]);
  }

  return <TaskList tasks={tasks} addTask={addTask} />;
}
```

This ensures snappy UI updates by showing instant feedback instead of waiting for a response. Once the task is saved, the `pending` property is removed, and the final task list updates accordingly.

In the UI, there are two things happening that are not supposed to happen. First, you can't see the `Adding Task...` text since it appears and disappears too quickly. Next, there's an error occurring after adding the task.

There are two things we need to do to address those issues.

First, we need to import `startTransition` from React and use it to wrap the line `addOptimisticTask(formData.get('task'))`:

```
startTransition(() => {
  addOptimisticTask(formData.get("task"));
});
```

Second, we need to make the `Adding Task...` text visible for some time before it goes away.

To do this, we can modify the `addTask` function with a pending state and simulate a delay of a few seconds before marking the task as completed. `setTimeout()` is ideal for this:

```
async function addTask(formData) {
  const newTaskText = formData.get("task");

  // Add an optimistic task with a pending state
  const tempTask = { id: Date.now(), text: newTaskText, pending: true };
  setTasks((prev) => [...prev, tempTask]);

  // Simulate a 3 seconds delay before marking the task as completed
  setTimeout(async () => {
    const savedTask = await saveTask(newTaskText);

    setTasks((prev) =>
      prev.map((task) =>
        task.id === tempTask.id
          ? { ...task, text: savedTask, pending: false }
          : task
      )
    );
  }, 3000);
}
```

And once you do that, everything works fine.

---

### Lecture 4.14: What Are React Server Components And How Do They Work

# What Are React Server Components, and How Do They Work?

React Server Components (RSCs) is a new trend that has changed the way React developers approach things. With RSCs, more work shifts to the server, which has a lot of benefits.

Let's take a look at what server components are, how they work, and what led to the introduction of server components.

React Server Components are React components that render exclusively on the server, which sends only the final HTML to the client. This means those components can directly access server-side resources and dramatically reduce the amount of JavaScript sent to the browser.

React apps have traditionally used a "client component" system that handles everything in a typical React app, such as rendering, interactivity, and side effects. The term "client component" was rarely used until the introduction of React server components recently.

But the client component system comes with some drawbacks like large JavaScript bundles and slower initial load times.

React frameworks like Next.js and Gatsby found workarounds to offload some processes to the server in order to fix those problems, but none of them were standardized. If you've used either framework, you've probably heard about `getServerSideProps` and `getServerData`.

Then came React Server Components, which let you run some components entirely on the server so you can do things like data fetching and computation before any code runs in the user's browser.

Server components were first popularized and are readily available in Next.js. Other frameworks like Remix and Gatsby are catching up, and there's an experimental plugin for Vite called `vite-plugin-react-server` which lets you build server components.

So how do server components work?

One of the best ways to demonstrate React Server Components is with data fetching.

In traditional React client components, you let the browser handle API requests. Since data fetching is a side effect, you make that API call in a `useEffect` hook.

It's also good practice to set state variables like loading, data, and error so you can indicate that the data is loading, display the data when it's ready, or display an error in your app.

With React Server Components, you can move the entire component to the server and fetch data there without having to use `useState` or `useEffect`:

```
const Users = async () => {
  const res = await fetch("https://jsonplaceholder.typicode.com/users");
  const users = await res.json();

  return (
    <>
      <h1 className="text-4xl text-center mt-6">Users</h1>
      <ul className="text-center mt-3">
        {users.map((user) => (
          <li key={user.id}>{user.name}</li>
        ))}
      </ul>
    </>
  );
};

export default Users;
```

Because React Server Components only run on the server, you can just fetch data from an API and render just once. Also, since data fetching happens on the server, closer to the source, your app may perform better, especially for people with slow network connections.

One major gotcha is that all the code for server components remains on the server, and doesn't get shipped to the browser. That means you can't use React hooks with them, and they don't have access to Web APIs or browser event listeners. So how can you add interactivity?

In the Next.js app router, all components are server components by default. If you want to add interactivity, you need to mark the component as a client component with the `"use client"` directive.

Let's say you want to make the previous example a client component. Here's how you can do that:

```
"use client";

import { useState, useEffect } from "react";

const Users2 = () => {
  const [status, setStatus] = useState({
    users: [],
    loading: true,
    error: null,
  });

  async function fetchUsers() {
    try {
      const res = await fetch("https://jsonplaceholder.typicode.com/users");
      const data = await res.json();
      setStatus((prevStatus) => ({
        ...prevStatus,
        users: data,
        loading: false,
      }));
    } catch (err) {
      setStatus((prevStatus) => ({
        ...prevStatus,
        error: err.message,
        loading: false,
      }));
    }
  }

  useEffect(() => {
    fetchUsers();
  }, []);

  if (status.loading) {
    return <p>Loading Users...</p>;
  }
  if (status.error) {
    return <p>Error getting users: {status.error}</p>;
  }

  return (
    <>
      <h1 className="text-4xl text-center mt-6">Users</h1>
      <ul className="text-center mt-3">
        {status.users.map((user) => (
          <li key={user.id}>{user.name}</li>
        ))}
      </ul>
    </>
  );
};

export default Users2;
```

If you want to add interactivity like click events, the component also has to be marked as a client component:

```
"use client";

import { useState } from "react";

const Counter = () => {
  const [count, setCount] = useState(0);

  return (
    <>
      <h1>Counter</h1>
      <button onClick={() => setCount(count + 1)}>Increment</button>
      <h2>{count}</h2>
      <button onClick={() => setCount(count - 1)}>Decrement</button>
    </>
  );
};

export default Counter;
```

If you don't add the use client directive to the component, you get an error with a message that says "You're importing a server component that needs `useState`. This React hook only works in a client component. To fix, mark the file (or its parent) with the `"use client"` directive."

The main benefits that come with React Server Components are that data fetching becomes simpler, the code is easier to read, and client complexity is reduced.

---

### React Forms Data Fetching And Routing

# React Forms, Data Fetching and Routing Review

Working with Forms in React
---------------------------

* **Controlled Inputs**: This is when you store the input field value in state and update it through `onChange` events. This gives you complete control over the form data and allows instant validation and conditional rendering.

```
import { useState } from "react";

function App() {
  const [name, setName] = useState("");

  const handleChange = (e) => {
    setName(e.target.value);
  };

  const handleSubmit = (e) => {
    e.preventDefault();
    console.log(name);
  };

  return (
    <>
      <form onSubmit={handleSubmit}>
        <label htmlFor="name">Your name</label> <br />
        <input value={name} id="name" onChange={handleChange} type="text" />
        <button type="submit">Submit</button>
      </form>
    </>
  );
}

export default App;
```

* **Uncontrolled Inputs**: Instead of handling the inputs through the `useState` hook, uncontrolled inputs in HTML maintain their own internal state with the help of the DOM. Since the DOM controls the input values, you need to pull in the values of the input fields with a `ref`.

```
import { useRef } from "react";

function App() {
 const nameRef = useRef();

 const handleSubmit = (e) => {
   e.preventDefault();
   console.log(nameRef.current.value);
 };

 return (
   <form onSubmit={handleSubmit}>
     <label htmlFor="name">Your</label>{" "}
     <input type="text" ref={nameRef} id="name" />
     <button type="submit">Submit</button>
   </form>
 );
}

export default App;
```

Working with the `useActionState` Hook
--------------------------------------

* **Server Actions**: These are functions that run on the server to allow form handling right on the server without the need for API endpoints. Here is an example from a Next.js application:

```
"use server";

async function submitForm(formData) {
 const name = formData.get("name");
 return { message: `Hello, ${name}!` };
}
```

The `"user server"` directive marks the function as a server action.

* **`useActionState` Hook**: This hook updates state based on the outcome of a form submission. Here's the basic syntax of the `useActionState` hook:

```
const [state, action, isPending] = useActionState(actionFunction, initialState, permalink);
```

* `state` is the current state the action returns.
* `action` is the function that triggers the server action.
* `isPending` is a boolean that indicates whether the action is currently running or not.
* `actionFunction` parameter is the server action itself.
* `initialState` is the parameter that represents the starting point for the state before the action runs.
* `permalink` is an optional string that contains the unique page URL the form modifies.

Data Fetching in React
----------------------

* **Options For Fetching Data**: There are many different ways to fetch data in React. You can use the native Fetch API, or third party tools like Axios or SWR.
* **Commonly Used State Variables When Fetching Data**: Regardless of which way you choose to fetch your data in React, there are some pieces of state you will need to keep track of. The first is the data itself. The second will track whether the data is still being fetched. The third is a state variable that will capture any errors that might occur during the data fetching process.

```
const [data, setData] = useState(null);
const [loading, setLoading] = useState(true);
const [error, setError] = useState(null);
```

Since data fetching is a side effect, it's best to use the `Fetch API` inside of a `useEffect` hook.

```
useEffect(() => {
  const fetchData = async () => {
    try {
      const res = await fetch("https://jsonplaceholder.typicode.com/posts");
      
      if (!res.ok) {
        throw new Error("Network response was not ok");
      }

      const data = await res.json();
      setData(data);
    } catch (err) {
      setError(err);
    } finally {
      setLoading(false);
    }
  };

  fetchData();
}, []);
```

Then you can render a loading message if the data fetching is not complete, an error message if there was an error fetching the data, or the results.

```
if (loading) {
  return <p>Loading...</p>;
}

if (error) {
  return <p>{error.message}</p>;
}

return (
  <ul>
    {data.map((post) => (
      <li key={post.id}>{post.title}</li>
    ))}
  </ul>
);
```

If you want to use Axios, you need to install and import it:

```
npm i axios
```

```
import axios from "axios";
```

Then you can fetch the data using `axios.get`:

```
const [data, setData] = useState(null);
const [loading, setLoading] = useState(true);
const [error, setError] = useState(null);

useEffect(() => {
  const fetchData = async () => {
    try {
      const res = await axios.get(
        "https://jsonplaceholder.typicode.com/users"
      );
      setData(res.data);
    } catch (err) {
      setError(err);
    } finally {
      setLoading(false);
    }
  };

  fetchData();
}, []);
```

To fetch data using the `useSWR` hook, you need to first install and import it.

```
npm i swr
```

```
import useSWR from "swr";
```

Here is how you can use the hook to fetch data:

```
import useSWR from "swr";

const fetcher = (url) => fetch(url).then((res) => res.json());

const FetchTodos = () => {
 const { data, error } = useSWR(
   "https://jsonplaceholder.typicode.com/todos",
   fetcher
 );

 if (!data) {
   return <h2>Loading...</h2>;
 }
 if (error) {
   return <h2>Error: {error.message}</h2>;
 }

 return (
   <>
     <h2>Todos</h2>
     <div>
       {data.map((todo) => (
         <h3 key={todo.id}>{todo.title}</h3>
       ))}
     </div>
   </>
 );
};

export default FetchTodos;
```

Working with the `useOptimistic` Hook
-------------------------------------

* **`useOptimistic` Hook**: This hook is used to keep UIs responsive while waiting for an async action to complete in the background. It helps manage "optimistic updates" in the UI, a strategy in which you provide immediate updates to the UI based on the expected outcome of an action, like waiting for a server response.

Here is the basic syntax:

```
const [optimisticState, addOptimistic] = useOptimistic(actualState, updateFunction);
```

* `optimisticState` is the temporary state that updates right away for a better user experience.
* `addOptimistic` is the function that applies the optimistic update before the actual state changes.
* `actualState` is the real state value that comes from the result of an action, like fetching data from a server.
* `updateFunction` is the function that determines how the optimistic state should update when called.

Here is an example of using the `useOptimistic` hook in a `TaskList` component:

```
"use client";

import { useOptimistic } from "react";

export default function TaskList({ tasks, addTask }) {
  const [optimisticTasks, addOptimisticTask] = useOptimistic(
    tasks,
    (state, newTask) => [...state, { text: newTask, pending: true }]
  );

  async function handleSubmit(e) {
    e.preventDefault();
    const formData = new FormData(e.target);

    addOptimisticTask(formData.get("task"));

    addTask(formData);
    e.target.reset();
  }

  return <>{/* UI */}</>;
}
```

* **`startTransition`**: This is used to render part of the UI and mark a state update as a non-urgent transition. This allows the UI to be responsive during expensive updates. Here is the basic syntax:

```
startTransition(action);
```

The `action` performs a state update or triggers some transition-related logic. This ensures that urgent UI updates (like typing or clicking) are not blocked.

Working with the `useMemo` Hook
-------------------------------

* **Memoization**: This is an optimization technique in which the result of expensive function calls are cached (remembered) based on specific arguments. When the same arguments are provided again, the cached result is returned instead of re-computing the function.
* **`useMemo` Hook**: This hook is used to memoize computed values. Here is an example of memoizing the result of sorting a large array. The `expensiveSortFunction` will only run when `largeArray` changes:

```
const memoizedSortedArray = useMemo(
  () => expensiveSortFunction(largeArray),
  [largeArray]
);
```

Working with the `useCallback` Hook
-----------------------------------

* **`useCallback` Hook**: This is used to memoize function references.

```
const handleClick = useCallback(() => {
  // code goes here
}, [dependency]);
```

* **`React.memo`**: This is used to memoize a component to prevent it from unnecessary re-renders when its prop has not changed.

```
const MemoizedComponent = React.memo(({ prop }) => {
 return (
   <>
     {/* Presentation */}
   </>
 )
});
```

Dependency Management Tools
---------------------------

* **Dependency Definition**: In software, a dependency is where one component or module in an application relies on another to function properly. Dependencies are common in software applications because they allow developers to use pre-built functions or tools created by others. The two core dependencies needed for a React project will be the `react` and `react-dom` packages:

```
"dependencies": {
  "react": "^18.3.1",
  "react-dom": "^18.3.1"
}
```

* **Package Manager Definition**: To manage software dependencies in a project, you will need to use a package manager. A package manager is a tool used for installation, updates and removal of dependencies. Many popular programming languages like JavaScript, Python, Ruby and Java, all use package managers. Popular package managers for JavaScript include npm, Yarn and pnpm.
* **`package.json` File**: This is a key configuration file in projects that contains metadata about your project, including its name, version, and dependencies. It also defines scripts, licensing information, and other settings that help manage the project and its dependencies.
* **`package-lock.json` File**: This file will lock down the exact versions of all packages that your project is using. When you update a package, then the new versions will be updated in the lock file as well.
* **`node_modules` Folder**: This folder contains the actual code for the dependencies listed in your `package.json` file, including both your project's direct dependencies and any dependencies of those dependencies.
* **Dev Dependencies**: These are packages that are only used for development and not in production. An example of this would be a testing library like Jest. You would install Jest as a dev dependency because it is needed for testing your application locally but not needed to have the application run in production.

```
"devDependencies": {
  "@eslint/js": "^9.17.0",
  "@types/react": "^18.3.18",
  "@types/react-dom": "^18.3.5",
  "@vitejs/plugin-react": "^4.3.4",
  "eslint": "^9.17.0",
  "eslint-plugin-react": "^7.37.2",
  "eslint-plugin-react-hooks": "^5.0.0",
  "eslint-plugin-react-refresh": "^0.4.16",
  "globals": "^15.14.0",
  "vite": "^6.0.5"
}
```

React Router
------------

* **Introduction**: React Router is a third party library that allows you to add routing to your React applications. To begin, you will need to install React Router in an existing React project like this:

```
npm i react-router
```

Then inside of the `main.jsx` or `index.jsx` file, you will need to setup the route structure like this:

```
import { StrictMode } from "react";
import { createRoot } from "react-dom/client";
import { BrowserRouter, Routes, Route } from "react-router";
import App from "./App.jsx";

import "./index.css";

createRoot(document.getElementById("root")).render(
  <StrictMode>
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<App />} />
      </Routes>
    </BrowserRouter>
  </StrictMode>
);
```

The `path` and `element` are used to couple the URL and UI components together. In this case, we are setting up a route for the homepage that points to the `App` component.

* **Multiple Views and Route Setup**: It is common in larger applications to have multiple views and routes setup like this:

```
<Routes>
  <Route index element={<Home />} />
  <Route path="about" element={<About />} />

  <Route path="products">
    <Route index element={<ProductsHome />} />
    <Route path=":category" element={<Category />} />
    <Route path=":category/:productId" element={<ProductDetail />} />
    <Route path="trending" element={<Trending />} />
  </Route>
</Routes>
```

The `index` prop in these examples is meant to represent the default route for a given path segment. So the `Home` component will be shown at the root `/` path while the `ProductsHome` component will be shown at the `/products` path.

* **Nesting Routes**: You can nest routes inside other routes which results in the path of the child route being appended to the parent route's path.

```
<Route path="products">
  <Route path="trending" element={<Trending />} />
</Route>
```

In the example above, the path for the trending products will be products/trending.

* **Dynamic Segments**: A dynamic segment is where any part of the URL path is dynamic.

```
<Route path=":category" element={<Category />} />
```

In this example we have a dynamic segment called `category`. When a user navigates to a URL like products/brass-instruments, then the view will change to the `Category` component and you can dynamically fetch the appropriate data based on the segment.

* **`useParams` Hook**: This hook is used to access the dynamic parameters from a URL path.

```
import { useParams } from "react-router";

export default function Category() {
  let params = useParams();
  {/* Accessing the category param: params.category */}
  {/* rest of code goes here */}
}
```

React Frameworks
----------------

* **Introduction**: React frameworks provide features like routing, image optimizations, data fetching, authentication and more. This means that you might not need to set up separate front-end and back-end applications for certain use cases. Examples of React Frameworks include Next.js and Remix.
* **Next.js Routing**: This routing system includes support for dynamic routes, parallel routes, route handlers, redirects, internalization and more.

Here is an example of creating a custom request handler:

```
export async function GET() {
  const res = await fetch("https://example-api.com");
  const data = await res.json();

  return Response.json({ data });
}
```

* **Next.js Image Optimization**: The `Image` component extends the native HTML `img` element and allows for faster page loads and size optimizations. This means that images will only load when they enter the viewport and the `Image` component will automatically serve correctly sized images for each device.

```
import Image from "next/image";

export default function Page() {
  return (
    <Image src="link-to-image-goes-here" alt="descriptive-title-goes-here" />
  );
}
```

Prop Drilling
-------------

* **Definition**: Prop drilling is the process of passing props from a parent component to deeply nested child components, even when some of the child components don't need the props.

State Management
----------------

* **Context API**: Context refers to when a parent component makes information available to child components without needing to pass it explicitly through props. `createContext` is used to create a context object which represents the context that other components will read. The `Provider` is used to supply context values to the child components.

```
import { useState, createContext } from "react";

const CounterContext = createContext();

const CounterProvider = ({ children }) => {
  const [count, setCount] = useState(0);

  return (
    <CounterContext.Provider value={{ count, setCount }}>
      {children}
    </CounterContext.Provider>
  );
};

export { CounterContext, CounterProvider };
```

* **Redux**: Redux handles state management by providing a central store and strict control over state updates. It uses a predictable pattern with actions, reducers, and middleware. Actions are payloads of information that send data from your application to the Redux store, often triggered by user interactions. Reducers are functions that specify how the state should change in response to those actions, ensuring the state is updated in an immutable way. Middleware, on the other hand, acts as a bridge between the action dispatching and the reducer, allowing you to extend Redux's functionality (e.g., logging, handling async operations) without modifying the core flow.
* **Zustand**: This state management solution is ideal for small to medium-scale applications. It works by using a `useStore` hook to access state directly in components and pages. This lets you modify and access data without needing actions, reducers, or a provider.

Debugging React Components Using the React DevTools
---------------------------------------------------

* **React Developer Tools**: This is a browser extension you can use in Chrome, Firefox and Edge to inspect React components and identify performance issues. For Safari, you will need to install the `react-devtools` npm package. After installing React DevTools and opening a React app in the browser, open the browser developer tools to access the two extra tabs provided for debugging React – Components and Profiler.
* **Components Tab**: This tab displays each component for you in a tree view format. Here are some things you can do in this tab:
  + view the app's component hierarchy
  + check and modify props, states, and context values in real time
  + check the source code for each selected component
  + log the component data to the console
  + inspect the DOM elements for the component
* **Profiler Tab**: This tab helps you analyze component performance. You can record component performance so you can identify unnecessary re-renders, view commit durations, and subsequently optimize slow components.

React Server Components
-----------------------

* **Definition**: React Server Components are React components that render exclusively on the server, sending only the final HTML to the client. This means those components can directly access server-side resources and dramatically reduce the amount of JavaScript sent to the browser.

---

## Module 5: Implementing Robust Typing with TypeScript

### Lecture 5.1: What Is Typescript And Why Is It Used In The Industry

# What Is TypeScript, and Why Is It Used in the Industry?

JavaScript is considered a dynamically-typed language. This means that variables can receive any values at run time - declaring a variable as a number does not prevent you from assigning it a string value later, and function parameters can be passed any value.

The challenge of a dynamically-typed language is that the lack of type safety can introduce errors if you are not careful. TypeScript extends the JavaScript language to include static typing, which helps catch those errors before you even deploy your code. But how does it work?

Consider this JavaScript function:

```
const getRandomValue = (array) => {
  return array[Math.floor(Math.random() * array.length)];
}
```

Our `getRandomValue` function takes an array and returns a random value from that array. But because JavaScript does not validate types, there is nothing preventing you from calling the function with a number:

```
console.log(getRandomValue(10));
```

The console output for the current example will return `undefined` because it was expecting an array instead of a number.

But with TypeScript you can define a type for the array parameter:

```
const getRandomValue = (array: string[]) => {
  return array[Math.floor(Math.random() * array.length)];
}
```

This type definition tells TypeScript that the array argument must be an array of strings. Then when you call `getRandomValue` and pass it a number, you get a different type of error called a compiler error.

Most JavaScript runtime environments, such as a browser or Node.js, cannot run TypeScript natively. Instead, you first need to compile, or translate, TypeScript code into regular JavaScript. You can do that with the built-in compiler that comes with the TypeScript language. When you run the compiler, TypeScript will evaluate your code and throw an error for any issues where the types don't match - such as passing a number into a function that expects an array.

You'll learn more about how these types work in the next few lessons. But it's this extra safety that makes TypeScript an appealing language for many developers and organizations.

---

### Lecture 5.2: How Do Primitive Types Work In Typescript

# How Do Primitive Types Work in TypeScript?

In this lesson, you will learn how to work with basic primitive types and how type annotations work for variables.

For the primitive data types `string`, `null`, `undefined`, `number`, `boolean`, and `bigint`, TypeScript offers corresponding type keywords.

For this lesson, we will focus on the commonly used primitives and not go into much detail for `bigint`. The `bigint` data type is a numeric data type in JavaScript to represent numbers larger than the standard integer type.

Let's take a look at each of these primitive types starting with `string`. Here is how you can type a string in TypeScript:

```
let firstName: string = "Angie";
```

Unlike vanilla JavaScript, the variable `firstName` is expecting a `string` type. So if you try to reassign it with a value of a number, then you will get an error like this:

```
let firstName: string = "Angie";
firstName = 9 // Type 'number' is not assignable to type 'string'.
```

The next type we will look at is the `number` type. Here is an example:

```
let age: number = 16;
```

You can assign integer and floats to the `number` type. But if you were to try and reassign a value that is a `bigint` type, then you will get an error like this:

```
let age: number = 16;

// Type 'bigint' is not assignable to type 'number'.
age = 123n;
```

The next type we will look at is the `boolean` type. Here are some examples:

```
let isLoggedIn: boolean = true;
let isAdmin: boolean = false;
```

The last two types are the `null` and `undefined` types.

As you recall from earlier JavaScript lessons, `null` represents an intentional absence of a value. `undefined` means a variable has been declared but has not been assigned a value.

You will see examples of how to work with these types later on when you learn about function types and union types.

Now that you have seen how type annotations work with variables, the question arises on if you need to always explicitly type out your variables.

If you have a simple type annotation like this, then you might not need to use an explicit type.

```
let firstName: string = "Angie";
```

Reason being is because TypeScript will try to automatically infer the types based on its value. So if you write this, TypeScript will understand it is a string.

```
let firstName = "Angie";
```

You should explicitly type your variables when TypeScript cannot clearly infer the type or when you want to enforce a specific type for situations like function parameters or complex objects.

---

### Lecture 5.3: How Do Types Work With Objects And Arrays

# How Do Types Work with Objects and Arrays?

In this lesson, you will learn how to add types for objects and arrays.

Let's take a look at arrays first.

Here is an example of an array of programming languages:

```
const programmingLanguages = ["Java", "C++", "Python"];
```

If you wanted to explicitly type that array as an array of strings, then you can type it as `string[]`:

```
const programmingLanguages:string[] = ["Java", "C++", "Python"];
```

As you learned earlier, TypeScript will be smart enough to infer the type as an array of strings if you just write this:

```
const programmingLanguages = ["Java", "C++", "Python"];
```

But explicitly typing it will help in situations if you attempt to add another type to the array like this:

```
// Type 'number' is not assignable to type 'string'.(2322)
const programmingLanguages:string[] = ["Java", 9, "Python"];
```

Another way to type arrays is to use this syntax:

```
const programmingLanguages:Array<string> = ["Java", "C++", "Python"];
```

Fundamentally, these two syntaxes are the same, and the choice between the two is generally a matter of preference.

Now, let's take a look at typing objects.

Here is an example of an object literal:

```
const developer = {
  firstName: "Jessica",
  isEmployed: true
}
```

To explicitly type the object properties, you can use this syntax:

```
const developer: { firstName: string, isEmployed: boolean } = {
  firstName: "Jessica",
  isEmployed: true
}
```

If you try to add or remove properties from the object, then you will get an error like this:

```
// Property 'isEmployed' is missing in type '{ firstName: string; }' but required in type '{ firstName: string; isEmployed: boolean; }'
const developer: { firstName: string, isEmployed: boolean } = {
  firstName: "Jessica",
}
```

You can make object properties optional by using the `?` after the property name like this:

```
const developer: { firstName: string, isEmployed?: boolean } = {
  firstName: "Jessica",
}
```

TypeScript will no longer display an error because the `isEmployed` property has been marked as optional.

So far, all of the object examples have had restrictive properties. That means we explicitly listed every property the object is allowed to have:

```
const developer: { firstName: string, isEmployed: boolean } = {
  firstName: "Jessica",
  isEmployed: true
}
```

But what if you don't know all of the property names ahead of time? What if you want an object that can have any number of properties but all of the values must follow a specific type?

Well, there are two ways to accomplish this. The first way is to use a `Record` which is a built-in generic utility type in TypeScript.

Here is the basic syntax:

```
Record<Keys, ValueType>
```

The first type represents the type of the keys while the second type represents the type of the values.

Here is an example of using a `Record` for a `userRoles` object:

```
const userRoles: Record<string, string> = {
  admin: "full-access",
  editor: "limited-access",
  viewer: "read-only"
};
```

This `userRoles` object can have any string keys, and all of the values must be strings. If you try to assign a non-string value, you’ll get an error:

```
// Type 'number' is not assignable to type 'string'
const userRoles: Record<string, string> = {
  admin: 1
};
```

The second way to write the same idea is with an index signature:

```
const obj: { [key: string]: string } = {};
```

The syntax above says that any property with a string key must have a string value. Here is an example for a `settings` object:

```
const settings: { [key: string]: string } = {
  theme: "dark",
  language: "en",
  layout: "grid"
};
```

Just like earlier, if you have incorrect value types, TypeScript will display an error message:

```
// Type 'boolean' is not assignable to type 'string'
const settings: { [key: string]: string } = {
  darkMode: true
};
```

Both `Record` and index signatures are fundamentally the same. So choosing between them is mostly a matter of preference.

---

### Lecture 5.4: How Do Function Types Work

# How do Function Types Work?

In this lesson, you will learn how to work with function types. Let's start with parameter type annotations.

Here is an example of a basic function:

```
function circleArea(radius) {
  return Math.PI * radius * radius;
}
```

Right now, TypeScript would display a message of `Parameter 'radius' implicitly has an 'any' type`. The `any` type indicates that a value can have any type. You will learn more about this type in a future lesson.

To get rid of the error and explicitly type the parameter, you can type it like this:

```
function circleArea(radius: number) {
  return Math.PI * radius * radius;
}
```

If you try to call the `circleArea` function with a different type that is not a number, TypeScript will display an error like this:

```
function circleArea(radius: number) {
  return Math.PI * radius * radius;
}

// Argument of type 'string' is not assignable to parameter of type 'number'
circleArea("3");
```

If you try to provide more arguments then the function expects, TypeScript will display an error:

```
function circleArea(radius: number) {
  return Math.PI * radius * radius;
}

// Expected 1 arguments, but got 2.
circleArea(3, 4);
```

If you provide too few arguments, then TypeScript will also display an error:

```
function circleArea(radius: number) {
  return Math.PI * radius * radius;
}

// Expected 1 arguments, but got 0.
// An argument for 'radius' was not provided.
circleArea();
```

You can make parameters optional by the using the `?` symbol near the parameter like this:

```
function area(radius: number, height?: number): number {
  const baseArea = Math.PI * radius * radius;

  if (height !== undefined) {
    const sideArea = 2 * Math.PI * radius * height;
    return baseArea + sideArea;
  }

  return baseArea;
}
```

Keep in mind that optional parameters must always come after required parameters. Placing a required parameter after an optional one will result in a TypeScript error.

The conditional check inside of the function is there in case the `height` argument is not provided.

If you want to type your return values, you can add return type annotations like this:

```
function circleArea(radius: number): number {
  return Math.PI * radius * radius;
}
```

The return type annotation goes after the parameter list. Similar to variable type annotations, most of the time TypeScript will be smart enough to infer the return type. So use an explicit return type annotation when you want to make the function's intent clearer or prevent unintended changes to the return value.

The next example we will look at will deal with asynchronous functions and promises. If your function is going to return a promise, you can use the `Promise` type like this:

```
async function getCityTemperature(city: string): Promise<number> {
  const response = await fetch(`https://api.example.com/weather?city=${city}`);
  const data = await response.json(); 
  return data.temperature;
}
```

In this situation, if you try to remove the return type, TypeScript might infer the return as `Promise<any>`. So this would be a good situation to explicitly type the return value.

Up till this point, we have only looked at named function examples. But how do types work with anonymous functions?

Here is an example using an anonymous function in the callback passed to a `forEach`:

```
const languages = ["JavaScript", "Python", "TypeScript"];

languages.forEach((lang) => {
  console.log(`${lang.toUpperCase()} has ${lang.length} characters`);
});
```

The `lang` parameter does not have a type annotation. Instead, TypeScript uses contextual typing which means it infers the type from the context in which it appears.

---

### Lecture 5.5: What Are Type Aliases And How Do They Work

# What are Type Aliases and How Do They Work?

In the prior lesson, you learned how to work with union types. One common way to work with union types is to use a type alias.

A type alias is a name for a type. Here is an example of providing a name for a union type:

```
type ID = number | string;
```

Often times in your projects, you will create type aliases and use them throughout your program like this:

```
type ID = number | string;

type User = {
  id: ID;
  name: string;
};

function getUserId(user: User): ID {
  return user.id;
}
```

This example uses two types named `ID` and `User`. `ID` would be a union type for `number` or `string` while `User` is an object type with `id` and `name` properties. The `id` is specified with the `ID` type while the `name` has the `string` type.

The `getUserId` function has one parameter called `user` and its type is `User`. The return type for the `getUserId` function would be `ID`.

Type aliases are a great way to describe the shape of an object. It is common to create object types and use them in arrays like this:

```
type User = {
  id: number | string;
  name: string;
};

const users: User[] = [
  { id: 101, name: "Alice" },
  { id: "A102", name: "Bob" },
  { id: 103, name: "Charlie" }
];
```

In this example, the `users` array must be filled with only `User` objects. If you forget a property in one of the objects, then TypeScript will throw an error like this:

```
type User = {
  id: number | string;
  name: string;
};

const users: User[] = [
  // Property 'name' is missing in type '{ id: number; }' but required in type 'User'.
  { id: 101 },
  { id: "A102", name: "Bob" },
  { id: 103, name: "Charlie" }
];
```

You might have noticed the use of PascalCase when it came to naming the type aliases. This is because by convention using PascalCase helps distinguish types from variables. It also helps with readability. When you see `User[]`, you will know it's an array of objects of type `User`.

---

### Lecture 5.6: What Are Interfaces And How Do They Work

# What are Interfaces and How Do They Work?

In a prior lesson, you learned how to work with type aliases and saw examples on how to name object types.

As you recall, one way to name an object type would be to use the `type` keyword like this:

```
type ID = number | string;

type User = {
  id: ID;
  name: string;
};
```

Another way to name an object type would be to use an `interface` declaration like this:

```
type ID = number | string;

interface User {
  id: ID;
  name: string;
}
```

`type` and `interface` are similar but one key difference is that interfaces use the `extends` keyword to build on other interfaces or types, while `type` aliases use intersection types (`&`) to combine types.

Let's look at some examples:

```
interface User {
  id: number | string;
  name: string;
}

interface Admin extends User {
  role: string;
}

const adminUser: Admin = {
  id: 101,
  name: "Alice",
  role: "superadmin"
};
```

In this example, `User` starts with `id` and `name`. The `Admin` interface extends `User`, meaning it includes `id` and `name` and adds a new property called `role`.

If you wanted to extend a `type`, you would use an intersection type (`&`) like this:

```
type User = {
  id: number | string;
  name: string;
};

type Admin = User & {
  role: string;
};

const adminUser: Admin = {
  id: 101,
  name: "Alice",
  role: "superadmin"
};
```

`Admin` combines the `User` type with a new object type that includes `role`. The result is the same shape as the interface example which is an object with `id`, `name`, and `role`.

Both `type` and `interface` can describe the shape of an object. If you're unsure which to use, remember that `interface` is specifically designed for object shapes, while `type` is more flexible and can also represent union types, primitives, and more complex type combinations.

---

### Lecture 5.7: What Are Union Types And How Do They Work

# What are Union Types and How Do They Work?

In the prior lessons, you learned how to work with primitive types like `string`, and `boolean`. But TypeScript allows you to build new types from existing ones. One example of this would be the union type.

A union type is a type that combines two or more other types.

Here is the basic syntax:

```
type1 | type2 | type3
```

Let's take a look at some examples to better understand the concept.

Here is a variable called `id` with a union type for `string` or `number`:

```
let id: string | number = "user_783";
```

The value can be updated to a number which is still valid for the union type:

```
let id: string | number = 1024;
```

If you tried to assign another value that isn't a `string` or `number`, then TypeScript will display an error message:

```
// Type 'string[]' is not assignable to type 'string | number'.
let id: string | number = ["Java", "Python"];
```

When working with union types, it is important to use methods that work for all of the types, otherwise TypeScript will throw an error like this:

```
function getId(id: string | number) {
  // Property 'toUpperCase' does not exist on type 'string | number'.
  return id.toUpperCase();
}
```

There is a solution for this which involves narrowing the union. But you will learn more about that as well as how union types work with type aliases in future lessons.

Union types are also helpful when working with `null` and `undefined` values.

Here is an example where a variable might contain a `string` value, or it might be `null` if no value has been set yet:

```
let username: string | null;

// Type 'number' is not assignable to type 'string | null'.
username = 42;
```

In this case, `username` can either be a `string` or `null`, but nothing else. You might use `null` when you want to intentionally represent the absence of a value.

Here is another example using `undefined`:

```
let score: number | undefined;

score = undefined; 

// Type 'string' is not assignable to type 'number | undefined'.
score = "high";
```

In this example, `score` can either be a `number` or `undefined`. You might use `undefined` when a value has not been assigned yet.

Using union types with `null` and `undefined` makes it clear when a value might be missing, while still allowing TypeScript to catch invalid assignments.

---

### Lecture 5.8: How Do The Any Never Unknown And Void Types Work

# How Do The any, never, unknown and void Types Work?

In prior lessons, you have learned how to work with primitive types as well as union types, and interfaces.

But TypeScript has some special types that you should be aware of. Let's start by looking at the `any` type.

The `any` type is used to represent any type of value.

```
let randomValue: any;

randomValue = 42;           

randomValue = "Hello";     
 
randomValue = true;        

randomValue = { name: "Alice" };
```

With this type, you have to be careful because it can be easily overused and misused. You don't want to type everything with the `any` type just to silence TypeScript error messages. That defeats the purpose of using TypeScript and adding type safety in the first place.

A safer counterpart to the `any` type would be the `unknown` type. `unknown` is similar to `any` but with the `unknown` type, you have to do a type check for the variable before using it.

Here is an example:

```
function doubleValue(value: unknown) {
  if (typeof value === "number") {
    console.log(value * 2);
  } else if (typeof value === "string") {
    console.log(value + value);
  }
}

doubleValue(10);    
doubleValue("Hi "); 
doubleValue(true);
```

In this example, the type checks ensure that operations are only performed on values of the correct type. Values that don't match the expected types are ignored.

The next type we will look at is the `never` type. This type represents something that will never happen.

In most situations, you will not be writing out type annotations using `never`. Instead, you will most likely see the `never` type show up in error messages like this:

```
function processValue(value: string | number) {
  if (typeof value === "string") {
    console.log("String value:", value.toUpperCase());
  } else if (typeof value === "number") {
    console.log("Number value:", value * 2);
  } else {
    console.log(value); 
  }
}
```

Inside the `else` clause of the example above, the `value` has a `never` type. This is because the `else` branch is now impossible to reach and there's no remaining type left. If you tried to call the function with a value other than `string` or `number` it would show an error like this:

```
function processValue(value: string | number) {
  if (typeof value === "string") {
    console.log("String value:", value.toUpperCase());
  } else if (typeof value === "number") {
    console.log("Number value:", value * 2);
  } else {
    console.log(value); 
  }
}

// Argument of type 'boolean' is not assignable to parameter of type 'string | number'.
processValue(true);
```

The last type we will look at is the `void` type. When you have a function that doesn't return a value, that would be a `void` type.

Here is an example:

```
type Status = "loading" | "success" | "error";

type Handler = {
  status: Status;
  onChange: (newStatus: Status) => void; 
};
```

In this example, the `onChange` property for the `Handler` type doesn't return anything which is why `void` is being used.

---

### Lecture 5.9: What Are Type Assertions And How Do They Work

# What are Type Assertions and How Do They Work?

Sometimes there will be situations where you will know more about a type than TypeScript does. This is where type assertions come in handy.

Here is an example using the `querySelector()` method to access an element with the `id` of `submit`:

```
const submitBtn = document.querySelector("#submit");
```

Right now, TypeScript only knows that this `submitBtn` is some sort of `Element` or possibly `null`. TypeScript will not look at the corresponding HTML to figure it out.

This is good place to use a type assertion to tell TypeScript what type of element this is. Here is an example:

```
const submitBtn = document.querySelector("#submit") as HTMLButtonElement;
```

Now, TypeScript will treat this as a `button` element because of that type assertion.

There are limits to using the `as` keyword. For example, you can't do stuff like this without TypeScript throwing an error:

```
// Conversion of type 'string' to type 'number' may be a mistake because neither type sufficiently overlaps with the other. If this was intentional, convert the expression to 'unknown' first.
const age = "awesome" as number;
```

In this example, it doesn't make much sense to try and assert that the string `"awesome"` should be viewed as a number type. TypeScript only allows type assertions between compatible or overlapping types.

One way to remove that error would be to use a double assertion like this:

```
const age = "awesome" as unknown as number;
```

Even though this works in TypeScript, it is still not recommended because logically it doesn't make much sense.

Another way to write type assertions is to use angle bracket syntax like this:

```
const submitBtn = <HTMLButtonElement>document.querySelector("#submit");
```

You need to be careful with this syntax when using `tsx` files because TypeScript will think you are trying to render a component and throw an error like this:

```
// file: index.tsx
// This JSX tag requires 'React' to be in scope, but it could not be found.
// JSX element 'HTMLButtonElement' has no corresponding closing tag.
const submitBtn =  <HTMLButtonElement>document.querySelector("#submit");
```

In most situations, you will see the first syntax using the `as` keyword being used over the second option.

---

### Lecture 5.10: What Are Generics And How Do They Work

# What Are Generics, and How Do They Work?

You have actually seen a generic type in a previous lesson: `Array<string>`. But you'll usually use generic types in functions. In fact, they can be thought of as a special parameter you provide to a function to control the behavior of the function's type definition.

Let's go back to our previous example of a function to get a random value from an array:

```
const getRandomValue = (array: string[]): string => {
  return array[Math.floor(Math.random() * array.length)];
}
```

Our function accepts an array of strings and returns a string. But what if we wanted to pass in an array of numbers and return a number?

You could use a union type:

```
const getRandomValue = (array: (string|number)[]): (string|number) => {
  return array[Math.floor(Math.random() * array.length)];
}
const val = getRandomValue([1, 2, 4])
```

But with this approach, even though we have passed in an array of only numbers, TypeScript determines that the `val` variable could be a number OR a string.

Instead, you can define a generic type for the function:

```
const getRandomValue = <T>(array: T[]): T => {
  return array[Math.floor(Math.random() * array.length)];
}
const val = getRandomValue([1, 2, 4])
```

There are a couple of important components in our new example. First, the `<T>` syntax tells TypeScript that you are defining a generic type `T` for the function. `T` is a common name for generic types, but you can actually name it whatever you want (within JavaScript's variable conventions).

Then, we tell TypeScript that the array parameter is an array of values matching the generic type, and that the returned value is a single element of that same type. This allows TypeScript to properly detect that `val` will be a number, because the array we passed consists solely of numbers.

But what about functions you don't control? Let's take a look at the `document.querySelector()` method:

```
const email = document.querySelector("#email");
console.log(email.value);
```

Because we're querying with an ID selector, TypeScript doesn't know what kind of element we are querying. It knows it's an `Element` of some sort, but our attempt to access the `value` property will throw an error because the top-level element interface does not have that property.

Thankfully, we can pass a type argument to the function call:

```
const email = document.querySelector<HTMLInputElement>("#email");
console.log(email.value);
```

Notice how we're using the angle bracket syntax again (`<HTMLInputElement>`), but this time in a function call. This tells TypeScript that the element we expect to find will be an `input` element, and we no longer get an error on the value property because input elements do have that property. Of course, `querySelector` can return `null` if an element is not found, and TypeScript will throw a compiler error here because we do not handle that case.

But you'll learn about that in the next lesson.

---

### Lecture 5.11: What Is Type Narrowing And How Does It Work

# What Is Type Narrowing, and How Does It Work?

There are going to be times where you have a value with a broad type and you need to narrow it down to a more specific type. For example, maybe you need to ensure an object matches an interface you defined. Or a string is within a specific list of values. There are quite a few ways to achieve this.

The first is narrowing by truthiness. Consider our example from the last lesson:

```
const email = document.querySelector<HTMLInputElement>("#email");
console.log(email.value);
```

We get a compiler error trying to access the `value` property of `email`, because `email` might be `null`. However, we can use a conditional statement to confirm `email` is truthy before accessing the property:

```
const email = document.querySelector<HTMLInputElement>("#email");
if (email) {
  console.log(email.value);
}
```

In this updated example, because `null` is not a truthy value, TypeScript is able to infer that `email` MUST be an `input` element within the conditional block. So it no longer throws a compiler error.

Truthiness checks can also work in the reverse direction:

```
const email = document.querySelector<HTMLInputElement>("#email");
if (!email) {
  throw new ReferenceError("Could not find email element!")
}
console.log(email.value);
```

With this approach, we throw an error if `email` is falsy. `null` is a falsy value. Throwing an error ends the logical execution of this code, which means when we reach the `console.log()` call TypeScript knows `email` cannot be `null`.

Optional chaining is also a form of type narrowing, under the same premise that the property access can't happen if the `email` value is `null`.

```
const email = document.querySelector<HTMLInputElement>("#email");
console.log(email?.value);
```

But what about other types? Well, you can also narrow types using the `typeof` operator. Let's look at an example of a variable we have indicated might be a string OR a number:

```
const myVal = Math.random() > 0.5 ? 222 : "222";
console.log(myVal / 10)
```

In this example, we see a compiler error because we cannot perform arithmetic on a string value. But we can use a conditional to check the `typeof` the `myVal` variable:

```
const myVal = Math.random() > 0.5 ? 222 : "222";
if (typeof myVal === "number") {
  console.log(myVal / 10);
}
```

Because we have used the `typeof` keyword, TypeScript now knows that `myVal` has to be a number, and we can safely perform arithmetic with it.

But what about more complex object types? If the object in question happens to come from a class, you can actually use the `instanceof` keyword to narrow the type. Going back to our `querySelector()` example:

```
const email = document.querySelector("#email");
```

Rather than passing a generic type and telling TypeScript what the element is, we can use `instanceof` to narrow the type and write safer code:

```
const email = document.querySelector("#email");

if (email instanceof HTMLInputElement) {
    console.log(email.value);
}
```

This approach may seem the same as our previous one, but `instanceof` is a runtime validation - which means, if we somehow got the TypeScript type wrong, our JavaScript code will still confirm that `email` is an `input` element.

Next, let's look at an example where we fetch a `User` object from an API and try to print the information:

```
interface User {
    name: string;
    age: number;
}

const printAge = (user: User) => 
  console.log(`${user.name} is ${user.age} years old!`)

const request = await fetch("url")
const myUser = await request.json();
printAge(myUser);
```

We'll get a compiler error trying to pass `myUser` into the function because, even though we know the API returns the correct object, TypeScript does not. And the `.json()` method does not take a generic type.

The "easy" way to resolve this issue would be to cast the type:

```
interface User {
    name: string;
    age: number;
}

const printAge = (user: User) => 
  console.log(`${user.name} is ${user.age} years old!`)

const request = await fetch("url")
const myUser = await request.json() as User;
printAge(myUser);
```

But whenever you cast the type, you're essentially weakening TypeScript's ability to catch potential errors. So instead of casting the type, you can write a type guard:

```
interface User {
    name: string;
    age: number;
}

const isValidUser = (user: unknown): user is User => {
  return !!user && 
    typeof user === "object" &&
    "name" in user &&
    "age" in user;
}
```

The return type here is the key component of this function definition. The `user is User` syntax indicates that our function returns a boolean value, which when `true` means the `user` value satisfies the `User` interface. We then do some basic checks to ensure that the structure of the `user` object matches - note the use of a truthiness (`!!user`) narrowing and a `typeof` narrowing. We must do this because `typeof null` returns `"object"`:

```
interface User {
    name: string;
    age: number;
}

const isValidUser = (user: unknown): user is User => {
  return !!user && 
    typeof user === "object" &&
    "name" in user &&
    "age" in user;
}

const printAge = (user: User) => 
  console.log(`${user.name} is ${user.age} years old!`)

const request = await fetch("url")
const myUser = await request.json() as User;
if (isValidUser(myUser)) {
    printAge(myUser);
}
```

Now, if we combine all of our logic together, we no longer get compiler errors and can successfully build our code.

Type narrowing is a powerful feature that helps you write safer, less error-prone code - but remember that TypeScript types are not completely rigid, so avoid practices like casting the type of a value without narrowing it.

---

### Lecture 5.12: What Is A Tsconfig File And Why Is It Important To Include In Your Typescript Projects

# What Is a tsconfig File, and Why Is It Important to Include in Your TypeScript Projects?

TypeScript's compiler settings can be configured to meet your project's needs. That configuration lives in a `tsconfig.json` file in the root directory of your project. In fact, without it, the compiler will not run unless you pass it command flags directly. But what exactly does this file do? Well, let's take a look at an example file:

```
{
  "compilerOptions": {
    "rootDir": "./src",
    "outDir": "./prod",
    "lib": ["ES2023"],
    "target": "ES2023",
    "module": "ES2022",
    "moduleResolution": "Node",
    "esModuleInterop": true,
    "skipLibCheck": true,
    "strict": true
  },
  "exclude": ["test/"]
}
```

This seems like a lot! So let's break it down. The `compilerOptions` property is going to contain the "meat" of your configuration - this is where you control how the TypeScript compiler behaves. Looking at that nested object…

The `rootDir` and `outDir` tell TypeScript which directory holds your source files, and which directory should contain the transpiled JavaScript code.

The `lib` property determines which type definitions the compiler uses, and allows you to include support for specific ES releases, the DOM, and more.

`module` and `moduleResolution` effectively work in tandem to manage how your package uses modules - either CommonJS or ECMAScript.

`esModuleInterop` allows for smoother interoperability between CommonJS and ES modules by automatically creating namespace objects for imports, making it easier to use modules from different systems together in your TypeScript projects, and the `skipLibCheck` option skips validating `.d.ts` files that aren't referenced by imports in your code.

And finally we reach the `strict` mode. One might argue that TypeScript isn't truly helpful without this flag enabled, as it toggles quite a few other checks, such as requiring you to properly handle nullable types, or warn when TypeScript can't infer a type and falls back to any.

Before we finish, a quick note about the top-level `exclude` property - when you've defined a source directory, you may have TypeScript code outside of that directory which you don't want compiled as part of your production code. For example, your test code. The `exclude` array tells the compiler to ignore these TypeScript files during compilation, but still allows tooling like Intellisense to expose potential issues.

There are a ton of other compiler options you can explore - over 50! I encourage you to explore the documentation and experiment to find the configuration that works for your project's needs.

---

### Typescript

# TypeScript Review

What is TypeScript
------------------

* **JavaScript**: JavaScript is a dynamically-typed language. This means that variables can receive any values at run time. The challenge of a dynamically-typed language is that the lack of type safety can introduce errors.

For example, even if your JavaScript function expects an array, you can still call it with a number:

```
const getRandomValue = (array) => {
  return array[Math.floor(Math.random() * array.length)];
}

console.log(getRandomValue(10));
```

The `console` output for the example above will be `undefined`.

* **TypeScript**: TypeScript extends the JavaScript language to include static typing, which helps catch errors caused by type mismatches before you run your code.

For example, you can define a type for the `array` parameter as follows:

```
const getRandomValue = (array: string[]) => {
  return array[Math.floor(Math.random() * array.length)];
}
```

This type definition tells TypeScript that the `array` parameter must be an array of strings. Then, when you call `getRandomValue` and pass it a number, you get an error called a compiler error.

* **Compiler**: You first need to compile TypeScript code into regular JavaScript. When you run the compiler, TypeScript will evaluate your code and throw an error for any issues where the types don't match.

Data Types in TypeScript
------------------------

* **Primitive Data Types in TypeScript**: For the primitive data types `string`, `null`, `undefined`, `number`, `boolean`, and `bigint`, TypeScript offers corresponding type keywords.

```
let str: string = "Naomi";
let num: number = 42;
let bool: boolean = true;
let nope: null = null;
let nada: undefined = undefined;
```

* **Array**: You can define an array of specific type with two different syntaxes.

```
const arrOne: string[] = ["Naomi"];
const arrTwo: Array<string> = ["Camperchan"];
```

* **Objects**: You can define the exact structure of an object.

```
const obj: { a: string, b: number } = { a: "Naomi", b: 42 };
```

If you want an object with any keys, but where all values must be strings, there are two ways to define it:

```
const objOne: Record<string, string> = {};
const objTwo: { [key: string]: string } = {};
```

* **Other Helpful Types in TypeScript**:

  + **`any`**: `any` indicates that a value can have any type. It tells the compiler to stop caring about the type of that variable.
  + **`unknown`**: `unknown` tells TypeScript that you *do* care about the type of the value, but you don’t actually know what it is. `unknown` is generally preferred over `any`.
  + **`void`**: This is a special type that you’ll typically only use when defining functions. Functions that don’t have a return value use a return type of `void`.
  + **`never`**: It represents a type that will never exist.
* **`type` Keyword**: This keyword is like `const`, but instead of declaring a variable, you can declare a type.

It is useful for declaring custom types such as union types or types that include only specific values:

```
type stringOrNumber = string | number;
type bot = "camperchan" | "camperbot" | "naomi";
```

* **`interface`**: Interfaces are like classes for types. They can implement or extend other interfaces, are specifically object types, and are generally preferred unless you need a specific feature offered by a `type` declaration.

```
interface wowie {
  zowie: boolean;
  method: () => void;
}
```

* **Defining Return Type**: You can also define the *return type* of the function.

The example below defines the return value as a string. If you try to return anything else, TypeScript will give a compiler error.

```
const getRandomValue = (array: string[]): string => {
  return array[Math.floor(Math.random() * array.length)];
}
```

Generics
--------

* **Defining Generic Type**: You can define a generic type and refer to it in your function. It can be thought of as a special parameter you provide to a function to control the behavior of the function's type definition.

Here is an example of defining a generic type for a function:

```
const getRandomValue = <T>(array: T[]): T => {
  return array[Math.floor(Math.random() * array.length)];
}
const val = getRandomValue([1, 2, 4])
```

The `<T>` syntax tells TypeScript that you are defining a generic type `T` for the function. `T` is a common name for generic types, but you can use any name.

Then, you tell TypeScript that the `array` parameter is an array of values matching the generic type, and that the returned value is a single element of that same type.

* **Specifying Type Argument in Function Call**: You can pass a type argument to a function call using angle brackets between the function name and its parameters.

Here is an example of passing a type argument to a function call:

```
const email = document.querySelector<HTMLInputElement>("#email");
console.log(email.value);
```

This tells TypeScript that the element you expect to find will be an input element.

Type Narrowing
--------------

* **Narrowing by Truthiness**: In the example below, you get a compiler error trying to access the `value` property of `email` because `email` *might* be `null`.

```
const email = document.querySelector<HTMLInputElement>("#email");
console.log(email.value);
```

You can use a conditional statement to confirm `email` is *truthy* before accessing the property:

```
const email = document.querySelector<HTMLInputElement>("#email");
if (email) {
  console.log(email.value);
}
```

Truthiness checks can also work in the reverse direction:

```
const email = document.querySelector<HTMLInputElement>("#email");
if (!email) {
  throw new ReferenceError("Could not find email element!")
}
console.log(email.value);
```

Throwing an error ends the logical execution of this code, which means when you reach the `console.log()` call, TypeScript knows `email` *cannot* be `null`.

* **Optional Chaining**: Optional chaining `?.` is also a form of type narrowing, under the same premise that the property access can't happen if the `email` value is `null`.

```
const email = document.querySelector<HTMLInputElement>("#email");
console.log(email?.value);
```

* **`typeof` Operator**: You can use a conditional to check the type of the variable using the `typeof` operator.

```
const myVal = Math.random() > 0.5 ? 222 : "222";
if (typeof myVal === "number") {
  console.log(myVal / 10);
}
```

* **`instanceof` Keyword**: If the object comes from a class, you can use the `instanceof` keyword to narrow the type.

```
const email = document.querySelector("#email");

if (email instanceof HTMLInputElement) {
    console.log(email.value);
}
```

* **Casting**: When TypeScript cannot automatically determine the type of a value, such as the result from `request.json()` method in the example below, you'll get a compiler error. One way to resolve this is by casting the type, but doing so weakens TypeScript's ability to catch potential errors.

```
interface User {
    name: string;
    age: number;
}

const printAge = (user: User) => 
  console.log(`${user.name} is ${user.age} years old!`)

const request = await fetch("url")
const myUser = await request.json() as User;
printAge(myUser);
```

* **Type Guard**: Instead of casting the type, you can write a type guard:

```
interface User {
    name: string;
    age: number;
}

const isValidUser = (user: unknown): user is User => {
  return !!user && 
    typeof user === "object" &&
    "name" in user &&
    "age" in user;
}
```

The `user is User` syntax indicates that your function returns a boolean value, which when true means the `user` value satisfies the `User` interface.

`tsconfig` File
---------------

* **`tsconfig.json`**: TypeScript's compiler settings live in a `tsconfig.json` file in the root directory of your project.

```
{
  "compilerOptions": {
    "rootDir": "./src",
    "outDir": "./prod",
    "lib": ["ES2023"],
    "target": "ES2023",
    "module": "ES2022",
    "moduleResolution": "Node",
    "esModuleInterop": true,
    "skipLibCheck": true,
    "strict": true
  },
  "exclude": ["test/"]
}
```

Here are descriptions of the compiler options used in the example above:

* **`compilerOptions`**: The `compilerOptions` property is where you control how the TypeScript compiler behaves.
* **`rootDir` and `outDir`**: The `rootDir` and `outDir` tell TypeScript which directory holds your source files, and which directory should contain the transpiled JavaScript code.
* **`lib`**: The `lib` property determines which type definitions the compiler uses, and allows you to include support for specific ES releases, the DOM, and more.
* **`module` and `moduleResolution`**: The `module` and `moduleResolution` work in tandem to manage how your package uses modules - either CommonJS or ECMAScript.
* **`esModuleInterop`**: The `esModuleInterop` allows for smoother interoperability between CommonJS and ES modules by automatically creating namespace objects for imports.
* **`skipLibCheck`**: The `skipLibCheck` option skips validating `.d.ts` files that aren't referenced by imports in your code.
* **`strict`**: The `strict` flag enables several checks, such as ensuring proper handling of nullable types and warning when TypeScript falls back to `any`.
* **`exclude`**: The top-level `exclude` property tells the compiler to ignore these TypeScript files during compilation.

---

## Module 6: Optimizing Core Web Performance & Experience

### Lecture 6.1: What Are The Key Performance Concepts

# What Are the Key Performance Concepts?

Why do some websites feel snappy and responsive, while others feel sluggish? The answer lies in key performance concepts that affect how a page loads and renders. Understanding key web performance concepts is essential for building fast, smooth, and user-friendly websites.

Let's break down source order, the critical rendering path, latency, and more.

Let's look at source order first.

Source order refers to the way HTML elements are structured in the document. This determines what loads first and can significantly impact performance and accessibility.

Some best practices for this include:

* Placing critical content such as headings, navigation or main text higher in the HTML structure.
* Deferring non-essential scripts such as ones for analytics, or third-party widgets, so they don't block rendering.
* Using progressive enhancement, to ensure the core experience works even before styles and scripts load. Progressive enhancement is a way of building websites and applications based on the idea that you should make your page work with HTML first.

Here is an example of good source order, using the best practices we just went through.

```
<!-- Good source order: Essential content first -->
<h1>Welcome to FastSite!</h1>
<p>Critical information loads first.</p>
<script src="slow-script.js" defer></script>
```

By optimizing source order, we make sure users see important content as soon as possible.

Now let's look at critical rendering path.

The critical rendering path is the sequence of steps the browser follows to convert code into pixels on the screen.

Here are the key steps that we will go into later:

1. Parsing HTML: Builds the DOM (Document Object Model)
2. Parsing CSS: Builds the CSSOM (CSS Object Model)
3. JavaScript Execution: Can modify the DOM & CSSOM
4. Render Tree Construction: Combines the DOM & CSSOM
5. Layout & Painting: Determines element sizes & draws pixels
6. Optimizations:

   * Minimize render-blocking resources (e.g., large CSS files, unused JS).
   * Use async and defer attributes for scripts:
   * Load only essential styles first; defer non-critical CSS.

Overall, a shorter critical rendering path equals a faster perceived performance. We will go into this in more detail later on.

And finally, let's look at latency.

Latency is the time it takes for a request to travel between the browser and the server. So in other words, high latency equals slow pages.

Some ways of reducing latency include:

* Using CDNs, or in other words, Content Delivery Networks, to serve files from closer locations.
* Enabling compression using things such as Gzip to reduce file sizes.
* Optimizing images and using lazy loading - which we will also go into later.

By reducing latency, we make interactions feel instant.

So in conclusion, by optimizing source order, reducing the critical path, and cutting down latency, you can make your website feel fast.

---

### Lecture 6.2: How Does A Browser Render A Page

# How Does a Browser Render a Page?

Have you ever wondered what happens behind the scenes when you enter a URL and press enter? How does the browser transform code into the interactive pages we see?

Understanding how a browser renders a web page is essential for developers aiming to optimize performance and enhance user experience.

In this lesson, we'll demystify the rendering process, breaking it down into clear, digestible steps.

First the browser parses the HTML and builds the DOM.

The process begins with the browser fetching the HTML content of the page. It parses this HTML to construct the Document Object Model, or DOM — a tree-like structure representing the page's content.

Consider this simple HTML snippet:

```
<html>
  <body>
    <h1>Hello, World!</h1>
    <p>Welcome to our website.</p>
  </body>
</html>
```

The browser parses this to create a DOM tree with `html` as the root, containing `body`, which in turn contains `h1` and `p` elements.

Next, the browser processes the CSS, constructing the CSS Object Model, or CSSOM. This is another tree structure that dictates how elements should be styled.

Given this CSS:

```
h1 {
  color: blue;
}
p {
  font-size: 16px;
}
```

The CSS Object Model specifies that `h1` elements are blue and `p` elements have a font size of 16 pixels.

The browser then combines the DOM and CSS Object Model to form the render tree. This tree includes only the nodes needed to render the page, each paired with its corresponding styles.

For our example, the render tree consists of the `h1` and `p` elements, styled appropriately.

With the render tree in hand, the browser calculates the exact position and size of each element in a process called layout or reflow. This ensures that elements appear in the correct location and dimensions on the screen.

Finally, the browser paints the pixels to the screen, rendering each element based on the calculated styles and layout. In complex pages, this might involve multiple layers that are composited together to form the final visual output.

In conclusion, from parsing HTML and CSS to painting pixels on the screen, the browser's rendering process is a sophisticated sequence of steps.

---

### Lecture 6.3: What Is The Difference Between Real Performance And Perceived Performance

# What Is the Difference Between Real Performance and Perceived Performance?

When we talk about performance, the term itself can feel a bit subjective, right? What is good performance? What is bad performance?

Is there a standard way to measure performance or is it completely dependent on the user's personal preferences and perception? Let's see.

We can classify a website's performance into two different categories: perceived performance and real performance.

The perceived performance is how users perceive the performance of a website. It's how they evaluate it in terms of responsiveness and reliability. This is a subjective measurement, so it's hard to quantify it, but it's very important, since the user experience determines the success or failure of a website.

In contrast, real performance is the objective and measurable performance of the website. It's measured using metrics like page load time, server response time, and rendering time. These measurements are influenced by multiple factors related to the network and to the code itself.

Even a website with excellent perceived performance can be further optimized for an even better user experience.

There are several techniques for improving perceived performance.

Reducing the initial load time as much as possible by loading non-essential resources in the background is essential. This technique is known as "lazy loading." That first impression can determine what users will think about your website.

Lazy loading will also impact the real performance of your website. By using this technique, you can reduce the amount of content that has to be loaded upfront, so the page will load faster, which is a real performance metric.

It's also very important to provide quick response and feedback to user interactions.

For example, showing a loading indicator for a long-running process as soon as the user clicks on an element can help the user feel connected and engaged with the process, making the wait time feel shorter - or at least they'll feel more involved.

Keeping users actively engaged with your website is very important for improving their time perception. Displaying text as soon as it arrives is helpful for keeping users engaged from the start, even if other resources, like images, have not been loaded yet.

If a user is waiting for a long-running task to be completed, keep them informed on the progress and update it regularly.

Another tip is to avoid content reflow and jumping content. For example, when ads or images are being loaded, the website might jump or readjust to make room for these new resources if they don't already have a space in the layout.

These sudden changes can result in a bad user experience because users may feel like the website is still loading. To avoid this, plan ahead and assign space for these elements from the start.

If your website has custom fonts, you should also try to minimize font loading delays, since this may result in flickering - or showing the fallback font while the custom font is being loaded. A suggestion for this is using a fallback font that is similar to the custom font, so in case this happens, the change will be much more subtle.

Also, be sure that the interface elements are active. The user should be able to interact with them with minimal lag.

We will go into these techniques in more detail in the next few lessons.

While real performance is important, perceived performance can have a tremendous impact on user experience. By optimizing for both, you can create websites that are and feel faster, creating a smooth and engaging user experience.

---

### Lecture 6.4: What Are Some Key Metrics For Measuring Performance

# What Are Some Key Metrics for Measuring Performance?

To measure and improve web performance, we use key performance metrics like First Contentful Paint (or FCP), Speed Index, Total Blocking Time (or TBT), Bounce Rate, and Unique Users. Let's look at all of these metrics individually.

First Contentful Paint, or FCP. This measures how quickly the first piece of content, like a text or image, appears on the screen. A good FCP is regarded as a time below 1.8 seconds, and a poor FCP is usually above 3 seconds. You can check your FCP using Chrome DevTools like this:

Step 1: Open Chrome DevTools

* Open Google Chrome.
* Go to the webpage you want to test.
* Press "F12" or Right-click and "Inspect".

Step 2: Find and click the "Lighthouse" tab in the DevTools.

Step 3: Click the "Analyze page load" button and wait for the analyzation to finish.

Now we can analyze the results. We do this by scrolling down to the "Metrics" section and looking for the "First Contentful Paint" marker. We can see the exact time in milliseconds or seconds.

FCP and Interaction to Next Paint (or INP), that we looked at previously, are both performance metrics, but they measure different aspects of user experience. It's important not to get them mixed up.

As a reminder, FCP is about how fast users see content after loading, and INP is about how fast users see feedback after clicking or typing.

Next we have the Speed Index.

Speed Index measures how quickly visible parts of the page are painted. Lower scores mean better performance! You can check your Speed Index in the Lighthouse Reports.

We also have Total Blocking Time or TBT. This shows how long the main thread is blocked by heavy JavaScript tasks. If TBT is high, users experience laggy interactions. To improve TBT, break up long tasks and defer non-essential scripts.

Next we have the Bounce Rate. This is the percentage of visitors who leave without interacting. If your site has high bounce rates, it might be because your page is too slow.

And finally we have unique users. This metric tracks how many individual visitors come to your site. To view the bounce rate and unique users, you can use Google Analytics. It will allow you to monitor these metrics and improve engagement.

---

### Lecture 6.5: What Is Inp

# What Is INP?

Have you ever clicked on a webpage and felt like nothing happened? This delay impacts user experience and is measured by a metric called Interaction to Next Paint, or INP.

INP assesses a page's overall responsiveness by measuring the time from when a user interacts — like a click or key press — to the next time the browser updates the display. A lower INP indicates a more responsive page.

But why is INP important? A high INP can make users feel that a page is unresponsive, leading to frustration. Optimizing INP ensures that users receive timely feedback, enhancing their experience.

Tools like Chrome's DevTools and web performance APIs can help measure INP by tracking interaction delays.

To improve INP, minimize main thread work, optimize event handlers, and ensure that user interactions trigger timely visual updates.

By understanding and optimizing INP, you can create web experiences that feel fast and responsive, keeping your users satisfied.

---

### Lecture 6.6: How To Measure And Improve Inp

# How to Measure and Improve INP?

Let's walk through a practical way to measure Interaction to Next Paint, or INP, using Chrome DevTools.

First of all, let's open DevTools by pressing "F12" or Right-click and click on "Inspect".

Now, let's say you have a search bar on your webpage.

Imagine a user types a query, but it takes 600ms before the suggestion dropdown appears. Chrome DevTools would mark this high INP value.

You can optimize by deferring heavy JavaScript, reducing long tasks, and improving event handling. The INP would then drop to 150ms, making interactions feel instant.

Cool, right?

Now, let's look at a practical measurement technique that helps identify interaction delays so you can create a faster and smoother user experience!

First, we would open Chrome DevTools. We would do so, once again, by opening Google Chrome, navigating to a webpage that we want to analyze, and pressing "F12" or right-clicking the page and clicking "Inspect". Now, let's head to the "Performance" tab - and there is everything that you need.

Now we are ready to identify the Interaction to Next Paint, or INP. We are going to look for the longest interaction delay recorded. A good INP is generally below 200ms, and a poor INP is above 500ms. And that's it!

---

### Lecture 6.7: What Are Some Common Performance Measurement Tools

# What Are Some Common Performance Measurement Tools?

If you want to make your website faster and more responsive, you need the right tools to measure and optimize performance. Let's explore some common performance measurement tools and how they help.

First up, we have Chrome DevTools.

Chrome DevTools is a built-in tool inside Google Chrome that lets you analyze and debug performance in real-time. DevTools will show loading times, CPU usage, and render delays. It's especially useful for measuring First Contentful Paint, or FCP, which we know by now, is how fast a user sees the first visible content. If your website feels slow, DevTools will help you spot the bottlenecks.

Next up, Lighthouse.

Lighthouse is an automated tool that checks performance, SEO, and accessibility. To use it, simply open Chrome DevTools and go to the "Lighthouse" tab. Next, click "Analyze page load" and it will give you a score on how fast and optimized your site is, as well as provide recommendations to improve it. If you want a quick performance audit, Lighthouse is your go-to tool.

Now, let's talk about WebPageTest.

WebPageTest lets you test how your site loads from different locations and devices. All you have to do is visit WebPageTest.org, enter your website URL, choose a test location and browser and click "Start Test". It gives a detailed breakdown of your site's Speed Index, Total Blocking Time, and other key performance metrics. If you want to know how real users experience your site globally, WebPageTest is the tool for that.

Another great tool is Google PageSpeed Insights.

This tool analyzes your website and suggests quick improvements for both mobile and desktop. Just go to PageSpeed Insights, enter your URL, and click "Analyze". It will tell you what's slowing your site down and give specific recommendations — like optimizing images, removing render-blocking scripts, and reducing server response times. PageSpeed Insights is a fast and easy way to check how Google sees your site's performance.

Lastly, let's talk about Real User Monitoring, or RUM tools. Unlike lab tests, RUM tools track actual user behavior, showing how real visitors experience your site. Popular RUM tools include Google Analytics, which tracks page load times and bounce rates. And New Relic or Datadog, which Monitors real-time performance issues. If you want data from actual users, RUM tools are essential.

Each tool has different strengths, so use a combination to get the best insights. Start by testing with Chrome DevTools or Lighthouse, then dive deeper with WebPageTest and RUM tools.

---

### Lecture 6.8: How Can You Use Performance Web Apis To Create Your Own Performance Measurement Tools

# How Can You Use Performance Web APIs to Create Your Own Performance Measurement Tools?

While tools like Lighthouse and Chrome DevTools are great, sometimes you need custom insights tailored to your site.

That's where Performance Web APIs come in!

In this lesson, we'll break down how to use three key Web APIs to measure and analyze your website's speed.

But first, what are Performance Web APIs?

Performance Web APIs let developers track how efficiently a webpage loads and responds, directly from code. These APIs allow you to measure page load times, track rendering and interaction delays and analyze JavaScript execution time.

With these APIs, you can build your own performance monitoring tools without relying on third-party software!

Let's explore three powerful Web APIs you can use today.

First up, `performance.now()`.

This API gives you high-precision timestamps (in milliseconds) to measure how long different parts of your site take to load.

Let's say you want to measure how fast a function runs:

```
const start = performance.now();  
// Run some code here  
const end = performance.now();  

console.log(`Execution time: ${end - start}ms`);
```

This is more accurate than using `Date.now()` because it measures time in milliseconds with microsecond precision, avoiding clock drift issues. You can use it to track script execution time, event response delays, and animation performance.

Next, the Performance Timing API.

This API gives you a breakdown on every single stage of page loading, from DNS lookup to `DOMContentLoaded`.

Want to measure how long your page takes to fully load?

```
let [navigationTiming] = performance.getEntriesByType("navigation");

if (navigationTiming instanceof PerformanceNavigationTiming) {
  // Calculate time from navigation start to DOM content loaded
  const pageLoadTime =
    navigationTiming.domContentLoadedEventEnd - navigationTiming.startTime;

  console.log("DOM Content Loaded Time:", pageLoadTime, "ms");
}
```

Key metrics you can track with this API are DNS lookup time - or in other words the connection speed, Time to First Byte (TTFB) - or server response speed, and `DOMContentLoaded` - or in other words, when the page is ready for interaction.

If your page load times are slow, this API pinpoints exactly where the delay happens!

And finally, let's talk about `PerformanceObserver`.

This API listens for performance events such as layout shifts, long tasks, and user interactions.

Want to monitor long-running JavaScript tasks?

```
const observer = new PerformanceObserver((list) => {  
  list.getEntries().forEach((entry) => {  
    console.log(`Long task detected: ${entry.duration}ms`);  
  });  
});  

observer.observe({ type: "longtask", buffered: true });
```

And what can this API track? Well, it can track long tasks - or in other words, JavaScript that blocks rendering, layout shifts to detect UI jank, and First Input Delay (FID) - or how fast a page responds to user input.

If you want real-time performance tracking, this API is a game-changer.

So, which API should you use? Here's a quick comparison:

| Performance API | Best For |
| --- | --- |
| `performance.now()` | Precise timing of functions and scripts |
| Performance Timing API | Measuring full page load performance |
| Performance Observer | Real-time monitoring of interactions and rendering |

By combining these APIs, you can build your own performance measurement tools and track exactly what matters for your site most.

---

### Lecture 6.9: What Are Some Ways To Reduce Page Loading Times

# What Are Some Ways to Reduce Page Loading Times?

Have you ever left a website because it took too long to load? Slow page loading can frustrate users and increase bounce rates. Today, we'll explore practical ways to reduce page loading times, ensuring your audience stays engaged.

Number 1: optimize media assets. Large images and videos are common culprits for slow load times. By optimizing these assets, you can significantly speed up your site:

* Compress Images: Use tools like TinyPNG to reduce image file sizes without compromising quality.
* Use Modern Formats: Implement formats like WebP for images and AV1 for videos to achieve better compression rates.
* Lazy Loading: Defer loading off-screen images and videos until they're needed. In HTML, add the `loading="lazy"` attribute to your media tags.

Next, we have to minimize HTTP requests. Each file your website requests adds to the load time. Reducing the number of HTTP requests can lead to faster page loads. You can:

* Combine Files: Merge CSS and JavaScript files to reduce the number of requests.
* Use Inline Critical CSS: Place essential CSS directly in the HTML to speed up initial rendering.
* Use CSS Sprites: Combine multiple images into a single sprite sheet to minimize requests.

And, of course, you can Leverage Browser Caching. Caching allows browsers to store parts of your website locally, reducing load times for returning visitors:

* Set Expiry Headers: Use the `Cache-Control` header to specify how long browsers should keep files.
* Version Assets: When updating files, change their names or use query strings to ensure browsers fetch the latest versions.

You can do this along with minifying and Compressing files, which will reduce the size of your files can lead to quicker downloads:

* Minify CSS and JavaScript: Remove unnecessary whitespace and comments using tools like UglifyJS for JavaScript and cssnano for CSS.
* Enable Compression: Configure your server to use Gzip to reduce the size of transmitted files.

You can also optimize web fonts. Web fonts can enhance design but may also slow down your site if not handled properly:

* Limit Font Variants: Only include the character sets and styles you need.
* Use `font-display`: Control how fonts are displayed during loading by setting the `font-display` property in your CSS.

So in conclusion, by implementing all these strategies, you can significantly reduce your page loading times, leading to a better user experience and improved site performance.

---

### Lecture 6.10: How Do You Improve Time To Usable

# How Do You Improve "Time to Usable"?

Improving the "time to usable", or in other words the interval from when a user requests a page to when they can meaningfully interact with it, is crucial for enhancing user experience.

Let's explore effective strategies to achieve a faster time to usable.

Begin by focusing on the content that the user sees first. This means loading essential elements immediately and deferring non-critical components.

For example, you could try to implement lazy loading.

We have already covered lazy loading, but here is an example of lazy load images as a refresher:

```
<img src="image.jpg" loading="lazy" alt="Description">
```

All you need to do is add the `loading="lazy"` attribute to image tags. This defers the loading of images until they are needed, typically when they enter the user's viewport. By loading images and videos only when they enter the viewport, we are conserving bandwidth as well as causing the speed up of initial rendering.

Normally, a webpage loads all images at once, even those not visible on the screen. With lazy loading, images below the fold, or in other words off-screen, they are only loaded when the user scrolls down to them.

And here is an example of lazy load iframes:

```
<iframe src="video.html" loading="lazy"></iframe>
```

You can apply the same attribute that you did before, but this time to iframes, and the same concept will apply.

You can also use the `defer` attribute to delay non-critical JavaScript until after the initial page load. Here is an example of us doing just that:

```
<script src="non-critical.js" defer></script>
```

You could also consider minimizing render-blocking resources.

Render-blocking resources delay the page from becoming interactive.

To avoid this, you could try loading CSS asynchronously. For non-critical CSS, use the `media` attribute to load stylesheets conditionally. Here is an example of us doing just that:

```
<link rel="stylesheet" href="print.css" media="print">
```

By specifying media value as `print`, the `print.css` will only be loaded when the page is printed or previewed on screen. In this next example, by passing `min-width: 800px` as the value to the `media` attribute, we are saying we only want `desktop.css` to load for screens wider than 800px:

```
<!-- This stylesheet is only loaded on screens wider than 800px -->
<link rel="stylesheet" href="desktop.css" media="(min-width: 800px)">
```

This saves bandwidth by skipping unnecessary styles.

So, in conclusion, by implementing these strategies, you can significantly reduce the "time to usable" for your website, ensuring users can interact with your content promptly.

---

### Lecture 6.11: What Are Some Techniques For Improving Css Performance

# What Are Some Techniques for Improving CSS Performance?

Every project is unique and you should carefully consider which ones of these techniques will be most helpful for your web application.

First, since all styles are parsed, you should remove any unnecessary styles from your CSS stylesheets.

You should also split your CSS styles into multiple files. This way, if a file is not required to render a specific web page, it will not be loaded and it won't block the rendering process.

By default, the browser assumes that all stylesheets should block the rendering process. But you can tell the browser when a stylesheet should be loaded by using the `media` attribute and a media query.

In this example, the `print.css` stylesheet will only be applied when the document is being printed because it has the `media` attribute with the value `print`:

```
<link rel="stylesheet" href="print.css" media="print" />
```

You can also minify your CSS files automatically to reduce their size during the build process and compress these files in the server where you host your web application.

Try to keep your CSS selectors as simple as possible and don't try to select more elements than necessary.

Take advantage of the cascading nature of CSS whenever possible. Some styles will be inherited.

Preloading resources with `rel="preload"` is another important technique. Critical assets should be loaded first.

Remember that CSS animations can have an impact on performance.

Animating certain CSS properties, such as dimensions, position, and layout, triggers a process called "reflow," during which the browser recalculates the position and geometry of certain elements on the page. This requires a repaint, which is computationally expensive.

Therefore, it's recommended to reduce the number of CSS animations as much as possible or at least give the user an option to toggle them on or off.

And even though fonts can enhance the visual presentation of your web application, they can have an impact on performance. Some fonts have large files, up to multiple megabytes. Try to use two or three fonts at most and use web-safe fonts whenever possible.

You may also consider preloading the most important fonts to have them ready for quick use.

These are some of the most important and commonly used techniques for optimizing CSS in web development. By incorporating them, you can optimize your website's performance to create a smooth user experience.

---

### Lecture 6.12: What Are Some Techniques For Improving Javascript Performance

# What Are Some Techniques for Improving JavaScript Performance?

Let's review some of the most important techniques for improving JavaScript performance specifically.

You may find this surprising, but the first technique is using less JavaScript whenever possible.

If you're developing a simple static website, you may be able to do exactly the same without frameworks that rely on JavaScript.

You should also try to remove any unused JavaScript code and use simpler solutions, if possible.

For example, you may consider using built-in browser features instead of custom ones. These built-in browser features include form validation, the browser's built-in video player, and CSS animations instead of custom JavaScript animations.

Use as few animations as possible.

Reduce the amount of DOM manipulation on your JavaScript code, since this is computationally expensive.

Splitting your JavaScript code into modules that perform critical and non-critical tasks is also helpful. This way, you'll be able to preload the critical ones as soon as possible and defer the non-critical ones to render the page as fast as possible.

Pre-loading files does not guarantee that they will be available when you use them, but the download will start sooner, so the overall waiting time should be shorter.

Once your code is split into multiple files, you can minify them automatically during the build process to reduce their size and optimize their load time.

If an event listener is no longer necessary, you should remove it:

```
element.removeEventListener("mousemove", handleMouseMove);
```

In this example, we remove the event listener for the `mousemove` event, so the `handleMouseMove` function is no longer called when the event is triggered. If you keep the event listener, the program will continue performing calculations that are no longer necessary, affecting the overall performance. This effect will be even more noticeable if you have multiple active event listeners simultaneously.

And since we're on the topic of events, it's recommended to use event delegation whenever possible.

This means that you don't need to set the event listeners on individual child elements. You can set it directly on the parent and the event will bubble up until it finds a parent that can handle it.

Optimizing JavaScript is crucial for developing fast and responsive web applications. In a real-world project, you'll constantly analyze the performance of your website to find areas for improvement.

---

### Lecture 6.13: How To Improve The Perceived Performance Of Features

# How to Improve the Perceived Performance of Features?

As we know, perceived performance isn't just about how fast a site actually is — it's about how fast it feels to users. So, for example, if you have ever used a website that felt slow, even though it wasn't? That's perceived performance — how fast a site feels to the user.

Small tweaks can make a huge difference in the user experience. Let's explore some practical ways to improve perceived performance!

Spinners can make users feel like they're waiting longer than they actually are. Instead, try skeleton screens — gray placeholders that mimic real content and gradually load in:

```
<div class="skeleton"></div>
<script>
  setTimeout(() => {
    document.querySelector(".skeleton").innerHTML = "✅ Content Loaded!";
  }, 2000);
</script>
```

Users feel like the page is loading progressively, rather than waiting in the dark.

In addition to this, users shouldn't have to wait for everything to load before they can start interacting. Load important content first, then load the rest in the background. We looked at this previously with lazy loading:

```
<img src="placeholder.jpg" data-src="real-image.jpg" class="lazy">
<script>
  document.addEventListener("DOMContentLoaded", function () {
    const lazyImages = document.querySelectorAll("img.lazy");
    lazyImages.forEach(img => {
      img.src = img.dataset.src;
    });
  });
</script>
```

This makes the page feel responsive, even if not everything has loaded yet.

Now - what if your site could predict what the user will click next? With preloading, you can fetch the next page before they request it:

```
<link rel="preload" href="next-page.html" as="document">
```

This reduces perceived loading time to near zero when users navigate.

And finally, users don't like uncertainty. When they click a button, acknowledge their action instantly:

```
<button onclick="this.innerText='⏳ Processing...'; setTimeout(() => this.innerText='✅ Done!', 2000);">
  Click Me
</button>
```

This means that, even if there's a delay, the user feels like something is happening.

So, in conclusion, improving perceived performance isn't just about raw speed, it's about how speed feels to the user. Use skeleton screens, prioritize important content, preload smartly, and give instant feedback to make your site feel faster.

---

### Lecture 6.14: How Does Performance Impact Sustainability

# How Does Performance Impact Sustainability?

Improving web performance is crucial for delivering a fast and efficient user experience. But did you know that optimizing your website's performance doesn't just improve speed — it also helps the environment?

Every time a page loads, energy is consumed. And when sites are inefficient, they use more resources, leading to higher carbon emissions.

Let's break down how performance impacts sustainability and show you practical ways to optimize your code for a greener web.

The internet accounts for around 2% of global carbon emissions — that's the same as the airline industry! Every byte transferred requires electricity, from data centers to user devices. Larger files and inefficient scripts mean more power consumption. A high-performance website isn't just faster, it also reduces unnecessary processing and energy use.

Here's an example of inefficient JavaScript:

```
// Inefficient JavaScript
function fetchData() {
    for (let i = 0; i < 1000000; i++) {
        console.log("Processing...");
    }
    fetch("https://api.example.com/data")
        .then(response => response.json())
        .then(data => console.log(data));
}
fetchData();
```

This script runs excessive console logs, wasting CPU cycles and energy.

Now, let's optimize it:

```
// Optimized JavaScript
async function fetchDataOptimized() {
    const response = await fetch("https://api.example.com/data");
    const data = await response.json();
    console.log(data);
}
fetchDataOptimized();
```

By removing unnecessary loops and using `async`/`await`, we lower processing time and energy consumption.

Here are some practical optimization tips you can use in your future projects.

1. Minify Your Assets: Use tools like Terser or UglifyJS to shrink JavaScript and CSS files. Smaller files load faster and require less energy.
2. Optimize Images: Use next-gen formats like WebP instead of PNGs or JPEGs to reduce file size without quality loss.
3. Reduce Network Requests: Each request adds overhead. Combine CSS and JavaScript files and use lazy loading to reduce load times.
4. Use Efficient Algorithms: A poorly optimized loop can increase CPU usage. This is the same as writing inefficient JavaScript that we saw in the example previously.
5. Leverage Caching & CDNs: Caching prevents repeated downloads, and CDNs deliver content closer to users, reducing transmission energy.

And now, what if you want to measure your impact and just how green your site is?

Use tools like Google Lighthouse to analyze performance and estimate energy savings. Or, for a deeper sustainability check, try the Website Carbon Calculator — as it estimates your page's environmental impact.

In conclusion, by understanding and implementing these performance fundamentals, developers can create web applications that are not only faster and more responsive but also more sustainable.

---

### Web Performance

# Web Performance Review

Differences Between Real and Perceived Performance
--------------------------------------------------

* **Perceived Performance**: This is how users perceive the performance of a website. It's how they evaluate it in terms of responsiveness and reliability. This is a subjective measurement, so it's hard to quantify it, but it's very important, since the user experience determines the success or failure of a website.
* **Real Performance**: This is the objective and measurable performance of the website. It's measured using metrics like page load time, server response time, and rendering time. These measurements are influenced by multiple factors related to the network and to the code itself.

Techniques for Improving Perceived Performance
----------------------------------------------

* **Lazy Loading**: This technique reduces the initial load time as much as possible by loading non-essential resources in the background.
* **Minimize Font Delays**: If your website has custom fonts, you should also try to minimize font loading delays, since this may result in flickering or in showing the fallback font while the custom font is being loaded. A suggestion for this is using a fallback font that is similar to the custom font, so in case this happens, the change will be more subtle.
* **Use of Loading Indicators**: Showing a loading indicator for a long-running process as soon as the user clicks on an element can help the user feel connected and engaged with the process, making the wait time feel shorter.

Core Performance Concepts
-------------------------

* **Source order**: This refers to the way HTML elements are structured in the document. This determines what loads first and can significantly impact performance and accessibility.

Some best practices for source order include:

* Placing critical content such as headings, navigation or main text higher in the HTML structure.
* Deferring non-essential scripts such as ones for analytics, or third-party widgets, so they don't block rendering.
* Using progressive enhancement, to ensure the core experience works even before styles and scripts load. Progressive enhancement is a way of building websites and applications based on the idea that you should make your page work with HTML first.

Here is an example of good source order, using the best practices we just went through:

```
<h1>Welcome to FastSite!</h1>
<p>Critical information loads first.</p>
<script src="slow-script.js" defer></script>
```

* **Critical Rendering Path**: This is the sequence of steps the browser follows to convert code into pixels on the screen.
* **Latency**: This is the time it takes for a request to travel between the browser and the server. So in other words, high latency equals slow pages.

Some ways of reducing latency include:

* Using CDNs, or Content Delivery Networks, to serve files from closer locations.
* Enabling compression using things such as Gzip to reduce file sizes.
* Optimizing images and using lazy loading.

```
<img src="placeholder.jpg" data-src="real-image.jpg" loading="lazy">
```

Improving INP
-------------

* **Definition**: INP (Interaction to Next Paint) assesses a page's overall responsiveness by measuring the time from when a user interacts, like a click or key press, to the next time the browser updates the display. A lower INP indicates a more responsive page.

Here are some ways to improve INP:

* Reduce main thread work by breaking up long JavaScript tasks.
* Use `requestIdleCallback()` for non-critical scripts. This will queue a function to be called during a browser's idle periods.
* Defer or lazy-load heavy assets which were covered earlier.
* Optimize event handlers. If these handlers run too frequently or perform heavy operations, they can slow down the page and increase INP. The solution for this is debouncing. Debouncing ensures that the function only runs after the user stops typing for a short delay - so for example 300ms. This prevents unnecessary calculations and improves performance.

How Rendering Works in the Browser
----------------------------------

* **How Rendering works**: First the browser parses the HTML and builds the DOM. Next, the browser processes the CSS, constructing the CSS Object Model, or CSSOM. This is another tree structure that dictates how elements should be styled. Finally, the browser paints the pixels to the screen, rendering each element based on the calculated styles and layout. In complex pages, this might involve multiple layers that are composited together to form the final visual output.

How Performance Impacts Sustainability
--------------------------------------

* **Background Information**: The internet accounts for around 2% of global carbon emissions—that's the same as the airline industry! Every byte transferred requires electricity, from data centers to user devices. Larger files and inefficient scripts mean more power consumption. A high-performance website isn't just faster, it also reduces unnecessary processing and energy use.

Ways to Reduce Page Loading Times
---------------------------------

* **Optimize Media Assets**: Large images and videos are common culprits for slow load times. By optimizing these assets, you can significantly speed up your site. This includes things like compressing images, using modern formats like WebP and using lazy loading for assets.
* **Leverage Browser Caching**: Caching allows browsers to store parts of your website locally, reducing load times for returning visitors.
* **Minify and Compress Files**: Reducing the size of your files can lead to quicker downloads. This includes reducing the size of transmitted files and minifying CSS and JavaScript files.

Improving "time to usable"
--------------------------

* **Definition**: "time to usable" is the interval from when a user requests a page to when they can meaningfully interact with it. To improve "time to usable" you can lazy load your asset or minimize render-blocking resources.

Key Metrics for Measuring Performance
-------------------------------------

* **First Contentful Paint or FCP**: It measures how quickly the first piece of content—text or image—appears on the screen. A good FCP is regarded as a time below 1.8 seconds, and a poor FCP is above 3 seconds. You can check your FCP using Chrome DevTools and checking the performance tab.
* **Total Blocking Time**: This shows how long the main thread is blocked by heavy JavaScript tasks. If Total Blocking Time (TBT) is high, users experience sluggish interactions. To improve TBT, break up long tasks and defer non-essential scripts.
* **Bounce Rate**: This is the percentage of visitors who leave without interacting. If your site has high bounce rates it might be because your page is too slow.
* **Unique Users**: This metric tracks how many individual visitors come to your site. To view the Bounce Rate and Unique Users, you can use Google Analytics. It will allow you to monitor these metrics and improve engagement.

Common Performance Measurement Tools
------------------------------------

* **Chrome DevTools**: Chrome DevTools is a built-in tool inside Google Chrome that lets you analyze and debug performance in real-time. DevTools will show loading times, CPU usage, and render delays. It's especially useful for measuring First Contentful Paint, or FCP, is how fast a user sees the first visible content. If your website feels slow, DevTools will help you spot the bottlenecks.
* **Lighthouse**: This is an automated tool that checks performance, SEO, and accessibility.
* **WebPageTest**: This tool lets you test how your site loads from different locations and devices. This tool gives you a detailed breakdown of your site's Speed Index, Total Blocking Time, and other key performance metrics. If you want to know how real users experience your site globally, WebPageTest is the tool for that.
* **PageSpeed Insights**: This tool analyzes your website and suggests quick improvements for both mobile and desktop. It will tell you what's slowing your site down and give specific recommendations like optimizing images, removing render-blocking scripts, and reducing server response times. PageSpeed Insights is a fast and easy way to check how Google sees your site's performance.
* **Real User Monitoring**: RUM tools track actual user behavior, showing how real visitors experience your site. Popular RUM tools include Google Analytics, which tracks page load times and bounce rates, and New Relic or Datadog, which monitor real-time performance issues. If you want data from actual users, RUM tools are essential.

Working with Performance Web APIs
---------------------------------

* **Definition**: Performance Web APIs let developers track how efficiently a webpage loads and responds directly in the code. These APIs allow you to measure page load times, track rendering and interaction delays and analyze JavaScript execution time.
* **`performance.now()`**: This API gives you high-precision timestamps (in milliseconds) to measure how long different parts of your site take to load.

```
const start = performance.now();  
// Run some code here  
const end = performance.now();  

console.log(`Execution time: ${end - start}ms`);
```

* **Performance Timing API**: This API gives you a breakdown of every stage of page loading, from DNS lookup to `DOMContentLoaded`.

```
const timing = performance.timing;  

const pageLoadTime = timing.loadEventEnd - timing.navigationStart;  
console.log(`Page load time: ${pageLoadTime}ms`);
```

* **`PerformanceObserver`**: This API listens for performance events such as layout shifts, long tasks, and user interactions.

```
const observer = new PerformanceObserver((list) => {  
  list.getEntries().forEach((entry) => {  
    console.log(`Long task detected: ${entry.duration}ms`);  
  });  
});  

observer.observe({ type: "longtask", buffered: true });
```

Techniques for Improving CSS Performance
----------------------------------------

* **CSS Animations**: Animating certain CSS properties, such as dimensions, position, and layout, triggers a process called "reflow", during which the browser recalculates the position and geometry of certain elements on the page. This requires a repaint, which is computationally expensive. Therefore, it's recommended to reduce the number of CSS animations as much as possible or at least give the user an option to toggle them on or off.

Techniques for Improving JavaScript Performance
-----------------------------------------------

* **Code Splitting**: Splitting your JavaScript code into modules that perform critical and non-critical tasks is also helpful. This way, you'll be able to preload the critical ones as soon as possible and defer the non-critical ones to render the page as fast as possible.
* **DOM Manipulation**: Remember that DOM Manipulation refers to the process of dynamically changing the content of a page with JavaScript by interacting with the Document Object Model (DOM). Manipulating the DOM is computationally expensive. By reducing the amount of DOM manipulation in your JavaScript code will improve performance.

---

## Module 7: Software Testing, Automation & Lifecycle

### Lecture 7.1: What Is The Software Development Life Cycle And How Does It Relate To Testing

# What Is the Software Development Life Cycle, and How Does It Relate to Testing?

When working on software teams, it is important to have a process for designing and building out new products and services. The Software Development Life Cycle is commonly used by software teams to build and deploy applications.

In this lesson, we will break down the different stages of the Software Development Life Cycle (SDLC) and the role that testing plays in it.

Here are the standard stages used in the Software Development Life Cycle:

* Planning stage
* Design stage
* Implementation stage
* Testing stage
* Deployment stage and
* Maintenance stage

Let's take a closer look at all of those stages in more detail.

In the planning stage, the development team collects requirements for the proposed work from the stakeholders. A stakeholder is someone with a vested interest in the success of the product or service. Examples of stakeholders could be investors, owners, or even other employees. The planning phase also includes estimating costs for the work and creating a schedule for when the work will be completed.

The next stage is the Design stage. In this phase, the software team breaks down the requirements and decide on the best approaches for solutions. This includes deciding on which external tools can be used to help things along and what internal tooling needs to be built to get the job done.

After the design stage, you have the implementation stage. This involves the software team breaking down the requirements into manageable tasks that they divide up amongst themselves and build out.

Once the implementation stage is complete, the software team moves into the testing stage. This involves manual and automated testing for the new work. Sometimes the team tests out the application throughout the entire development stage to catch and fix any issues that come up.

The next stage is the deployment stage. This is where the team deploys the new changes to a build or testing environment. This allows the team to test out the application some more and fix any issues before the changes go to production. The production application is the app that end users will use.

The last stage is the maintenance stage. This involves fixing any issues that arise from customers in the production application. This also involves monitoring the system for any possible improvements on the software.

Finally, there are different models of the Software Development Life Cycle used in the industry, such as Waterfall and Agile. The Waterfall model is where each phase of the life cycle needs to be completed before the next phase can begin. In contrast, the Agile model focuses on iterative development by breaking down work into sprints so teams can quickly make changes and deliver work over time.

By going through the Software Development Life Cycle, the development team and stakeholders can be on the same page when it comes to requirements, cost estimates, and schedules. This makes for more efficient collaboration and communication across the board.

---

### Lecture 7.2: What Is The Overall Purpose Of Testing Your Applications

# What Is the Overall Purpose of Testing Your Applications?

Up until this point, you have been building tons of small projects in languages like HTML, CSS, JavaScript, and more. But how do you know if your projects are working correctly?

One option is to do what is called manual testing. This is where a tester will go through each part of the application and test out all of the different features to make sure it works correctly. If any bugs are uncovered in the testing process, the tester will report those bugs back to the software team so they can be fixed.

While it is important to manually test out your applications, often times it will not be enough. Real-world applications involve many components and services and can often be complex in nature. So only relying on manual testing will result in many bugs lying beneath the surface that can hurt the usability and maintainability of an application.

This is where automated testing comes in. You can write separate test code to check whether your application behaves as expected, without needing to manually click through it. Both manual and automated tests can be grouped into different types, depending on what they are testing.

Over the next few lessons, we are going to cover the different types of testing used in the industry like unit testing, end-to-end testing, functional testing and more.

Writing tests for your applications will help ensure that your code is doing what it is supposed to be doing. It is important that you start to familiarize yourself with the basics of testing because it will be something that you will need in a developer job.

---

### Lecture 7.3: What Is Unit Testing

# What Is Unit Testing?

As you design your applications, you will often have a series of small functions responsible for one thing. This is known as the "single responsibility principle." When you have a series of small functions, it is best to test these functions to ensure that everything works as expected. In this lesson, we will take a look at how to create a unit test using the popular Jest testing framework.

In this example, we are going to create a function that is responsible for returning a newly formatted string:

```
export function getFormattedWord(str) {
  if (!str) return '';
  return str.charAt(0).toUpperCase() + str.slice(1);
}
```

This `getFormattedWord` function has a parameter called `str` and will first check if the `str` is empty. If so, then an empty string is returned. Otherwise, a new string is returned where the first letter is capitalized. We are exporting this function so we can use it in a test file.

In a separate `getFormattedWord.test.js` file, we can write some tests to verify that the function is doing what it is supposed to be doing.

At the top of the `getFormattedWord.test.js` file, we need to first import the function like this:

```
import { getFormattedWord } from "./getFormattedWord.js";
```

Then we need to install the Jest package by using `npm i jest`. Then we can add a test to check that a word made up of lowercase characters, `hello`, is properly formatted to `Hello`, which starts with a capital `H`:

```
test('capitalizes the first letter of a word', () => {
  expect(getFormattedWord('hello')).toBe('Hello');
});
```

The `expect` function is used to test a value. It's combined with a matcher, which is a function that checks whether the value behaves as expected. In this case the matcher is `toBe()`. Jest has a variety of matchers to help you test for truthiness, strings, numbers, and more.

One way to run your tests is by adding an npm script to your `package.json` file. Here's an example script for the Jest framework:

```
"scripts": {
  "test": "jest"
},
```

Then just run `npm run test` in your terminal to run your tests. If your tests pass, you should see something in the terminal like this:

```
PASS ./getFormattedWord.test.js
  ✓ capitalizes the first letter of a word (1 ms)

Test Suites: 1 passed, 1 total
Tests:       1 passed, 1 total
Snapshots:   0 total
Time:        0.103 s, estimated 1 s
Ran all test suites.
```

To see what a failing test looks like, we can intentionally break the test by updating the function to the following:

```
export function getFormattedWord(str) {
  if (!str) return '';
  return "This is incorrect";
}
```

Now when you run the `npm run test` command, there will be an error message because the test was expecting a different result:

```
FAIL ./getFormattedWord.test.js
  ✕ capitalizes the first letter of a word (1 ms)

  ● capitalizes the first letter of a word

  expect(received).toBe(expected) // Object.is equality

  Expected: "Hello"
  Received: "This is incorrect"

    2 |
    3 | test('capitalizes the first letter of a word', () => {
    4 |   expect(getFormattedWord('hello')).toBe('Hello');
                                            ^
    5 | });
    6 |

    at Object.toBe (getFormattedWord.test.js:4:37)

Test Suites: 1 failed, 1 total
Tests:       1 failed, 1 total
Snapshots:   0 total
Time:        0.121 s, estimated 1 s
Ran all test suites.
```

Now we can update our function back to the original here:

```
export function getFormattedWord(str) {
  if (!str) return '';
  return str.charAt(0).toUpperCase() + str.slice(1);
}
```

Add another test to check for cases where no argument is provided to `getFormattedWord`:

```
test("returns an empty string when no argument is provided", () => {
  expect(getFormattedWord()).toBe("");
});
```

There are other tests you can add to make things more robust, but these first couple of tests are a good introduction to unit testing.

When it comes to testing JavaScript applications some common testing frameworks include Jest, Mocha, and Vitest.

Unit testing is important because it will help you catch more bugs in your programs, and ensure that everything works as expected. It also can serve as a form of documentation for your application because it is meant to represent the expected behavior for your code.

---

### Lecture 7.4: How Do Assertions Work In Unit Testing

# How Do Assertions Work in Unit Testing?

You were first introduced to assertions and unit testing in a previous lesson. But as a review, unit testing is when you check the output of individual functions or components independently, in contrast with testing the final output of the entire program. Assertions are used to test that the code is behaving as expected.

In this lesson, we are going to take a closer look at assertions in unit tests and explore some best practices.

A commonly used assertion library is Chai. This is the same library used inside of the freeCodeCamp codebase. Whenever you go through a workshop or lab, there is an automated test suite that runs against your code to ensure that your code is behaving the way it is supposed to.

Let's take a look at a few examples that are from the Full-Stack Developer Curriculum.

In Build a Calculator workshop, Step 1 is testing for a function called `addTwoAndSeven`:

```
assert.isFunction(addTwoAndSeven);
```

That assertion checks that the provided code contains a function named `addTwoAndSeven`. If the user creates an array, string, or anything else that's not a function and assigns it to `addTwoAndSeven`, then the test will fail.

Let's take a look at another assertion from later in the workshop:

```
assert.equal(addThreeAndFour(), 7);
```

This assertion checks that the return value from the `addThreeAndFour` function is equal to the number `7`. If the return value does not equal `7`, then the test will fail.

There are many more asserts built into Chai, like ones that check if a value is a boolean, if an object has a certain property name, or if a value is `null`. Other common JavaScript assertion libraries are should.js and expect.js.

Regardless of which assertion library you are working with, there are a few best practices to be aware of. The first is to write clear assert messages. Clear and meaningful assert messages should describe the intent behind it. Otherwise, it will be difficult to locate which tests are failing.

Another best practice is to write descriptive failure messages. A descriptive failure message should state which condition is true. This will help you figure out why a particular assert is failing.

As you continue learning to code, it's important to familiarize yourself with testing and start writing tests for your personal projects. Doing this will go a long way in helping you prepare for your first developer job.

---

### Lecture 7.5: What Is Functional Testing And How Does It Differ From Unit Testing

# What Is Functional Testing, and How Does It Differ from Unit Testing?

In prior lessons, you learned how to test small units of code through unit testing. Well, unit testing is part of functional testing. Functional testing checks if the features and functions of the application work as expected.

In this lesson, we will take a look at the differences between functional and non-functional testing.

The goal of functional testing is to test the system as a whole against multiple scenarios to ensure that the system works as expected. An example of functional testing would be smoke testing. Smoke testing is where you perform a preliminary check on the system for basic or critical issues before more extensive testing is done.

In contrast, non-functional testing focuses on things like performance and reliability.

A real test scenario for functional testing would be a user login. A user should be able to log in to the application with their username and password. If successful, they should be able to access their account information. If there is an issue, then that error needs to be handled properly. When you are writing tests, you need to account for all types of success and failure scenarios.

An example of non-functional testing would be to test the performance of your application under different network conditions. In a future lesson, you will learn more about performance testing.

The reasons why functional testing is so important is because you want to identify bugs early on in your application. You also want to make sure that your application meets the requirements that were laid out at the beginning of the planning phase. Lastly, you want to ensure that your users have a good user experience. Users should not struggle to use your application or be blocked by broken features and system failures.

---

### Lecture 7.6: What Is End To End Testing

# What Is End-to-End Testing?

End-to-end testing, or E2E for short, tests real-world scenarios from the user's perspective. Examples of E2E testing scenarios include testing the registration and login process or testing the checkout for an e-commerce site.

To better understand how end-to-end testing works, let's take a look at a real-world example from the freeCodeCamp codebase. This example uses Playwright, a popular end-to-end testing framework developed by Microsoft.

Inside the freeCodeCamp codebase, there is a directory called `e2e` which holds tests for donations, certifications, exams and more. Inside the directory, there is a `donate-page-donor.spec.ts` file which has tests for the authenticated donor supporter page.

The first step is to navigate to the donation page as a demo user who is already a supporter:

```
test.beforeEach(async ({ page }) => {
  execSync("node ./tools/scripts/seed/seed-demo-user --set-true isDonating");
  await page.goto("/donate");
});
```

Since there are multiple tests in this file, the `beforeEach` hook will run before each of the tests.

Once the user is on the donation page, they will see a thank you message with suggestions on how to support freeCodeCamp further. Here are just a few of the tests to check for some of the text found on the donation page:

```
test("should render the donate page correctly", async ({ page }) => {
  await expect(
    page.getByText("Thank you for your continued support")
  ).toBeVisible();

  await expect(
    page.getByText(
      "Your contributions are crucial in creating resources that empower millions of people to learn new skills and support their families."
    )
  ).toBeVisible();

  ...
});
```

There are also tests to check that the donor has a supporter link in the menu bar, as well as a special stylized border around their avatar to indicate they are a supporter:

```
test("The menu should have a supporters link", async ({ page }) => {
  const menuButton = page.getByTestId("header-menu-button");
  const menu = page.getByTestId("header-menu");

  await expect(menuButton).toBeVisible();
  await menuButton.click();

  await expect(menu).toBeVisible();

  await expect(page.getByRole("link", { name: "Supporters" })).toBeVisible();
});

test("The Avatar should have a special border for donors", async ({ page }) => {
  const container = page.locator(".avatar-container");
  await expect(container).toHaveClass("avatar-container gold-border");
});
```

By having these types of detailed tests, you can increase the test coverage for your application beyond just unit tests. End-to-end tests also help ensure that your application behaves correctly, and is predictable for users. Examples of other end-to-end testing tools include Cypress, Selenium, and Puppeteer.

While end-to-end testing is important, it is expensive because it is time-consuming to set up, design, and maintain. E2E tests are great for critical user flows, while unit tests are great for testing small units in the application.

---

### Lecture 7.7: What Are The Differences Between Mocking Faking And Stubbing

# What Are the Differences Between Mocking, Faking, and Stubbing?

Mocking is the process of replacing real data with false data that simulates the behavior of real components. This allows testers and developers to test for specific components in the application without having to rely on external dependencies.

A common use case for mocking data would be when dealing with API calls. Imagine you have a fetch call like this in your application:

```
export const postService = {
  async getPosts() {
    const response = await fetch("https://api.example.com/posts");
    return response.json();
  },
};
```

If you need to test the `postService` function, you could mock the API response instead of making continuous API calls to fetch the data. Fetching from an API takes time and depends on external factors like network availability and server responses. Mocking the API response removes those external factors and allows testers to work with a predictable, controlled data set.

Here is an example mock API response:

```
[
  {
    "id": 1,
    "title": "Understanding Async/Await in JavaScript",
    "content": "Async/Await makes asynchronous code look and behave like synchronous code...",
    "author": "Jane Doe",
    "created_at": "2025-04-10T14:32:00Z"
  },
  {
    "id": 2,
    "title": "10 Tips for Writing Clean Code",
    "content": "Clean code is not just about code formatting. It involves naming, architecture...",
    "author": "John Smith",
    "created_at": "2025-04-08T09:21:00Z"
  },
  {
    "id": 3,
    "title": "Exploring React 19 Features",
    "content": "React 19 comes with exciting features like new hooks and better performance...",
    "author": "Alex Lee",
    "created_at": "2025-04-07T18:47:00Z"
  }
]
```

Now that we understand what mocking is, let's compare it with stubbing. Stubs are objects that return pre-defined responses or dummy data for an expected behavior in an application. For example, you can stub the behavior for a database connection in your tests without having to rely on an actual database connection.

Here is an example of a stub in Jest:

```
import { postService } from "./postService";
import { db } from "./db";

jest.mock("./db", () => ({
  db: {
    fetchPosts: jest.fn(),
  },
}));

test("should return stubbed posts", async () => {
  const fakePosts = [
    { id: 1, title: "Stubbed Post", content: "This is a stubbed post." },
  ];

  db.fetchPosts.mockResolvedValue(fakePosts);

  const posts = await postService.getPosts();

  expect(posts).toEqual(fakePosts);
});
```

`db.fetchPosts.mockResolvedValue(fakePosts);` is the stub in this example.

The last component to discuss are fakes. Fakes are simplified versions of real components without the complexity or side effects of the real thing. For example, you can fake a database by storing the data in memory instead of interacting with the real database. This will allow you to mimic database operations in memory, which will be much faster than dealing with the real database. Another common example would be to use fakes when working with file systems. You can create a fake file system in place of the real one when it comes to testing.

As you continue to build out more complex software applications, consider using mocks, stubs, or fakes where appropriate in your testing.

---

### Lecture 7.8: What Are Bdd And Tdd

# What Are BDD and TDD?

There are two types of testing approaches that you should be aware of in software development. Those approaches are TDD (Test-Driven Development) and BDD (Behavior-Driven Development).

Let's first take a look at TDD. Test-Driven Development is a methodology that emphasizes writing tests first before building out the features for an application.

Here is the typical process for TDD:

1. Write a test
2. Ensure that it fails
3. Write the code for that test
4. Ensure that the test passes this time
5. Make any necessary refactors to the code

Repeat steps 1-5.

Writing tests before building out features provides real-time feedback to developers during the development process. It also helps with catching bugs earlier on in the development stage.

While some software teams will choose to follow the TDD approach, TDD is a polarizing topic in the industry. You will find tons of articles and videos out there both advocating for or bashing TDD. Regardless of how you feel about this approach, it is important to be aware of it because you might come across it in real-world scenarios.

The second testing approach we will take a look at is Behavior-Driven Development (BDD). Behavior-Driven Development is the approach of aligning a series of tests with business goals. These tests should be written in a language that can be understood by both technical and non-technical individuals.

When testing for specific behaviors in a software application, BDD commonly uses the Gherkin language, which is used in businesses to describe behaviors and scenarios. The Gherkin language uses Given, When, and Then statements when describing scenarios.

Here is an example:

**Scenario:** Creating a New Blog Post

**Given** the user is logged into their account and is on the "Create New Post" page,

**When** the user enters a title and content for the post and clicks the "Publish" button,

**Then** the blog post should be saved and displayed on the homepage with the correct title, content, and timestamp.

You first want to define a scenario. Example scenarios include when a user logs into an application or places an order on a website. In this example, the scenario is for a user creating a new blog post on a site.

After the scenario is defined, you should start with a Given statement. This provides context for where the user is starting before performing an action. The When statement is used to represent the action taken by the user.

Finally, the Then statement is used to represent the desired outcome from the previous action taken by the user. Once you define all of your scenarios, you can write tests for each scenario.

Examples of BDD testing frameworks include Cucumber, JBehave, and SpecFlow.

---

### Lecture 7.9: What Is Regression Testing

# What Is Regression Testing?

As an application continues to grow, it is not uncommon to have situations where new changes unintentionally break existing functionality. This is known as a regression.

To help catch these issues before they happen, you can use regression testing. Regression testing is when you re-run functional tests against parts of your application to ensure that everything still works as expected. If you've implemented bug fixes, enhancements, or even have updates to your configuration, then it's a good idea to perform regression testing.

There are different tools that you can use to perform regression testing. They include Puppeteer, Playwright, Selenium, and Cypress.

There are also a few testing techniques to be aware of when it comes to regression testing. The first is called unit regression testing. This is where you have a list of items that need to be tested each time major changes or fixes are implemented into the app.

Another testing technique is called partial regression testing. This involves targeted approaches to ensure that new changes have not broken specific aspects of the application.

Finally, there's complete regression testing. This is the most time-consuming and detailed option, which looks at all the functionalities affected by the recent changes in the codebase and runs tests against them.

It's important to note that retesting and regression testing are different. Retesting is used to check for known issues and ensure that they have been resolved, whereas regression testing searches for unknown issues that might have occurred through recent changes in the codebase.

---

### Lecture 7.10: What Is Compatibility Testing

# What Is Compatibility Testing?

When you build out web applications at scale, you will need to think beyond your personal computing environment. How will these applications work on a variety of devices, operating systems, and browsers? Well, this is where compatibility testing comes in.

The goal of compatibility testing is to see how well your software works in a variety of different computing environments. This provides the team with the ability to catch bugs before they reach production and will help contribute to a smoother product launch.

Different types of compatibility testing include backwards and forwards compatibility, hardware testing, operating systems, networks, browsers, and mobile devices.

Let's take a look at each of the types in more detail by starting with backwards and forwards compatibility. Backwards compatibility refers to when current software is compatible with earlier versions. Forwards compatibility is when software and systems will work with future versions of itself.

The next type of testing is for hardware. Hardware compatibility testing focuses on the software's ability to work properly in different hardware configurations. This includes different types of processors, memory, storage, and graphics cards.

Another type of compatibility testing is for operating systems. You don't want to design software that works smoothly on Mac devices but has bugs on Windows or vice versa. You also need to consider Linux distributions like Ubuntu and Fedora.

The next type of testing is network compatibility testing. You will have users working with different network speeds, protocols, security settings, and more. Therefore, software teams will need to be mindful of all of those different conditions when testing.

Then, there's browser compatibility testing. There are a few popular browsers in the market like Google Chrome, Safari, Firefox, and more. Since all browsers work slightly differently, it's important to test your web application thoroughly and make sure your web applications work consistently across many browsers.

The last type of testing is mobile testing. There was a time in web development when most developers didn't think about testing for mobile devices. This was because, in the early 2000s, mobile devices weren't nearly as powerful or widely used as they are today. But now, tens of millions of people visit websites on phones and tablets. So, it is important to ensure that your software applications work on a variety of Android and iOS devices.

Those are just a few types of testing that you will need to consider when building out your applications. While this might seem like a lot of extra work, it is important to perform compatibility tests because you do want to ensure that your applications work in a variety of computing environments.

---

### Lecture 7.11: What Is Usability Testing And What Does The Process Look Like

# What Is Usability Testing, and What Does the Process Look Like?

Usability testing is when you have real users interacting with the application to discover if there are any design, user experience, or functionality issues in the app. This type of testing is important because this feedback will help ensure that the application meets the needs of the users.

The four common types of usability testing are explorative, comparative, assessment and validation testing.

Let's first start with explorative usability testing. This type of testing involves users interacting with the different features of the application to better understand how they work. The goal here is to identify any potential issues in the application so they can be addressed early on and resolved.

The second type of usability testing is comparative testing. This is where you compare your application's user experience with similar applications in the marketplace. The goal is to see where your application falls short compared to the competition so those areas can be improved on.

The third type of usability testing is assessment testing. This is where you study how intuitive the application is to use and if there are any major blockers for users. This type of testing will result in reduced costs and headaches once the application is live to thousands or even millions of users down the line.

The last type of usability testing is validation testing. This is where you identify any major issues that will prevent the user from using the application effectively. This type of testing usually happens after the initial development stage and just before the final release of the application.

There are many tools out there to assist with usability testing, but here are a few popular ones to be aware of:

* Loop11
* Maze
* Userbrain
* UserTesting and
* UXTweak

It is important to note that functional testing is not the same as usability testing. Functional testing focuses on the functionality of the application while usability testing focuses on the intuitiveness of the application by users.

---

### Lecture 7.12: What Is Performance Testing

# What Is Performance Testing?

If a software application is slow to respond or unstable, that will lead to a poor user experience. Performance testing is what you do when you test an application's speed, responsiveness, scalability, and stability under different workloads. The goal is to resolve any type of performance bottleneck before it reaches your users.

In this lesson, we will go through a few types of performance testing.

The first type is load testing. A load in this context refers to the amount of work or demand put on a system. Load testing determines how a system behaves during normal and peak load times. The goal is to analyze metrics like response times and resource usage and determine if the current software build is ready or not.

Another type of testing is stress testing. This is where you test your application in extreme loads and see how well your system responds to the higher load. The goal here is to identify any bottlenecks and vulnerabilities by testing the system beyond its limits.

The next type of performance testing is soak testing, also known as endurance testing. This is a type of load testing where you test the system with a higher load for an extended period of time. The goal here is to determine any types of memory leaks and performance degradation.

Another type of testing is spike testing. This is where you dramatically increase and decrease the loads and analyze the system's reactions to the changes. The goal here is to see if your system will fail with these dramatic changes in the load.

Finally, there's breakpoint testing, also known as capacity testing. This is where the load will slowly increment over time to the point where the system starts to fail or degrade. The goal here is to better understand the system's limits and capacities.

These are just a few types of performance testing you can do on your applications. Since performance plays a vital role in software development, it is important that you perform these types of tests to ensure that your application doesn't have any major issues and provides a smooth experience for users.

---

### Lecture 7.13: What Is Security Testing

# What Is Security Testing?

The web is a powerful place filled with a wealth of information and activities. But it can also be a dangerous place if you are not careful. There are many hackers and cyber criminals out there looking for new ways to breach websites and compromise data.

You've probably heard of a few high-profile data breaches that affected billion-dollar companies like Meta and Microsoft. When it comes to working on web applications, you will need to do thorough security testing to help identity vulnerabilities and weaknesses.

Here are a few principles to be aware of when it comes to performing security audits and testing:

* Confidentiality: This protects against the release of sensitive information to other recipients that aren't the intended recipient.
* Integrity: This involves preventing malicious users from modifying user information.
* Authentication: This involves verifying the user's identity to ensure that they are allowed to use that system.
* Authorization: This is the process of determining what actions authenticated users are allowed to perform or which parts of the system they are permitted to access.
* Availability: This ensures that information and services are available to authorized users when they need it.
* Non-repudiation: This ensures that both the sender and recipient have proof of delivery and verification of the sender's identity. It protects against the sender denying having sent the information.

Now that we understand the reasoning behind security testing, let's take a look at a few common security threats:

* Cross-site Scripting (XSS): You learned about this in an earlier lesson. But as a refresher, XSS attacks happen when an attacker injects malicious scripts into a web page that is viewed by other users. These scripts can then execute in the context of the victim's browser, potentially stealing cookies and session data or performing other malicious actions without the user's knowledge or consent.
* SQL Injection: SQL is a language for managing and storing information in a relational database. SQL injection allows malicious users to inject malicious code into a database. You will learn more SQL, relational databases, and SQL injection in a future module.
* Denial-of-Service (DoS) attack: This is when malicious users flood a website with a high number of requests or traffic, causing the server to slow down and possibly crash, making the site unavailable to users.

There are many more types of security threats, but there are many tools you can use to help protect your web applications and make them more secure. Here are the broad categories that security testing tools fall into:

* Static application security testing: These tools are used to evaluate the source code for an application to identify security vulnerabilities.
* Dynamic application security testing (DAST): These tools interface with the application's front-end to uncover potential security weaknesses. Unlike static application security testing, DAST tools do not have access to the source code.

Another type of security testing is penetration testing (or pentest for short). This involves creating simulated cyberattacks on the application to identify any vulnerabilities in the system. Mid to large-sized companies might have a team of dedicated cybersecurity professionals that perform pentests on a regular basis as part of their regular security audits.

The world of cybersecurity is very vast and detailed. But every developer should understand a few common threats against web applications and ways to guard against them.

---

### Lecture 7.14: What Is Ab Testing

# What Is A/B Testing?

Most of you have a select group of websites that you visit every day. This might include sites like X, Discord, or freeCodeCamp. But have you ever wondered why you often see small changes to the design of your most frequently visited pages? Well, this doesn't happen by accident.

Companies spend a lot of time analyzing analytics and studying user behavior. They do this to identify pain points in the user experience for their site or application. These companies then use that data to come up with solutions to create a smoother user experience.

One of the techniques companies employ is called A/B testing. This type of testing involves comparing two versions of a page or application and studying which version performs better. Sometimes, this type of testing is known as bucket or split testing.

Let's take a look at an example so you can better understand the concept. Imagine you have a landing page with some introductory text and a CTA (call to action) button. Remember that a CTA button is used to encourage users to perform a specific action, like donate or log in.

As you go through the site analytics, you realize that the click-through rate for the CTA is low. So you try redesigning that button so it's more prominent on the page. You increase the size of the button and change the button color from blue to green. To actually see if those changes made a difference, you can use A/B testing.

You can randomly divide your users into two groups. Group A is the control group, which sees the original version of the page with the smaller blue button, while group B is the experimental group, which see the new version of the page with the larger green button. If the new version of the page results in a higher click-through rate, then you can confidently replace the old button styling with the new one.

Examples of tools to use for A/B testing include GrowthBook and LaunchDarkly.

There are many common use cases for A/B testing like testing ads, email campaigns, or new product features. A/B testing allows you to make more data-driven decisions and continually improve the user experience.

---

### Lecture 7.15: What Is Alpha And Beta Testing

# What Is Alpha and Beta Testing?

Once the initial development and software testing are complete, it is important to have the application tested by testers and real users. This is where alpha and beta testing come in.

Alpha testing is done by a select group of testers who go through the application to ensure there are no bugs before it is released into the marketplace. This is part of acceptance testing, which ensures that the software application meets the needs of users before its release.

Alpha testing also utilizes both white and black box testing techniques. Black box testing only focuses on the expected behavior of the application, whereas white box testing involves the tester knowing the internal components and performing tests on that.

After the alpha testing phase, there is the beta testing phase. This is where the application is made available to real users. Actual users can interact with the application and provide feedback. This is a form of user acceptance testing which ensures that the application meets the business requirements as well as user needs.

While both stages of testing can be time-consuming, it is important to perform alpha and beta tests on your applications. This will help ensure that the application is truly ready for the marketplace and meets the needs of its users.

---

### Testing

# Testing Review

Manual and Automated Testing
----------------------------

* **Manual Testing**: In manual testing, a tester will manually go through each part of the application and test out different features to make sure it works correctly. If any bugs are uncovered in the testing process, the tester will report those bugs back to the software team so they can be fixed.
* **Automated Testing**: In automated testing, you can automate your tests by writing a separate program that checks whether your application behaves as expected.

Unit Testing
------------

* **Unit Testing**: In unit testing, you test each function to ensure that everything is working as expected. Unit tests can also serve as a form of documentation for your application because they are meant to represent the expected behavior for your code.
* **Single Responsibility Principle**: The single responsibility principle recommends keeping each function small and responsible for one thing.
* **Common JavaScript Testing Frameworks**: Some common testing frameworks include Jest, Mocha, and Vitest. Jest is a popular testing framework for unit tests.

Here is an example of unit tests using Jest.

First, you can create a function that is responsible for returning a newly formatted string:

```
export function getFormattedWord(str) {
  if (!str) return '';
  return str.charAt(0).toUpperCase() + str.slice(1);
}
```

In a separate `getFormattedWord.test.js` file, you can write some tests to verify that the function is working as expected. The `getFormattedWord.test.js` file will look like this:

```
import { getFormattedWord } from "./getFormattedWord.js";
import { test, expect } from "jest";

test('capitalizes the first letter of a word', () => {
  expect(getFormattedWord('hello')).toBe('Hello');
});
```

* **`expect` Function**: The `expect` function is used to test a value.
* **Matcher**: Matcher is a function that checks whether the value behaves as expected. In the above example, the matcher is `toBe()`. Jest has a variety of matchers.

To use Jest, you first need to install the `jest` package by using `npm i jest`. You will also need to add a script to your `package.json` file like this:

```
"scripts": {
  "test": "jest"
},
```

Then, you can run the command `npm run test` to run your tests.

Software Development Lifecycle
------------------------------

* **Different Stages of Software Development Lifecycle**:

  + **Planning Stage**: The development team collects requirements for the proposed work from the stakeholders.
  + **Design Stage**: The software team breaks down the requirements and decides on the best approaches for solutions.
  + **Implementation Stage**: The software team breaks down the requirements into manageable tasks and implements them.
  + **Testing Stage**: This involves manual and automated testing for the new work. Sometimes, the team tests out the application throughout the entire development stage to catch and fix any issues that come up.
  + **Deployment Stage**: The team deploys the new changes to a build or testing environment.
  + **Maintenance Stage**: This involves fixing any issues that arise from customers in the production application.
* **Different Models of the Software Development Lifecycle**:

  + **Waterfall Model**: The Waterfall model is where each phase of the lifecycle needs to be completed before the next phase can begin.
  + **Agile Model**: The Agile model focuses on iterative development by breaking down work into sprints.

BDD and TDD
-----------

* **TDD**: Test-driven development is a methodology that emphasizes writing tests first. Writing tests before building out features provides real-time feedback to developers during the development process.
* **BDD**: Behavior-driven development is the approach of aligning a series of tests with business goals. The test scenarios in BDD should be written in a language that can be understood by both technical and non-technical individuals. An example of such syntax is Gherkin.
* **BDD Testing Frameworks**: Examples of BDD testing frameworks include Cucumber, JBehave, and SpecFlow.

Assertions in Unit Testing
--------------------------

* **Assertion**: Assertions are used to test that the code is behaving as expected.
* **Assertion Libraries**: Chai is a commonly used assertion library. Other common JavaScript assertion libraries are `should.js` and `expect.js`.

Here is an example of an assertion using Chai that checks that the return value from the `addThreeAndFour` function is equal to the number 7:

```
assert.equal(addThreeAndFour(), 7);
```

* **Best Practices**: Regardless of which assertion library you use, you should write clear assert and failure messages that will help you understand which tests are failing and why.

Mocking, Faking, and Stubbing
-----------------------------

* **Mocking**: Mocking is the process of replacing real data with false data that simulates the behavior of real components. For example, you could mock the API response in testing instead of making continuous API calls to fetch the data.
* **Stubbing**: Stubs are objects that return pre-defined responses or dummy data for an expected behavior in an application. For example, you can stub the behavior for a database connection in your tests without having to rely on an actual database connection.
* **Faking**: Fakes are simplified versions of real components without the complexity or side effects. For example, you can fake a database by storing the data in memory instead of interacting with the real database. This will allow you to mimic database operations in memory, which will be much faster than dealing with the real database.

Functional Testing
------------------

* **Functional Testing**: Functional testing checks if the features and functions of the application work as expected. The goal of functional testing is to test the system as a whole against multiple scenarios.
* **Non-Functional Testing**: Non-functional testing focuses on things like performance and reliability.
* **Smoke testing**: Smoke testing is a preliminary check on the system for basic or critical issues before beginning more extensive testing.

End-to-End Testing
------------------

* **End-to-End Testing**: End-to-end testing, or E2E, tests real-world scenarios from the user's perspective. End-to-end tests help ensure that your application behaves correctly and is predictable for users. However, it is time-consuming to set up, design, and maintain.
* **End-to-End Testing Frameworks**: Playwright is a popular end-to-end testing framework developed by Microsoft. Other examples of end-to-end testing tools include Cypress, Selenium, and Puppeteer.

Here is an example of E2E tests from the freeCodeCamp codebase using Playwright. The `beforeEach` hook will run before each of the tests. The tests check that the donor has a supporter link in the menu bar, as well as a special stylized border around their avatar:

```
test.beforeEach(async ({ page }) => {
  execSync("node ./tools/scripts/seed/seed-demo-user --set-true isDonating");
  await page.goto("/donate");
});

...

test("The menu should have a supporters link", async ({ page }) => {
  const menuButton = page.getByTestId("header-menu-button");
  const menu = page.getByTestId("header-menu");

  await expect(menuButton).toBeVisible();
  await menuButton.click();

  await expect(menu).toBeVisible();

  await expect(page.getByRole("link", { name: "Supporters" })).toBeVisible();
});

test("The Avatar should have a special border for donors", async ({ page }) => {
  const container = page.locator(".avatar-container");
  await expect(container).toHaveClass("avatar-container gold-border");
});
```

Usability Testing
-----------------

* **Usability Testing**: Usability testing is when you have real users interacting with the application to discover if there are any design, user experience, or functionality issues in the app. Usability testing focuses on the intuitiveness of the application by users.
* **Four Common Types of Usability Testing**:
  + **Explorative**: Explorative usability testing involves users interacting with the different features of the application to better understand how they work.
  + **Comparative**: Comparative testing is where you compare your application's user experience with similar applications in the marketplace.
  + **Assessment**: Assessment testing is where you study how intuitive the application is to use.
  + **Validation**: Validation testing is where you identify any major issues that will prevent the user from using the application effectively.
* **Usability Testing Tools**: Examples of tools for usability testing include Loop11, Maze, Userbrain, UserTesting, and UXTweak.

Compatibility Testing
---------------------

* **Compatibility Testing**: The goal of compatibility testing is to ensure that your application works in different computing environments.
* **Different Types of Compatibility Testing**:
  + **Backwards Compatibility**: Backwards compatibility refers to when the software is compatible with earlier versions.
  + **Forwards Compatibility**: Forwards compatibility refers to when the software and systems will work with future versions.
  + **Hardware Compatibility**: Hardware compatibility is the software's ability to work properly in different hardware configurations.
  + **Operating Systems Compatibility**: Operating systems compatibility is the software's ability to work on different operating systems, such as macOS, Windows, and Linux distributions like Ubuntu and Fedora.
  + **Network Compatibility**: Network compatibility means the software can work in different network conditions, such as different network speeds, protocols, security settings, etc.
  + **Browser Compatibility**: Browser compatibility means the web application can work consistently across different browsers, such as Google Chrome, Safari, Firefox, etc.
  + **Mobile Compatibility**: It is important to ensure that your software applications work on a variety of Android and iOS devices, including phones and tablets.

Performance Testing
-------------------

* **Performance Testing**: In performance testing, you test an application's speed, responsiveness, scalability, and stability under different workloads. The goal is to resolve any type of performance bottleneck.
* **Different Types of Performance Testing**:
  + **Load Testing**: Load testing determines how a system behaves during normal and peak load times.
  + **Stress Testing**: Stress testing is where you test your application in extreme loads and see how well your system responds to the higher load.
  + **Soak Testing (Endurance Testing)**: Soak testing or endurance testing is a type of load testing where you test the system with a higher load for an extended period of time.
  + **Spike Testing**: Spike testing is where you dramatically increase and decrease the loads and analyze the system's reactions to the changes.
  + **Breakpoint Testing (Capacity Testing)**: Breakpoint testing or capacity testing is where you slowly increment the load over time to the point where the system starts to fail or degrade.

Security Testing
----------------

* **Security Testing**: Security testing helps identify vulnerabilities and weaknesses.
* **Security Principles**:
  + **Confidentiality**: This protects against the release of sensitive information to other recipients that aren't the intended recipient.
  + **Integrity**: This involves preventing malicious users from modifying user information.
  + **Authentication**: This involves verifying the user's identity to ensure that they are allowed to use that system.
  + **Authorization**: This is the process of determining what actions authenticated users are allowed to perform or which parts of the system they are permitted to access.
  + **Availability**: This ensures that information and services are available to authorized users when they need it.
  + **Non-Repudiation**: This ensures that both the sender and recipient have proof of delivery and verification of the sender's identity. It protects against the sender denying having sent the information.
* **Common Security Threats**:
  + **Cross-Site Scripting (XSS)**: XSS attacks happen when an attacker injects malicious scripts into a web page and then executes them in the context of the victim's browser.
  + **SQL Injection**: SQL injection allows malicious users to inject malicious code into a database.
  + **Denial-of-Service (DoS) Attack**: DoS attack is when malicious users flood a website with a high number of requests or traffic, causing the server to slow down and possibly crash, making the site unavailable to users.
* **Categories of Security Testing Tools**:
  + **Static Application Security Testing**: These tools evaluate the source code for an application to identify security vulnerabilities.
  + **Dynamic Application Security Testing**: These tools interface with the application's front-end to uncover potential security weaknesses. DAST tools do not have access to the source code.
* **Penetration Testing (pentest)**: Penetration testing is a type of security testing that involves creating simulated cyberattacks on the application to identify any vulnerabilities in the system.

A/B Testing
-----------

* **A/B Testing**: A/B testing involves comparing two versions of a page or application and studying which version performs better. It is also known as bucket or split testing. A/B testing allows you to make more data-driven decisions and continually improve the user experience.
* **Tools for A/B Testing**: Examples of tools to use for A/B testing include GrowthBook and LaunchDarkly.

Alpha and Beta Testing
----------------------

Once the initial development and software testing are complete, it is important to have the application tested by testers and real users. This is where alpha and beta testing come in.

* **Alpha Testing**: Alpha testing is done by a select group of testers who go through the application to ensure there are no bugs before it is released into the marketplace. Alpha testing is part of acceptance testing and utilizes both white and black box testing techniques.
* **Beta Testing**: Beta testing is where the application is made available to real users. Users can interact with the application and provide feedback. Beta testing is also a form of user acceptance testing.
* **Acceptance Testing**: Acceptance testing ensures that the software application meets the business requirements and the needs of users before its release.
* **Black Box Testing**: Black box testing only focuses on the expected behavior of the application.
* **White Box Testing**: White box testing involves the tester knowing the internal components and performing tests on them.

Regression Testing
------------------

* **Regression**: Regression refers to situations where new changes unintentionally break existing functionality.
* **Regression Testing**: Regression testing helps catch regression issues. In regression testing, you re-run functional tests against parts of your application to ensure that everything still works as expected.
* **Tools for Regression Testing**: Tools that you can use to perform regression testing include Puppeteer, Playwright, Selenium, and Cypress.
* **Techniques for Regression Testing**:
  + **Unit Regression Testing**: This is where you have a list of items that need to be tested each time major changes or fixes are implemented into the app.
  + **Partial Regression Testing**: This involves targeted approaches to ensure that new changes have not broken specific aspects of the application.
  + **Complete Regression Testing**: This runs tests against all the functionalities in the codebase. This is the most time-consuming and detailed option.
* **Retesting**: Retesting is used to check for known issues and ensure that they have been resolved. In contrast, regression testing searches for unknown issues that might have occurred through recent changes in the codebase.

---

