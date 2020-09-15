# HTML/CSS (10/15)

Workshop Recording: (__insert-link-here__)

In this workshop, we learned about HTML and CSS. Specifically, we learned about **how to create website elements** and **how to style webpage elements**.

We used these ideas to to:
- [x] Create pokemon images and descriptions
- [x] Create a navbar
- [x] Style the Pokemon Generator text


## What is HTML/CSS?

HTML (Hyper-Text Markup Language) is a front-end language. It is used for structuring websites. If a website is like a house, then the HTML elements would be the foundations, walls, roof, etc.

CSS (Cascading Style Sheet) is another front-end language. It is used for styling websites. If a website is like a house, then the CSS elements would be the paint, decorations, color, etc that are applied to HTML elements.

In Hack School, we will be using HTML to create elements of the Pokemon Generator. We will be using CSS elements to style these HTML elements.


### How to create website elements

We create website elements using HTML.

HTML consists of a series of [elements] which are called using tag names enclosed with arrows `<tag name>`. Usually, but not always, these elements require an end tag `<\tag name>`.

Let's look at an example.

#### `<!DOCTYPE html>`, `<html>` and `<\html>`

All HTML is enclosed in three tags: `<!DOCTYPE html>` and `<html>` at the beginning, and `<\html>` at the end.

`<!DOCTYPE html>` is a unique tag that does not require an end tag. It tells the compiler that the following code will be be written in HTML.

`<html>` is a tag that begins the HTML. `<\html>` is the end tag that corresponds to `<html>`, and marks the end of the HTML. Between `<html>` and `<\html>` is all of our HTML code.

These three tags can be seen here:

```
<!DOCTYPE html>
<html>

<!-- content here -->

<\html>
```

Note that `<!-- -->` is a HTML tag that denotes a comment. Comments are used to make notes in code.

Inside of the `<html>` and `<\html>` tags are the `<head>` and `<body>` elements.


#### `<head>` and `<body>` elements

The `head` element contains all the website's metadata. Metadata might be shown in the top tab of the website, or it might not be shown.

The `body` element contains all the website's content. Content is what you see on the website itself.


#### Common HTML elements

##### `<img>` element

The `<img>` element creates an image. It is another unique element that does not have an end tag.

This element contains two attributes: `src` and `alt`. (If you look at `<img>` documentation, you will see that `<img>` has many more attributes, but we are  only using these two.)

The `src` attribute asks for a source where the computer can find an image. This can be a link, or, if the image is in the same folder as your code, you can simply give the file name. If you want to show an image, you NEED this attribute so the computer knows where to find the image!

The `alt` attribute asks for an alternate text to display if the computer cannot load or find the image. Unlike the `src` attribute, the `alt` attribute is not necessary to display an image; however, it is a good attribute to include for accessibility reasons or in case the user has slow wi-fi and can't load an image.

Here's an example of the `<img` element.
`<img src="image.jpg" alt="the thing didn't load" />`

##### `<a>` element

The `<a>` element creates a link. It has the end tag `</a`.
  
This element requires one attribute `href`. The `href` attribute asks for a reference link (where you will go if you click on the link). Usually, you can copy-paste a URL for this attribute.

The text contained between the two `<a>` tags will serve as your link.

`<a href="other-site.html">The text that shows up</a>`

##### `<h>` element

The `<h>` elements are header elements. They display bold text on a webpage at different sizes with `<h1>Heading One</h1>` being the largest text, and `<h6>small</h6>` being the smallest heading.

For reference, look at Slide 14 of the HTML/CSS slides.

##### `<p>` element

The `<p>` element is the plain-text elements. They display regular, unbolded text on a website.

For reference, look at Slide 14 of the HTML/CSS slides.


### How to create website elements

CSS determines the layout, design and color of a webpage. We style webpage elements with CSS.

While it is possible to style HTML using other HTML elements like `<font>`, it is a NIGHTMARE to implement in a website. You have to put the HTML style elements around every paragraph that you want styled, adding a new element for each change in font size/font color/background color/alignment...

Usually, when developing a website, developers use an external CSS.

CSS syntax follows this rule: `selector {property:value}`. We apply a `selector`(s) that describes an HTML element, and then we apply a `declaration` styling that element. Each declaration contains a `property` and a `value`.

For example, if we want to make each plain-text element have 14-pt font:

```p {font-size:14}```

This selects each element `p` in the HTML document, and applies a declaration. The declaration says that `font-size` (property) now is equal to `14` (value).

CSS contains other properties such as `background-color`, `color` and `border`. They are fairly self-explanatory, but if you want more information on CSS properties, check out the Simple Resources at the bottom of these notes!

#### Classes and Ids

Selecting all plain-text elements is okay if you want *all* plain-text to have font-size of 14. But what if you only want some plain-text to be styled this way?

That's where classes and ids come in.

A **class** is an identifier that can be used for multiple HTML elements. If you give the HTML element the attribute `class="example_class"`, then you can style that element by using `.example_class` as your CSS selector.

Note that you add a `.` before your `example_class` to tell the CSS compiler that `example_class` is a CLASS.

For example, if you modify elements in your HTML document with `example_class`:
```
<h1 class="example_class"> This text will be red. </h1>
<p class="example_class"> This text will be red. </p>
<p> This text will not be red. </p>
```

Then you can style those modified elements in your CSS document:
```
.example_class {
    color: 'red';
}
```

An **id** is an identifier that can only be used for *ONE* HTML element. If you give an HTML element the attribute `id="example_id"`, then you can style that element by using `#example_id` as your CSS selector.

Note that you add a `#` before your `example_id` to tell the CSS compiler that `example_id` is an ID.

For example, by tagging the first heading in HTML:
```
<h1 id="example_id"> This text will be blue and 20-pt. </h1>

<h2> Remember, I can't give this the id "example_id" because you can only use one id for one HTML element! </h2>
```

You can reference that in CSS by selecting the id:
```
#example_id {
    color: 'red';
    font-size: 20;
}
```


## Project Implementation

### Task 1

We want to do (insert task here) for our Pokemon generator.

For that, we use **main idea 1** and **main idea 2**.

```
example code here
```

<details> 
  <summary> Hint #1: </summary>
   Try doing this: <code> code </code>
</details>

## Simple Resources:

**Main Idea 1**:

Site #1: (link)

Site #2: (link)
