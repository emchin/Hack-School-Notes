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

The `<h>` elements are header elements. They display text on a webpage at different sizes.

<img href="http://coschedule.com/blog/wp-content/uploads/html-heading-tag-levels.png">

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
