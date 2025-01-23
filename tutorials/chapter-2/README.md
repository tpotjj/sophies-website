```markdown
# CSS Basics: Styling Your HTML with Style!

In the HTML tutorial, you learned how to structure a webpage. Now, let's add some style and personality with CSS (Cascading Style Sheets)! This tutorial will give you a quick introduction to CSS and show you how to make your webpages look awesome.

## What is CSS?

CSS is a language that describes the presentation of an HTML document. It controls things like:

*   **Colors:** Text color, background color, etc.
*   **Fonts:** Font family, font size, font weight (bold, etc.).
*   **Layout:** Positioning of elements, spacing, etc.
*   **And much more!**

## How CSS Works: Rules and Selectors

CSS uses **rules** to define how elements should be styled. Each rule has two main parts:

1. **Selector:** This targets the HTML element(s) you want to style.
2. **Declaration Block:** This contains one or more **declarations** that specify the style properties and their values.

**Example:**

```css
p {
  color: blue;
  font-size: 16px;
}
```

*   **`p`** is the **selector** – it targets all `<p>` (paragraph) elements.
*   **`{ ... }`** is the **declaration block**.
*   **`color: blue;`** and **`font-size: 16px;`** are **declarations**.
    *   `color` and `font-size` are **properties**.
    *   `blue` and `16px` are **values**.

## Ways to Add CSS to HTML

There are three main ways to add CSS to your HTML:

1. **Inline Styles (not recommended for most cases):** You can add style directly to an HTML element using the `style` attribute.

    ```html
    <p style="color: red;">This text will be red.</p>
    ```

2. **Internal Stylesheet (within the `<head>`):** You can embed CSS rules within `<style>` tags in the `<head>` section of your HTML.

    ```html
    <!DOCTYPE html>
    <html>
    <head>
        <title>My Webpage</title>
        <style>
            h1 {
                color: green;
            }
        </style>
    </head>
    <body>
        <h1>This heading will be green.</h1>
    </body>
    </html>
    ```

3. **External Stylesheet (recommended for larger projects):** You can create a separate `.css` file and link it to your HTML using the `<link>` tag in the `<head>`.

    *   **styles.css:**

        ```css
        body {
            background-color: lightyellow;
        }

        h1 {
            color: navy;
            text-align: center;
        }

        p {
            font-family: Arial, sans-serif;
            font-size: 18px;
        }
        ```

    *   **index.html:**

        ```html
        <!DOCTYPE html>
        <html>
        <head>
            <title>My Webpage</title>
            <link rel="stylesheet" href="styles.css">
        </head>
        <body>
            <h1>Welcome to My Page</h1>
            <p>This is a paragraph of text.</p>
        </body>
        </html>
        ```

## Common CSS Properties

Here are some essential CSS properties to get you started:

*   **`color`:** Sets the text color.
*   **`background-color`:** Sets the background color of an element.
*   **`font-family`:** Specifies the font for the text.
*   **`font-size`:** Sets the size of the text.
*   **`text-align`:** Aligns the text (left, right, center, justify).
*   **`margin`:** Controls the space around an element (outside its border).
*   **`padding`:** Controls the space between an element's content and its border.
*   **`border`:** Adds a border around an element.
*   **`width`:** Sets the width of an element.
*   **`height`:** Sets the height of an element.

## CSS Selectors: Targeting Elements

Selectors are crucial for applying styles to the right elements. Here are some common selector types:

*   **Element Selector:** Targets elements by their tag name.

    ```css
    p { color: blue; } /* Targets all <p> elements */
    ```

*   **ID Selector:** Targets an element with a specific `id` attribute. (IDs must be unique on a page.)

    ```html
    <p id="intro">This is the introduction paragraph.</p>
    ```

    ```css
    #intro { font-weight: bold; } /* Targets the element with id="intro" */
    ```

*   **Class Selector:** Targets elements with a specific `class` attribute. (Multiple elements can have the same class.)

    ```html
    <p class="highlight">This is important.</p>
    <p class="highlight">This is also important.</p>
    ```

    ```css
    .highlight { background-color: yellow; } /* Targets elements with class="highlight" */
    ```

## Practice Time: Style Your Webpage!

Let's add some CSS to the HTML page you created in the previous tutorial (or create a new one).

1. **Copy the file `index.html` from chapter-1 into chapter-2:**

2. **Create a CSS File:** Create a new file called `styles.css` in the same folder as your `index.html`.

2. **Link the CSS File:** Add the `<link>` tag to the `<head>` of your `index.html`, as shown in the example above.

3. **Add CSS Rules:** Start adding CSS rules to your `styles.css` file (or within `<style>` tags in the `<head>`). Here are some ideas to try:

    *   Change the background color of the `body`.
    *   Change the color and font family of the `<h1>` heading.
    *   Center the `<h1>` heading using `text-align`.
    *   Add some margin or padding to the `<p>` elements.
    *   Give an image a border.
    *   Create a class to highlight certain text and apply it to some elements in your HTML.

**Example `styles.css`:**

```css
body {
  background-color: #f0f0f0; /* Light gray */
}

h1 {
  color: #336699; /* Dark blue */
  font-family: "Times New Roman", serif;
  text-align: center;
}

p {
  font-size: 16px;
  line-height: 1.5; /* Adjust line spacing */
  margin-bottom: 20px; /* Add space between paragraphs */
}

img {
  border: 2px solid #ccc; /* Light gray border */
  width: 300px;
}

.highlight {
  background-color: #ffffcc; /* Light yellow */
  padding: 5px;
}
```

## The Box Model

The **Box Model** is a fundamental concept in CSS. Every element is treated as a rectangular box with the following properties:

*   **Content:** The actual content of the element (text, image, etc.).
*   **Padding:** The space between the content and the border.
*   **Border:** The line around the padding and content.
*   **Margin:** The space outside the border, separating the element from other elements.

You can adjust these properties using CSS to control the spacing and layout of your elements.
