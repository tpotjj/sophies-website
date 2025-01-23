# HTML Basics: A Quick and Fun Introduction

Welcome to the world of web development! This short tutorial will teach you the fundamentals of HTML (HyperText Markup Language), the language that forms the structure of every website you visit. Don't worry, it's easier than you think!

## What is HTML?

Imagine building a house. You need a solid foundation, walls, a roof, and maybe some windows and doors. HTML is like the blueprint for a website – it defines the different elements and how they're organized.

HTML uses **tags** to label different parts of your content, like headings, paragraphs, images, and links. These tags tell the web browser (like Chrome, Firefox, or Safari) how to display the content on the page.

## Getting Started: Your First HTML File

Let's create your very first webpage!

1. **Create index.html:** On the left side, you see the file structure we are currently working in, under tutorials -> chapter-1 create a new file called: `index.html`. Do this by right clicking on the folder `chapter-1` and selecting `New File...`.

2. **Write the Basic Structure:**  Copy and paste this code into your text editor:

    ```html
    <!DOCTYPE html>
    <html>
    <head>
        <title>Sophie's First Webpage</title>
    </head>
    <body>
        <h1>Hello, world!</h1>
    </body>
    </html>
    ```

3. This all might go a little fast, what are all the things that I just copied? Let's break this down: Inbetween the <head> & </head> elements, there is information which is not directly displayed on the webpage but is crucial for the browser, search engines, and other services to understand the page's structure, appearance, and behavior. In this case, we told the Browser that the name of this website is: 'Sophie's First Webpage'. Between the <body> & </body> elements, we've specified what the Browser should display to the User, which in this case is: `Hello, world!`.

4. **Save the File:** Save by pressing `CMD + s`.

5. **Open in a Browser:** On the left side, in the file structure, you see the `index.html` appear under `chapter-1`. Right click on `index.html` and select: `Copy Path`. Open a new Browser tab and paste the value you just copied & press enter.

6. **Sophie, you are amazing:** Congratulations, this is your very first, self made website

P.S. displaying `Hello World` is something all developers do when they try out a new programming language or a new tool, it somehow became a cult.

## Understanding the Code (breakdown):

Let's break down what each part of the code means:

*   **`<!DOCTYPE html>`:** This tells the browser that it's dealing with an HTML5 document (the latest version of HTML).
*   **`<html>`:** This is the root element of every HTML page. Everything else goes inside it.
*   **`<head>`:** This section contains meta-information about the page, like the title that appears in the browser tab.
    *   **`<title>`:**  Sets the title of your webpage.
*   **`<body>`:** This is where the visible content of your webpage goes – text, images, etc.
    *   **`<h1>`:**  This is a heading (the largest one). There are also `<h2>`, `<h3>`, down to `<h6>` for smaller headings.
    *   **`<p>`:** This is a paragraph of text.

## Common HTML Tags:

Here are some of the most frequently used HTML tags you should know:

*   **Headings:**
    ```html
    <h1>Main Heading</h1>
    <h2>Subheading</h2>
    <h3>Smaller Subheading</h3>
    ```

*   **Paragraphs:**
    ```html
    <p>This is a paragraph of text. You can write as much as you want here.</p>
    ```

*   **Links:**
    ```html
    <a href="https://www.wikipedia.org">This is a link to wikipedia.org</a>
    ```
    *   **`<a>`:**  The anchor tag creates a link.
    *   **`href`:** This attribute specifies the URL (web address) the link goes to.

*   **Images:**
    ```html
    <img src="image.jpg" alt="Description of the image">
    ```
    *   **`<img>`:** The image tag embeds an image.
    *   **`src`:** This attribute specifies the path or URL to the image file.
    *   **`alt`:** This attribute provides alternative text for the image, which is important for accessibility (screen readers) and if the image can't be loaded.

*   **Lists:**
    *   **Unordered List (bullet points):**
        ```html
        <ul>
            <li>Item 1</li>
            <li>Item 2</li>
            <li>Item 3</li>
        </ul>
        ```
    *   **Ordered List (numbered):**
        ```html
        <ol>
            <li>First item</li>
            <li>Second item</li>
            <li>Third item</li>
        </ol>
        ```

## Practice Time: Let's Add More to Your Page!

Now it's your turn to experiment!

1. **Add a Heading:** Add an `<h2>` heading below the `<h1>` that says "About Me".
2. **Add a Paragraph:** Write a short paragraph about yourself below the "About Me" heading.
3. **Add an Image:**
    *   Find an image on your computer or download one from the internet.
    *   Save the image in the same folder as your `index.html` file.
    *   Add an `<img>` tag to your HTML to display the image. Remember to use the correct `src` and `alt` attributes.
4. **Add a Link:** Add a link to your favorite website.
5. **Add a List:** Create an unordered list of your favorite hobbies.

**Example of what your code might look like after adding these elements:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Webpage</title>
</head>
<body>
    <h1>Hello, world!</h1>
    <p>This is my first webpage.</p>

    <h2>About Me</h2>
    <p>I'm learning HTML, and it's really fun! I like to...</p>

    <img src="my-photo.jpg" alt="A photo of me">

    <p>Visit my favorite website: <a href="https://www.wikipedia.org/">Wikipedia</a></p>

    <h2>My Hobbies</h2>
    <ul>
        <li>Coding</li>
        <li>Reading</li>
        <li>Hiking</li>
    </ul>
</body>
</html>