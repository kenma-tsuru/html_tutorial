# What is HTML?
* HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way.
# HTML elements
![image](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-small.png)
* Tags in HTML are not case-sensitive. This means they can be written in uppercase or lowercase. For example, a `<title>` tag could be written as `<title>`, `<TITLE>`, `<Title>`, `<TiTlE>`, etc., and it will work. However, it is best practice to write all tags in lowercase for consistency and readability.
## Example: creating your first HTML element
* Edit the line below by wrapping the word 'web' with the tags `<em>` and `</em>`. Doing this should give the line italic text formatting! See your changes update live in the Output area.
```text
I want to be a web developer
```

# Nesting HTML elements
* Give text:
```text
My cat is very grumpy
```
* If we wanted to state that our cat is very grumpy, we could wrap the word "very" in a `<strong>` element, which means that the word is to be strongly emphasized:
 ```html
 <p>My cat is <strong>very</strong> grumpy.</p>

 ```
 * The tags have to open and close in a way that **they are inside or outside one another**. If they overlap, then your web browser will try to make the best guess at what you were trying to say, which can lead to unexpected results.

 # Empty HTML elements
 * Some elements have no content and are called empty elements. 
 ```html
<img src="https://raw.githubusercontent.com/mdn/beginner-html-site/gh-pages/images/firefox-icon.png" alt="My test image" />
 ```

# HTML Attribute
![image](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-attribute-small.png)
* Attributes contain extra information about the element
*  The class attribute allows you to give the element a non-unique identifier that can be used to target it (and any other elements with the same class value) with style information and other things.
* An attribute should always have the following:
    1. A space between it and the element name (or the previous attribute, if the element already has one or more attributes).
    2. The attribute name followed by an equal sign.
    3. The attribute value wrapped by opening and closing quotation marks.
* Sometimes you will see attributes written **without values**. This is entirely acceptable. These are called Boolean attributes. 
```html
<!-- full version -->
<input type="text" disabled="disabled" />

<!-- short version which give the same output as above-->
<input type="text" disabled />
```
* You can choose sigle quote or double quote to wrap around the value.

 # HTML Document
 * Now we'll look at how individual elements are combined to form an entire HTML page.
 * First, create index.html and put this into it.
 ```html
 <!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width" />
    <title>My test page</title>
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="My test image" />
  </body>
</html>
 ```
* `<!DOCTYPE html>` basically just needed to make sure your document behaves correctly.
* `<html></html>` This element wraps all the content on the entire page and is sometimes known as the root element. It also includes the `lang ` attribute, setting the primary language of the document.
* `<head></head>` This element acts as a container for all the stuff you want to include on the HTML page that isn't the content you are showing to your page's viewers. This includes things like keywords and a page description that you want to appear in search results, CSS to style our content, character set declarations, and more.
* `<meta charset="utf-8">` This element sets the character set your document should use to UTF-8 which includes most characters from the vast majority of written languages.
* `<meta name="viewport" content="width=device-width">` — This viewport element ensures the page renders at the width of viewport, preventing mobile browsers from rendering pages wider than the viewport and then shrinking them down.
* `<title></title>` This sets the title of your page, which is the title that appears in the browser tab the page is loaded in
* `<body></body>` This contains all the content that you want to show to web users when they visit your page, whether that's text, images, videos, games, playable audio tracks, or whatever else.

# HTML comments
* The purpose of comments is to allow you to include notes in the code to explain your logic or coding. 
* To write an HTML comment, wrap it in the special markers `<!-- and -->`
```html
<!-- <p>I am inside the comment</p> -->
```
