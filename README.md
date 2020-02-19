# HTML and CSS Lab

This tutorial was written by [Lindsay K. Mattock](http://lindsaymattock.net) and adapted by [Katherine Walden](https://github.com/kwaldenphd). 

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>
This tutorial is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

Over the next few weeks we are going to complete a number of programming projects. As you read in your assigned reading for this week, both of these languages require a specific syntax. The reading from w3 Schools suggested downloading a text editor to create your html files. We already have several options on our Pi, including the Leaf Pad text editor and Nano at the command line. But, there are other tools that provide additional functions that will help us to work with these languages. Before we start building our HTML pages we are going to install an Integrated Development Environment (IDE) that help us to write and find errors in our HTML. We will also use the IDE for future labs that work with Python.

<blockquote>Integrated Development Environment (IDE): a software application that provides comprehensive facilities to computer programmers for software development. An IDE normally consists of a source code editor, build automation tools and a debugger. Most modern IDEs have intelligent code completion. Some IDEs, such as NetBeans and Eclipse, contain a compiler, interpreter, or both; others, such as SharpDevelop and Lazarus, do not. https://en.wikipedia.org/wiki/Integrated_development_environment</blockquote>

## Lab Objectives

By the end of this lab you will be able to:
-	Install software at the Command Line
-	Identify the key features of an IDE
-	Use the Geany IDE to generate HTML pages
-	Use the Geany IDE to generate CSS stylesheets to format your HTML pages

## Acknowledgements

This lab is based on the "Project 3: HTML/CSS" project materials developed by [Lindsay K. Mattock](http://lindsaymattock.net/) for the the [SLIS 5020 Computing Foundations course](http://lindsaymattock.net/computingfoundations.html). 

# Table of Contents
- [Installing the Geany IDE](#installing-the-geany-ide)
- [What is HTML?](#what-is-html)
  * [Hello World!](#hello-world)
- [Creating an HTML File](#creating-an-html-file)
  * [Adding Content to `Index.html`](#adding-content-to-indexhtml)
- [Building Additional Web Pages](#building-additional-web-pages)
- [Creating Links in HTML](#creating-links-in-html)
- [Adding Images in HTML](#adding-images-in-html)
- [Using Cascading Style Sheets](#using-cascading-style-sheets-css)
  * [Creating and Implementing CSS](#creating-and-implementing-css)
- [Creating a Website](#creating-a-website)
- [Endnotes](#endnotes)
- [Lab Questions](#lab-questions)

# Installing the Geany IDE

1. We are going to install Geany at the command line. This will give you some more practice for a future lab when we build a server on our Pi.

2. Connect your Pi to the Internet either through Wi-Fi or the Ethernet cable. Open a Terminal session (If you don’t remember how, revisit the Project 1 instructions)

3. Install Geany IDE at the command line using `sudo apt-get install geany`. After the installation is complete you will find Geany in Menu > Programming

<blockquote>Geany documentation http://www.geany.org</blockquote>

<blockquote>Q1: How do you typically install new software on your computer? How is this process similar/different?</blockquote>

# What is HTML?

HTML stands for HyperText Markup Language

<em>“HyperText is the method by which you move around on the web — by clicking on special text called hyperlinks which bring you to the next page. The fact that it is hyper just means it is not linear — i.e. you can go to any place on the Internet whenever you want by clicking on links — there is no set order to do things in.

* "Markup is what HTML tags do to the text inside them. They mark it as a certain type of text (italicised text, for example).

* "HTML is a Language, as it has code-words and syntax like any other language.”</em><sup><a href="#fn1" id="ref1">1</a></sup>

HTML is all about sharing, storing, and accessing information. HTML provides the background for the World Wide Web.

## Hello World!

```HTML
<html>
<body>Hello World</body>
</html>
```

This is a very basic HTML document. The HTML tags `<HTML>` identify this document as a html document. The body tags `<body>` enclose the content that will be visible on the page.
   
4. Download the `hello_world.html` file and open it with the web browser on your Pi. You should see just the text “Hello World!” The browser has translated the HTML tags and returned only the text.

5. `helloworld.html` contains the minimum requirements for an HTML document. However, it is best practice to create a HTML document that is “well formed,” that is, that it follows all of the grammar, vocabulary, and syntax rules of html. 

6. We can check the well-formed-ness of this document in a validator like the W3C Markup Validation Service https://validator.w3.org. 

7. Click on “Validate by Direct Input” and copy and paste the code above into the validator and click `check`. You should receive a few errors. 
  
8. While our browser was able to interpret this code in the last project, this document does not follow all of the rules of the current version of HTML. HTML is pretty forgiving, but other languages are not, so it’s best to practice following all of the rules from the start.

<blockquote>Q2: Try to interpret a few of these errors in your own words. In particular, how would you explain the warnings related to character encoding?</blockquote>

# Creating an HTML File

9. Let’s make a few modifications to the Hello World file that will make it valid. Open Geany and open a new file from File > New (with Template). Select `file.html`. 

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_1.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_1.png?raw=true" /></a></p>

10. If you compare this blank template to the structure of an html document that you read about from the WC3 this week, you will find all of the required elements in this template. 

11. Geany has conveniently highlighted these different elements in different colors so that they can be easily distinguished as you build your html document.

12. The red at the top are comments indicated by the `<!-- and -->`. Comments are written for the user and not for the computer. 

13. These special start and end tags tell the computer to ignore what follows. Comments are used to include instructions and explanations about the code in a human-readable form. 

14. Feel free to use comments throughout your code to leave notes for yourself or describe what the code is doing (or what you want it to do).

15. Next, in green we have the document type declaration beginning with `<!DOCTYPE`. In this case, the document type is followed by html. This is simply telling the computer that what follows is a HTML document. 

16. The next piece, `-//W3C//DTD XHTML 1.0 Strict//EN` is the version declaration. 

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_2.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_2.png?raw=true" /></a></p>

17. In this case we are using XHTML. Learn more about the different versions of HTML: https://www.w3schools.com/html/html_intro.asp.

18. The final piece of this declaration is the URL for the DTD or Document Type Definition: http://www.w3.org/TR/xhtml1/dtds.html. 

19. This is the data structure or the rules for this version of HTML. Each version will have a different DTD defining the structure and all of the elements and attributes that can be used.

<blockquote>DTD for XHTML 1.0 http://www.w3.org/TR/xhtml1/dtds.html</blockquote>

20. Next we see the opening HTML tag, but there are a few additional attributes here: `<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">` 

21. This is just another piece of the XHTML specification. 

22. The namespace provides a means of disambiguation between elements with the same name. We won’t run into this issue in this lab. 

23. Also note here that the document language is declared as English with the `en` code with a standardized abbreviation for the English language.

<blockquote>XHTML 1.0 Documentation http://www.w3.org/TR/xhtml1/</blockquote>

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_3.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_3.png?raw=true" /></a></p>

24. What follows are the tags that define the structure of a basic HTML document as illustrated in the W3C reading this week.

25. Geany has constructed a blank template for us to work from. This html document is well- formed and valid. 

26. We can test this by copying and pasting our file into the HTML Validator. (Go ahead and give it a try https://validator.w3.org). 

27. This is one of the advantages to using and IDE for website development. As you will see in a few moments, Geany has a few other features that will help us to create clean, well-formed, and valid HTML documents.

# Adding Content to `Index.html`

28. At the moment, our document doesn’t have any content – let’s add some.  Between the `<head>` tags you will see a set of `<title>` tags. 

29. As the diagram illustrates, this data is not presented in the browser. This is true for the most part. 

30. The `<head>` of the document is reserved for metadata, but also includes the `<title>` of the page which is represented in the tabs in some web browsers. 

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_4.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_4.png?raw=true" /></a></p>

31. Replace “untitled” between the `<title>` tags to give your document a new title.

<blockquote>Q3: Between the head tags, there are also a few meta tags. Use the W3C site to translate this information in your notebook.</blockquote>
  
32. Now, let’s modify the body. This is where the content that we will see in the web browser is entered. 

33. HTML uses a number of different formatting tags. You can use the W3C site to browse through all of the different options. 

34. For now, we’ll use `<h1>` and `<p>`.

35. After the first `<body>` tag, place a `<h1>` tag on a new line. 

36. Notice two things:
  * The line is indented. This isn’t a requirement of HTML, but it is a convention that is used by coders to write cleaner code. The indentation allows you to easily determine what tags are nested within each other. For example, the `<title>` and `<meta>` tags are nested within the `<head>` tags. Now, our `<h1>` is nested within the `<body>`. The use of the tabs simply makes the code easier for us to read, but the computer doesn’t care (with Python the indentation is important and will cause errors if the indents do not appear in the right place).

  * Geany has completed your `<h1>` with a closing `</h1>` tag. The closing tag is not required for all HTML tags, but it is good practice to close all of your tags. This is a good example. Without a closing tag, everything that follows will be formatted as a `<h1>`. IDEs like Geany provide this function to help you prevent errors in your code and create valid documents.

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_5.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_5.jpg?raw=true" /></a></p>

37. Go ahead and enter some content between the `<h1>` tags. `<h1>` is preformatted as first level heading text. We’ll see how it looks in a minute. Next add a `<p>` tag and type some text. `<p>` tags are preformatted as paragraphs with padding between paragraphs.

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_6.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_6.jpg?raw=true" /></a></p>

38. Geany has another function that will be helpful as we develop our websites. Press F5 and your html document will display in the web browser.

39. At any time you can check the way that your code will render by pressing the F5 key. Go ahead and save the file by selecting Save As from the File menu. 

<blockquote>You can also press <code>Control + S</code> to save file updates.</blockquote>

40. Save the file in a dedicated new folder for this project, and call it `index.html.`

<blockquote>Why <code>index.html</code>? <code>index.html</code> is the name of the default landing page for websites. The web server (the computer hosing the site) will automatically recognize <code>index.html</code> as the first page or the home page of a website. Some servers use other variations like <code>home.html</code>, but we’ll use <code>index.html</code>.</blockquote>

# Building Additional Web Pages

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_7.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_7.jpg?raw=true" /></a></p>

41. What we have just created is a single web page. If we want to build a web site, we have to link this page to additional pages of content. 

42. Without closing the `index.html` file, let’s create a second file by clicking on down arrow next to the `+` icon in the upper left corner of the Geany window. 

43. Select `file.html`. Save this file as `page2.html` in the same folder where you have just saved `index.html`.

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_8.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_8.jpg?raw=true" /></a></p>

44. Now add some content to your second page. Be sure to add a title, `<h1>` and `<p>` tags. 

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_9.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_9.jpg?raw=true" /></a></p>

# Creating Links in HTML

45. Now, let’s add a link to the second page on our `index.html` page. 

46. We add links with the `<a href>` tag. This tag allows us to link pages in the same website and link out to pages that exist on external websites.

47. The tag syntax is as follows: `<a href=”URL to page”>`Text that you would like to appear`</a>`. 
  
48. Below your paragraph tag on the `index.html` page add the line `<a href=”page2.html”>Link to page 2</a>.`

Learn more about the `<a href>` tag at w3school: http://www.w3schools.com/TAGS/att_a_href.asp</blockquote>

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_10.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_10.png?raw=true" /></a></p>

49. Go ahead an open index.html by pressing F5 or opening it in your browser to see what our new link looks like. 

50. When you click on “Link to page 2” your `page2.html` file should open. In this case, our URL to the page in our `<a href>` tags is just the name of new page we created. 

51. We do not need a full URL (http://www.somewhere.com) because we are calling a file that is stored in the same directory on our server (the Pi). 

52. If we had saved this file to another folder or directory, we would put the file path here.

# Adding Images in HTML

53. Let’s add an image to the `index.html` page. Find an image that you like on the web and save it to the folder containing your two html documents on your Pi. 

54. The `<img>` tag is very similar to the `<a href>` tag that we just used. 

55. The tag has two required attributes `src` or the source and `alt` or the alternative text for the image. 

56. The `src` can be a local file or a URL to an image on the web, just like the href attribute in the `<a href>` tag. 

57. The `alt` is for the alternative text or the text that is displayed for the visually impaired or browsers like lynx that don’t support images. 

Learn more about the `<img>` tag at w3school:  http://www.w3schools.com/tags/tag_img.asp</blockquote>

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_11.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_11.jpg?raw=true" /></a></p>

58. On your `index.html` page, add the line `<img src=”imagefilename” alt=Description of image>`.

59. Be sure to use your image file name in place of the italicized text above. 

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_12.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_12.jpg?raw=true" /></a></p>

60. View the page in your browser to see if the image has loaded correctly.

<blockquote>Q4: Create another link to another HTML page or image, but save that file in a different directory or folder on your computer. How did you have to modify the HTML to call that file in your webpage? Why?</blockquote>
  
# Using Cascading Style Sheets (CSS)

If you read through the w3schools site, you will see that there is so much more that you can do with HTML. You will have an opportunity to explore on your own in a little bit. 

HTML allows us to add style to our pages internally, or inline. 

We’ve already styled our pages a bit using the `<h1>` tag. `<h1>` designates preformatted text that is larger than the `<p>` or paragraph text. But, what if we want to add color or change the font on our page? 

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_13.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_13.jpg?raw=true" /></a></p>

61. We can add style to each individual element within the page like so.

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_14.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_14.png?raw=true" /></a></p>

62. Here you can see that I’ve used the style attribute for the `<h1>` heading to change the text color to blue and center the text. 

63. I’ve used the same style attribute for the `<p>` to change the background color to powder blue and the font to courier. 

<blockquote>HTML Colors: http://www.w3schools.com/colors/default.asp</blockquote>
<blockquote>HTML Fonts: http://www.w3schools.com/css/css_font.asp</blockquote>

<blockquote>Q5: Take a look at the HTML Colors page listed above. Do you see anything familiar?</blockquote>

64. You can always add style in this matter, but if I want every heading to be blue and centered and every paragraph in courier font with a light blue background, then I need to add quite a bit of code every time I add a new page or element. 

65. Cascading Style Sheets (CSS) provides a more elegant way to add these style attributes across the pages in our site. 

66. As you saw in the demo in your reading (http://www.w3schools.com/css/css_intro.asp) you can take the same page content and change the look and feel with a new CSS. 

67. For those of you familiar with WordPress, this is how the various “themes” of the sites are managed. These are external CSS because they are files that are separate from the HTML pages. 

68. Let’s create a simple external CSS for our site. The CSS is cascading because there is a hierarchy to the way that styles are applied. If styles are defined within the document (as in the previous example), then they are applied before those in the stylesheet. 

69. In this way we can override the stylesheet if there is particular content that we would like to style differently.

## Creating and Implementing CSS

70. Open a new file in Geany. Geany doesn’t have a standard template for CSS, but will recognize the file as a CSS after we save the file with the extension. 

71. Open a new file and save it in the same folder as your other two `.html` files with the name `mystyle.css.`

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_15.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_15.png?raw=true" /></a></p>

72. The CSS file doesn’t contain any content, it only defines the styles for the various elements in HTML files. 

73. I’ve added a few simple styles for the background, `<h1>`, and `<p>`. Each tag is defined first `<body>`, `<h1>`, and `<p>` in this example. These are referred to as the selectors. 

74. Our style instructions for each tag are enclosed in `{ }`. These are called declarations. 

75. We can add as many style declarations as we would like in between the brackets, separating each with a semicolon. Each declaration has a property followed by a colon and then a value. 

76. It is common practice to place each declaration on a new line and to indent the declarations, but this is only to make the file easier for us to read and edit. The spacing has no impact on how the computer reads and interprets the code.

77. Now we need to link the CSS to our HTML files. This is called a reference. Each HTML page must reference the CSS to apply it to the page. We create this reference in the `<head>` of the HTML document with the other metadata. 

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_16.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_16.jpg?raw=true" /></a></p>

78. In the `<head>` of `index.html` add the reference `<link rel=”stylesheet” type=”text/css” href=”mystyle.css”>`.

79. This line can appear anywhere between the `<head>` and `</head>`. 

  * The `<link>` tag is another way to create links to other documents. 
  
  * In this case the `rel` attribute defines the relationship between the HTML file and the linking document. 

  * The `type` defines the type and `href` contains the URL or location reference for the file.

Learn more about the `<link rel>` tag at w3school: http://www.w3schools.com/tags/att_link_rel.asp

<p align="center"><a href="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_17.jpg?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/HTML-CSS/blob/master/images/Image_17.jpg?raw=true" /></a></p>

80. Open the `index.html` file in a browser to see the updated CSS.

81. However, if you click on the link to `page2.html`, it will look the same as it did before. This is because we need to link the stylesheet to each of the pages. 

82. Add the same `<link rel=”stylesheet” type=”text/css” href=”mystyle.css”>` to `page2.html`. 

83. Now both pages should share the same style.

# Creating a Website

84. Now, it’s time to build your own website. This lab has introduced you to the tools that you need, but feel free to expand on what you have learned using the w3schools site and whatever other resources you find on the web. 

85. We will continue building this website in a future lab on Python. For now, your site needs to fit a few minimum requirements.
  
86. First, the theme. Choose at least three media items—these can be books, articles, podcasts, films, songs, etc. Ideally, these three (or more) items will have something in common, but that connection is up to you.

87. Next, you are going to build a website about these items. 

88. You need to meet the following requirements:
  * You need a landing page (index.html) that describes the items and provides a brief introduction to your site. For example, if you are presenting books from your favorite author you could provide a brief into to the author here. It doesn’t need to be extensive, but you want to include some content. Your landing page should also include some logo or image.
  * The landing page (index.html) must also link to three different pages, one for each of the items you have chosen. Each of the item pages must include:
    * A short description of the item. You may pull this description from another source (publisher, archives, Wikipedia), just be sure to cite the source and link back to it if it is online.
    * A link to some related source on the web (Wikipedia, a book review or museum exhibit, for example) If you’ve pulled your description from another source, then the link to this source can serve as the link.
    * A representative image.
  * You also need a CSS for your site. The CSS will be used across all four pages of content to standardize the look and feel of your site.

89. That’s it. You are free to be as creative as you’d like as long as you meet these requirements.

90. I encourage you to use the w3schools pages as a guide for HTML (http://www.w3schools.com/html/) and CSS (http://www.w3schools.com/css/default.asp) as you design your site. 

91. You’ll find tutorials for menus, tables, and other elements to jazz up your site. Feel free to borrow code and CSS from anywhere on the web. Have fun and experiment!

92. Submit the HTML files and relevant CSS as as `.zip` folder on P-Web, along with your lab notebook.

<blockquote>Q6: Have you ever created a website before? Have you used a software like WordPress? How is this process different? Reflect on the process of creating a website by working directly with the HTML.</blockquote>

# Endnotes

<sup id="fn1">1. “What is HTML?” http://www.yourhtmlsource.com/starthere/whatishtml.html.<a href="#ref11" title="Jump back to footnote 1 in the text.">↩</a></sup>

# Lab Questions

All of the required questions are listed here. Be sure to answer each question completely, including an explanation of how you arrived at your answer. Also submit the HTML files and relevant CSS as a `.zip` folder on P-Web.

Q1: How do you typically install new software on your computer? How is this process similar/different?

Q2: Try to interpret a few of these errors in your own words. In particular, how would you explain the warnings related to character encoding?

Q3: Between the <head> tags, there are also a few <meta> tags. Use the W3C site to translate this information in your notebook.

Q4: Create another link to another HTML page or image, but save that file in a different directory or folder on your computer. How did you have to modify the HTML to call that file in your webpage? Why?
  
Q5: Take a look at the HTML Colors page listed above. Do you see anything familiar? Describe the way that RGB and Hexadecimal colors work in your own words.

Q6: Have you ever created a website before? Have you used a software like WordPress? How is this process different? Reflect on the process of creating a website by working directly with the HTML.
