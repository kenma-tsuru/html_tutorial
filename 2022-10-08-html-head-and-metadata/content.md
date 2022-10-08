# What is the HTML head?

- The head of an HTML document is the part that is not displayed in the web browser when the page is loaded.
- Web browsers (i.e. Chrome, Edge) use information contained in the head to render the HTML document correctly.

# Revisit Example

```html
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <title>My test page</title>
  </head>
  <body>
    <p>This is my page</p>
  </body>
</html>
```

- The HTML head is the contents of the `<head>` element. Unlike the contents of the `<body>` element, the head's content is not displayed on the page.
- Instead, the head's job is to contain **metadata** about the document

# `<title>` element

- The `<title>` element can be used to add a title to the document.

```html
<head>
  <meta charset="utf-8" />
  <title>My test page</title>
</head>
```

# `<meta>` element

- Metadata is data that describes data.
Go to https://www.analyticsvidhya.com/blog/2019/11/comprehensive-guide-attention-mechanism-deep-learning/ and use Inspection tool to see the example of metadata tag in real world

# Specifying your document's character encoding

- This element specifies the document's character encoding — the character set that the document is permitted to use.
- utf-8 is a universal character set that includes pretty much any character from any human language

```html
<head>
  <meta charset="utf-8" />
</head>
```

# Adding an author and description
* Many `<meta>` elements include name and content attributes.
* Two such meta elements that are useful to include on your page define the **author** of the page, and provide a **concise description** of the page.
* `name` specifies the type of meta element it is; what type of information it contains.
* `content` specifies the actual meta content.
* Specifying a _description_ that includes keywords relating to the content of your page is useful as it has the potential to make your page appear higher in relevant searches performed in search engines (such activities are termed Search Engine Optimization, or SEO.).

```html
<meta name="author" content="Chris Mills" />
<meta
  name="description"
  content="The MDN Web Docs Learning Area aims to provide
complete beginners to the Web with all they need to know to get
started with developing web sites and applications." />
```

# Adding custom icons to your site
* To further enrich your site design, you can add references to custom icons in your metadata, and these will be displayed in certain contexts. 
* The most commonly used of these is the **favicon** (short for "favorites icon", referring to its use in the "favorites" or "bookmarks" lists in browsers).
* A favicon can be added to your page by:
    * Saving it in the same directory as the site's index page, saved in .ico format
    * Adding the following line into your HTML's <head> block to reference it:
    ```html
    <link rel="icon" href="<path>/<filename>.ico" type="image/x-icon" />

    ```

# Applying CSS and JavaScript to HTML
* Just about all websites you'll use in the modern day will employ CSS to make them look cool, and JavaScript to power interactive functionality, such as video players, maps, games, and more. 
* These are most commonly applied to a web page using the `<link>` element and the `<script>` element, respectively.
* The `<link>` element should always go inside the head of your document. This takes two attributes, `rel="stylesheet"`, which indicates that it is the document's stylesheet, and href, which contains the path to the stylesheet file:
 ```html
<link rel="stylesheet" href="<path>/<filename>.css" />
 ```
 * The `<script>` element should also go into the head, and should include a `src` attribute containing the path to the JavaScript you want to load.
  ```html
<script src="<path>/<filename>.js"></script>
 ```