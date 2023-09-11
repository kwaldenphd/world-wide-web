# The World Wide Web

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>This tutorial was written by Katherine Walden and is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

## Lab Objectives

By the end of this lab you will be able to:
-	Identify the key features of an IDE
-	Use the Repl.it IDE to generate HTML pages that include links, images, and tables
-	Use the Repl.it IDE to generate CSS stylesheets to format your HTML pages

<table>
 <tr><td>
<img src="https://elearn.southampton.ac.uk/wp-content/blogs.dir/sites/64/2021/04/PanPan.png" alt="Panopto logo" width="50"/></td>
<td><a href="https://notredame.hosted.panopto.com/Panopto/Pages/Viewer.aspx?pid=5ef8c193-e587-45dd-9ae8-b07a001ab734">Lecture/live coding playlist</a></td>
  </tr>
  </table>

## Acknowledgements

This lab is based on the "Project 3: HTML/CSS" project materials developed by [Lindsay K. Mattock](http://lindsaymattock.net/) for the the [SLIS 5020 Computing Foundations course](http://lindsaymattock.net/computingfoundations.html). 

# Table of Contents
- [Lecture & Live Coding](#lecture--live-coding)
- [Key Concepts](#key-concepts)
- [Lab Notebook Template](#lab-notebook-template)
- [The World Wide Web](the-world-wide-web)
- [Tutorial: Building Content For the Web](#tutorial-building-content-for-the-web)
  * [Well-Formed HTML](#well-formed-html)
  * [Building Web Pages](#building-web-pages)
  * [Link Web Pages](#linking-web-pages)
  * [Adding Images](#adding-images)
  * [Building Tables](#building-tables)
  * [Style & Formatting](#style--formatting)
    * [Cascading Style Sheets (CSS)](#cascading-style-sheets-css)
- [Application](#application)
- [Additional Resources](#additional-resources)
- [Lab Notebook Questions](#lab-notebook-questions)

# Lecture & Live Coding

Throughout this lab, you will see a Panopto icon at the start of select sections.

This icon indicates there is lecture/live coding asynchronous content that accompanies this section of the lab. 

You can click the link in the figure caption to access these materials (ND users only).

Example:

<table>
 <tr><td>
<img src="https://elearn.southampton.ac.uk/wp-content/blogs.dir/sites/64/2021/04/PanPan.png" alt="Panopto logo" width="50"/></td>
<td><a href="https://notredame.hosted.panopto.com/Panopto/Pages/Viewer.aspx?pid=5ef8c193-e587-45dd-9ae8-b07a001ab734">Lecture/live coding playlist</a></td>
  </tr>
  </table>

## Key Concepts

[Click here](https://github.com/kwaldenphd/world-wide-web/blob/main/key-concepts.md) for a full list of key concepts and definitions for this lab.

## Lab Notebook Template

[Link to Replit workspace template](https://replit.com/team/eoc-f23/Buliding-Web-Content) (ND users, Replit)

# The World Wide Web 

<table>
 <tr><td>
<img src="https://elearn.southampton.ac.uk/wp-content/blogs.dir/sites/64/2021/04/PanPan.png" alt="Panopto logo" width="50"/></td>
<td><a href="https://notredame.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=7bacf9bb-6940-44f2-8e90-aef401865c19">The World Wide Web</a></td>
  </tr>
  </table>

## Key Concepts

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/WWW_Berners_Lee.png?raw=true" width="500"></p>

**World Wide Web (WWW)**
- "The World Wide Web (WWW), commonly known as the Web, is an information system where documents and other web resources are identified by Uniform Resource Locators (URLs, such as https://www.example.com/), which may be interlinked by hypertext, and are accessible over the Internet. The resources of the WWW are transferred via the Hypertext Transfer Protocol (HTTP) and may be accessed by users by a software application called a web browser and are published by a software application called a web server" ([Wikipedia](https://en.wikipedia.org/wiki/World_Wide_Web))

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Hypertext.png?raw=true" width="500"></p>

**Hyerlinks & Hypertext**
- "In computing, a hyperlink, or simply a link, is a reference to data that the user can follow by clicking or tapping. A hyperlink points to a whole document or to a specific element within a document. Hypertext is text with hyperlinks" ([Wikipedia](https://en.wikipedia.org/wiki/Hyperlink))

**Web Browsers**
- "A web browser (also referred to as an Internet browser or simply a browser) is application software for accessing the World Wide Web or a local website. When a user requests a web page from a particular website, the web browser retrieves the necessary content from a web server and then displays the page on the user's device" ([Wikipedia](https://en.wikipedia.org/wiki/Web_browser))
- Sample web browsers: Internet Exporer, Microsoft Edge, Mozilla Firefox, Safari, Google Chrome

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/URL.png?raw=true" width="500"></p>

**Uniform Resource Locator (URL)**
- "A Uniform Resource Locator (URL), colloquially termed a web address, is a reference to a web resource that specifies its location on a computer network and a mechanism for retrieving it. A URL is a specific type of Uniform Resource Identifier (URI), although many people use the two terms interchangeably" ([Wikipedia](https://en.wikipedia.org/wiki/URL))

**Web Server**
- "A web server is computer software and underlying hardware that accepts requests via HTTP (the network protocol created to distribute web content) or its secure variant HTTPS" ([Wikipedia](https://en.wikipedia.org/wiki/Web_server))

**Hypertext Transfer Protocol (HTTP)**
- "The Hypertext Transfer Protocol (HTTP) is an application protocol for distributed, collaborative, hypermedia information systems. HTTP is the foundation of data communication for the World Wide Web, where hypertext documents include hyperlinks to other resources that the user can easily access, for example by a mouse click or by tapping the screen in a web browser" ([Wikipedia](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol))

**Markup Language**
- "In computer text processing, a markup language is a system for annotating a document in a way that is syntactically distinguishable from the text, meaning when the document is processed for display, the markup language is not shown, and is only used to format the text" ([Wikipedia](https://en.wikipedia.org/wiki/Markup_language))
- [Click here](https://youtu.be/C0ivP3KYO3A) to learn more about markup languages.

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/HTML_Tag.png?raw=true" width="500"></p>

**Hypertext Markup Language (HTML)**
- “HyperText Markup Language, invented by Tim Berners-Lee as the basis for the World Wide Web….based on the international standard SGML (Standardized Generalized Markup Language), which was originally developed for the representation of print documents in electronic form. HTML created a notation for hypertext that has become the global standard, and provided the basis for the standardized linking and display of documents independent of the platform, operating system, and application in which they were created.” (Janet Murray, *[Inventing the Medium: Principles of Interaction Design as a Cultural Practice](https://mitpress.mit.edu/9780262016148/inventing-the-medium/)*, pp. 424)

**Tag**
- “A heading in a web page as indexing, structural, or formatting terms. Formatting tags identify structural parts of a document, such as <heading> or display <italics>.” (Janet Murray, *[Inventing the Medium: Principles of Interaction Design as a Cultural Practice](https://mitpress.mit.edu/9780262016148/inventing-the-medium/)*, pp. 440)

**Cascading Style Sheets (CSS)**
- "Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language such as HTML or XML" ([Wikipedia](https://en.wikipedia.org/wiki/CSS))

[Click here](https://github.com/kwaldenphd/world-wide-web/blob/main/key-concepts.md) for a full list of key concepts and definitions for this lab.

## Comprehension Check

<table>
 <tr><td>
<img src="https://github.com/kwaldenphd/internet/blob/main/images/clipboard.png?raw=true" alt="Clipboard icon" width="50"/></td>
  <td><a href="https://docs.google.com/forms/d/e/1FAIpQLSec8RlhNcj9YKG6Fliv3LBm35y4fhO_-mcENs1Vvfe5aHJ6Mw/viewform?usp=sf_link">The WWW Comprehension Check</a></td>
  </tr>
  </table>

# Tutorial: Building Content For the Web

- [Well-Formed HTML](#well-formed-html)
- [Building Web Pages](#building-web-pages)
- [Link Web Pages](#linking-web-pages)
- [Adding Images](#adding-images)
- [Building Tables](#building-tables)
- [Style & Formatting](#style--formatting)
  * [Cascading Style Sheets (CSS)](#cascading-style-sheets-css)
- [Putting It All Together](#putting-it-all-together)
- [HTML/CSS Lab Notebook Questions](#htmlcss-lab-notebook-questions)
- [Additional Resources](#additional-resources)

[Link to Replit workspace template](https://replit.com/team/eoc-f22/HTMLCSSLab) (ND users, Replit)

REPLIT TEMPLATE

## Well-Formed HTML

Create a `.txt` file on your computer and add the text listed below. Save the file as `hello-world.html` and open it in a web browser.

```HTML
<html>
<body>Hello World</body>
</html>
```

This is a very basic HTML document. The HTML tags `<HTML>` identify this document as a html document. The body tags `<body>` enclose the content that will be visible on the page. You should see just the text “Hello World!” The browser has translated the HTML tags and returned only the text.

`hello-world.html` contains the minimum requirements for an HTML document. However, it is best practice to create a HTML document that is “well formed,” that is, that it follows all of the grammar, vocabulary, and syntax rules of html. We can check the well-formed-ness of this document in a validator like the [W3C Markup Validation Service](https://validator.w3.org). 

Head to the W3C validator and click on “Validate by Direct Input” and copy and paste the code above into the validator and click `check`. You should receive a few errors. 
- [W3Schools, "HTML head tag"](https://www.w3schools.com/tags/tag_head.asp)
- [W3Schools, "HTML !DOCTYPE Declaration"](https://www.w3schools.com/tags/tag_doctype.asp)
- [W3Schools, "HTML ISO Language Codes"](https://www.w3schools.com/tags/ref_language_codes.asp)
  
HTML is pretty forgiving, but other languages are not, so it’s best to practice following all of the rules from the start. Navigate to your Replit workspace for this lab and open the `index.html` document.

<table>
 <tr><td>
<img src="https://elearn.southampton.ac.uk/wp-content/blogs.dir/sites/64/2021/04/PanPan.png" alt="Panopto logo" width="50"/></td>
<td><a href="https://notredame.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=03112275-fe69-4b36-85e5-aef50171900c">IDE Overview & Getting Started With Replit</a></td>
  </tr>
  </table>

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Fig_A.png?raw=true" width="500"></p>

Comments are indicated by `<!-- and -->` and are written for the user (not the computer). These special start and end tags tell the computer to ignore what follows. Comments are used to include instructions and explanations about the code in a human-readable form. You can use comments throughout your code to leave notes for yourself or describe what the code is doing (or what you want it to do).

A few other pieces of information Replit has added to this page so we have valid, well-formed HTML:
- The `<!DOCTYPE` declaration tells the computer this is an HTML document
- The opening `<html>` tag marks the start of the page/document
- We also have additional information like XHTML specification, namespace, and document language (`en`)

## Building Web Pages

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/HTML_Page_Structure.png?raw=true" width="500"></p>

Now that we have a template for a valid, well-formed HTML page, we can start adding content to the page. Between the `<head>` tags you will see a set of `<title>` tags. The `<head>` of the document is reserved for metadata, but also includes the `<title>` of the page which is represented in the tabs in some web browsers. 

```html
  <head>
    <title>YOUR PAGE TITLES GOES HERE</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
  </head>
```

Replace `YOUR PAGE TITLE GOES HERE` between the `<title>` tags to give your document a new title. Click `Run` to see the updated page.

Now, let’s modify the body. This is where the content that we will see in the web browser is entered. HTML uses a number of different formatting tags. You can use the W3Schools's ["HTML Reference"](https://www.w3schools.com/tags/default.asp) to browse through some of the different options. 

For now, we’ll use `<h1>` (heading 1) and `<p>` (paragraph). After the first `<body>` tag, place a `<h1>` tag on a new line. 

A couple things to notice:
- The line is indented. This isn’t a requirement of HTML, but it is a convention that is used by coders to write cleaner code. The indentation allows you to easily determine what tags are nested within each other. For example, the `<title>` and `<meta>` tags are nested within the `<head>` tags. Now, our `<h1>` is nested within the `<body>`. The use of the tabs simply makes the code easier for us to read, but the computer doesn’t care (with Python the indentation is important and will cause errors if the indents do not appear in the right place).
- Repl.it has completed your `<h1>` with a closing `</h1>` tag. The closing tag is not required for all HTML tags, but it is good practice to close all of your tags. This is a good example. Without a closing tag, everything that follows will be formatted as a `<h1>`. Some IDEs include an auto-complete function to help you prevent errors in your code and create valid documents.

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Image_5.jpg?raw=true" width="500"></p>

Go ahead and enter some content between the `<h1>` tags. `<h1>` is preformatted as first level heading text. We’ll see how it looks in a minute. 

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Image_6.jpg?raw=true" width="500"></p>

Next add a `<p>` tag and type some text. `<p>` tags are preformatted as paragraphs with padding between paragraphs.

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Fig_J.png?raw=true" width="500"></p>

Repl.it has another function that will be helpful as we develop our websites. Click the `Run` button and your `.html` document will display in Replit's web browser. Repl.it will auto-save your work (like Google Docs). For other IDEs, you can press <code>Control + S</code> to save file updates.

<blockquote><h1>Why <code>index.html</code>?</h1><br><code>index.html</code> is the name of the default landing page for websites. The web server (the computer hosing the site) will automatically recognize <code>index.html</code> as the first page or the home page of a website. Some servers use other variations like <code>home.html</code>, but we’ll use <code>index.html</code>.</blockquote>

We have just created is a single web page. To build a web site, we likely want multiple pages of linked content. 

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Fig_L.png?raw=true" width="500"></p>

Let’s create a second `.html` file by clicking on the `+` "Add File" icon in the upper left-hand corner. Save this file as `page2.html`. 

We can copy the HTML from `index.html` to make sure we're starting with an HTML document that is well-formed and valid.

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Fig_K.png?raw=true" width="500"></p>

Add some content to your second page, starting with a title, `<h1>` and `<p>` tags. 

## Linking Web Pages

Now, let’s add a link to the second page on our `index.html` page. We add links with the `<a>` tag and the `href` attribute. The `a` tag defines a hyperlink, and the `href` attribute shows the link destination.`<a href>` tag. This tag allows us to link pages in the same website and link out to pages that exist on external websites.

The tag syntax is as follows: `<a href="URL to page">Text that will appear as the link</a>`. 
  
Below your paragraph tag on the `index.html` page add the line `<a href=”page2.html”>Link to page 2</a>.`
- Learn more about the `<a href>` tag via W3Schools: http://www.w3schools.com/TAGS/att_a_href.asp

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Image_10.png?raw=true" width="500"></p>

Run `index.html` to see the updated file with a link. When you click on “Link to page 2” your `page2.html` file should open. In this case, our URL to the page in our `<a href>` tags is just the name of new page we created. We do not need a full URL (http://www.somewhere.com) because we are calling a file that is stored in the same directory on our server (the repl).
- NOTE: If your link is not working, try re-typing the quotation marks around the destination link.

If we had saved this file to another folder or directory, we would need to include the full file path, including any directory information. For example if we had put `page2.html` in a folder titled "pages," the `a href` tag would look like `<a href="pages/page2.html">`.

## Adding Images

Let’s add an image to the `index.html` page. 

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Fig_I.png?raw=true" width="500"></p>

Find an image that you like on the web, save it to your local computer, and upload the file to your repl. 

The `<img>` tag is very similar to the `<a href>` tag that we just used. It has two required attributes:
- `src` or the source
-  `alt` or the alternative text for the image

`src` can be a local file or a URL to an image on the web, just like the href attribute in the `<a href>` tag. `alt` is for the alternative text or the text that is displayed for screen readers or browsers that don’t support images. 

<blockquote>Learn more about the <code>img</code> tag via <a href="http://www.w3schools.com/tags/tag_img.asp">W3Schools</a>.</blockquote>

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Fig_M.png?raw=true" width="500"></p>

On your `index.html` page, add the line `<img src="imagefilename" alt=Description of image>` in the `<body>`. Be sure to use your image file name in place of the italicized text above. 

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Image_12.jpg?raw=true" width="500"></p>

View the page in the Replit browser (using `Run`) to see if the image has loaded correctly.

At this point, our website project only has one image. If we end up using multiple images, we might want to put all the images files in an `images` folder.

Create an `images` folder and move your single image file into the folder. What happens when you hit `Run`? What would you need to modify in the HTML to correctly display this image?
- HINT: Think about absolute versus relative file paths.

## Building Tables

HTML uses a few core tags for web pages that include tables.
- `table` (marks the start and end of a table
- `tbody` (marks the start and end of the table body)
- `tr` (marks the start and end of each table row)
- `th` (marks the start and end of each column in the first row of the table)
- `td` (marks the start and end of each column after the first row of the table)

How we might see those tags combined in a table structure:

```HTML
<table>
 <tr>
  <th>First Column Header</th>
  <th>Second Column Header</th>
  <th>Third Column Header</th>
 </tr>
 <tr>
  <td>Data in first column/first row</td>
  <td>Data in second column/first row</td>
  <td>Data in third column/first row</td>
 </tr>
 <tr>
  <td>Data in first column/second row</td>
  <td>Data in second column/second row</td>
  <td>Data in third column/second row</td>
 </tr>
</table>
```

The output of that HTML would look like:

<table>
 <tr>
  <th>First Column Header</th>
  <th>Second Column Header</th>
  <th>Third Column Header</th>
 </tr>
 <tr>
  <td>Data in first column/first row</td>
  <td>Data in second column/first row</td>
  <td>Data in third column/first row</td>
 </tr>
 <tr>
  <td>Data in first column/second row</td>
  <td>Data in second column/second row</td>
  <td>Data in third column/second row</td>
 </tr>
</table>

Additional attributes like `align`, `style`, etc. can be used with many of these tags. For more on building tables in HTML:
- [W3Schools, "HTML Tables"](https://www.w3schools.com/html/html_tables.asp)
- [W3Schools, "HTML table tag"](https://www.w3schools.com/tags/tag_table.asp)

Add a table to one of your HTML pages (index.html or page2.html). You could create fictional data or add meaningful data from another source.

## Style & Formatting

HTML allows us to add style to our pages internally, or inline, using HTML tags. We’ve already styled our pages a bit using the `<h1>` tag. `<h1>` designates preformatted text that is larger than the `<p>` or paragraph text. But, what if we want to add color or change the font on our page? 

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Image_13.jpg?raw=true" width="500"></p>

We can add style to individual HTML element tags using `style` attributes. The syntax for style attributes is `style="STYLE_PROPERTY:PROPERTY_VALUE;"`

For example, if we wanted text characters in the `H1` tag to be blue and center aligned:
```HTML
 <h1 style="color:blue; text-align:center;">Hello World!</h1>
```

And if we wanted text in the `p` tag to have a light blue background and a different font:
```HTML
 <p style="background-color:powderblue; font-family:courier;">This is my first HTML page.</p>
```

All style elements are enclosed in quotation marks and include a semicolon after each element. To put that all together:

```HTML
<body>
 <h1 style="color:blue; text-align:center;">Hello World!</h1>
 <p style="background-color:powderblue; font-family:courier;">This is my first HTML page.</p>
</body>
```

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Image_14.png?raw=true" width="500"></p>

We can see how the style attributes are changing how the web page content displays:
- The `<h1>` heading has has a blue text color and is center-aligned
- The `<p>` content has a powder blue background color and Courier font

For more on HTML styles:
- HTML Styles: https://www.w3schools.com/html/html_styles.asp
- HTML Colors: https://www.w3schools.com/html/html_colors.asp

Take a look at the W3Schools [HTML Colors](https://www.w3schools.com/html/html_colors.asp) page. See anything familiar? HTML supports multiple formats for representing color.

If you haven't already, experiment with modifying your existing HTML pages to include some of these (or other) style elements.

### Cascading Style Sheets (CSS)

You can customize HTML using style attributes, but imagine you want all instances of the `<h1>` or `<p>` tag in your website to have the same formatting. Doing this with `style` would require adding code every time you use these elements.

Cascading Style Sheets (CSS) provides a more elegant way to add these style attributes across the pages in our site. For those familiar with website-building tools like WordPress, Weebly, or Wix, CSS is a main part of how different site "themes" are managed. 
- For more on CSS: https://www.w3schools.com/css/css_intro.asp

Let’s create a simple external CSS for our site. The CSS is cascading because there is a hierarchy to the way that styles are applied. 

If styles are defined within the document (as in the previous example), then they are applied before those in the stylesheet. This lets us override the stylsheet if there is particular content that we would like to style differently.

Open the `style.css` file already in your repl. The CSS file doesn’t contain any content, it only defines the styles for the various elements in HTML files. 

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Image_15.png?raw=true" width="500"></p>

Let's get started by adding a few styles for the background, `<h1>`, and `<p>`. Each tag is defined first- these are referred to as the selectors. 

Our style instructions for each tag are enclosed in `{ }`. These are called declarations. We can add as many style declarations as we would like in between the brackets, separating each with a semicolon. Each declaration has a property followed by a colon and then a value. 

It is common practice to place each declaration on a new line and to indent the declarations, but this is only to make the file easier for us to read and edit. The spacing has no impact on how the computer reads and interprets the code.

Putting that all together:

```CSS
body {
 background-color: lightblue;
 }
 
h1 {
 color: white;
 text-align: center;
}

p {
 font-family: courier;
 font-size: 20px;
}
```

This CSS sample has three declarations (`body`, `h1`, `p`), and each declaration has at least one property (`background-color`, `color`, `text-align`, etc).

Now we need to link the CSS to any HTML file where we want the style sheet to apply. This connection is called a reference. Each HTML page must reference the CSS to apply it to the page. 

We create this reference in the `<head>` of the HTML document with the other metadata. In the `<head>` of `index.html` add the reference `<link rel="stylesheet" type="text/css" href="mystyle.css">`.

```HTML
<head>
 <title>Page Title</title>
 <link rel="stylesheet" type="text/css" href="style.css">
```

This line can appear anywhere between the `<head>` and `</head>`. 
- The `<link>` tag is another way to create links to other documents. 
- In this case the `rel` attribute defines the relationship between the HTML file and the linking document. 
- The `type` defines the type and `href` contains the URL or location reference for the file.
  * To learn more about the `<link rel>` tag: http://www.w3schools.com/tags/att_link_rel.asp

<p align="center"><img src="https://github.com/kwaldenphd/internet/blob/main/images/Image_17.jpg?raw=true" width="500"></p>

Run the `index.html` file in the Replit browser to see the updated CSS. However, if you click on the link to `page2.html`, it will look the same as it did before. This is because we need to link the stylesheet to each of the pages. Add the same `<link rel="stylesheet" type="text/css" href="mystyle.css">` to `page2.html`. Now both pages should share the same style.

If you haven't already, experiment with creating a CSS and linking it to your HTML pages.

# Application

[Link to Replit workspace template](https://replit.com/team/eoc-f23/Buliding-Web-Content) (ND users, Replit)

Now it's your turn. The lab procedure has covered the tools you can use to get started, but you can also expand on what you've learned using the W3Schools HTML and CSS resources and documentation (be sure to cite resources you consult or reference- a list of URLs is fine). You're welcome to use or reuse the HTML/CSS content you created in the last section of the lab.

For now, your site needs to fit a few minimum requirements. 

First, the theme. Think of what you're building as a personal website that introduces you! You could focus on academics, hobbies, or clubs. You could focus on home, family, or pets. Up to you!

Next, the landing page. Build a landing page (`index.html`) that introduces you and provides a brief introduction to your site. 
- The landing page (`index.html`) must also link to at least one other page
- You'll also need at least one....
  * Image or logo (can be on any page)
  * External link (to a page outside your site; can be on any page)
  * Table built in HTML (can be on any page)

Last (but not least), style & formatting. Your site should include a CSS for your site. The CSS will be used across all pages of content to standardize the look and feel of your site.

That’s it. You are free to be as creative as you’d like as long as you meet these requirements. As you design your site, the W3Schools [HTML](http://www.w3schools.com/html/) and [CSS](http://www.w3schools.com/css/default.asp) includes tutorials or sample code tutorials for menus, tables, and other elements you could add to your site. Feel free to borrow code and CSS you find on the web (be sure to provide a link back to sources). Have fun and experiment!

<table>
 <tr><td>
<img src="https://elearn.southampton.ac.uk/wp-content/blogs.dir/sites/64/2021/04/PanPan.png" alt="Panopto logo" width="50"/></td>
<td><a href="https://notredame.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=f9d0322b-e52a-46cc-a7ad-af18015ab0a1">Submitting your website</a></td>
  </tr>
  </table>

All the materials for your website (`.html`, `.css`, and image files) can be submitted as a single `.zip` folder on Canvas. You can download the entire Replit project by clicking on the `Download as Zip` option under the three dots next to `Files` on the left-hand side of the page.

Also include a link to your Replit project workspace. This link is the URL that is active in your browser when you are working on this project in Replit.
- Link template: `https://replit.com/@USERNAME/PROJECTNAME`
- The link you copy in from Replit should include your username, followed by the project name

# Additional Resources

Interested in learning more about computer networks and the World Wide Web? The "[Additional Resources](https://github.com/kwaldenphd/internet/blob/main/additional-resources.md)" page in this repository includes links to a variety of content on...
- Conceptual and technical foundations
- Markup languages and HTML
- Cultural histories of the internet
- Identity and power in online spaces

# Lab Notebook Questions

[Link to Replit workspace template](https://replit.com/team/eoc-f23/Buliding-Web-Content) (ND users, Replit)

Q1: Include the website you built using HTML and CSS as your lab submission. Include a single `.zip` folder as well as a link to the Replit workspace for the website.

Website components:
- At least two pages (`index.html` and something else)
- At least one image
- At least one external link
- At least one table

<table>
 <tr><td>
<img src="https://elearn.southampton.ac.uk/wp-content/blogs.dir/sites/64/2021/04/PanPan.png" alt="Panopto logo" width="50"/></td>
<td><a href="https://notredame.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=f9d0322b-e52a-46cc-a7ad-af18015ab0a1">Submitting your website</a></td>
  </tr>
  </table>

All the materials for your website (`.html`, `.css`, and image files) can be submitted as a single `.zip` folder on Canvas. You can download the entire Replit project by clicking on the `Download as Zip` option under the three dots next to `Files` on the left-hand side of the page.

Also include a link to your Replit project workspace. This link is the URL that is active in your browser when you are working on this project in Replit.
- Link template: `https://replit.com/@USERNAME/PROJECTNAME`
- The link you copy in from Replit should include your username, followed by the project name
