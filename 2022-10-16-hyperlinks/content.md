# What is a hyperlink?
* Hyperlinks allow us to link documents to other documents or resources, link to specific parts of documents.

# Anatomy of a link
* A basic link is created by wrapping the text or other content inside an `<a>` element and using the `href` attribute, also known as a **Hypertext Reference**, or target, that contains the web address.

```html
<p>
  I'm creating a link to
  <a href="https://www.mozilla.org/en-US/">the Mozilla homepage</a>.
</p>
```

# Adding supporting information with the `title` attribute
*  The title contains additional information about the link, such as which kind of information the page contains, or things to be aware of on the website.
*  This gives us the hovering over the link displays the title as a tooltip

```html
<p>
  I'm creating a link to
  <a
    href="https://www.mozilla.org/en-US/"
    title="The best place to find more information about Mozilla's
          mission and how to contribute">the Mozilla homepage</a>.
</p>
```

# Block level links
* If you have an image you want to make into a link, use the `<a>` element and reference the image file with the `<img>` element.
```html
<a href="https://www.youtube.com/">
  <img src="img/youtube-logo.png" alt="Youtube" />
</a>
```

# A quick primer on URLs and paths
* A URL, or Uniform Resource Locator is a string of text that defines where something is located on the Web.
* If you wanted to include a hyperlink inside index.html (the top level index.html) pointing to contacts.html, you would specify the filename that you want to link to, because it's in the same directory as the current file.

```html
<p>
  Want to contact a specific staff member? Find details on our
  <a href="contacts.html">contacts page</a>.
</p>
```
* If you wanted to include a hyperlink inside index.html pointing to projects/index.html, you would need to go down into the projects directory before indicating the file you want to link to. This is done by specifying the directory's name, then a forward slash, then the name of the file.

```html
<p>Visit my <a href="projects/index.html">project homepage</a>.</p>
```

# Document fragments
* It's possible to link to a specific part of an HTML document, known as a **document fragment**. To do this you first have to assign an id attribute to the element you want to link to.
* Then to link to that specific id, you'd include it at the end of the URL, preceded by a hash/pound symbol (`#`)

```html
<h2 id="Mailing_address">Mailing address</h2>
```
```html
<p>
  Want to write us a letter? Use our
  <a href="contacts.html#Mailing_address">mailing address</a>.
</p>
```

* You can even use the document fragment reference on its own to link to another part of the current document

```html
<p>
  The <a href="#Mailing_address">company mailing address</a> can be found at the
  bottom of this page.
</p>
```

# Use the download attribute when linking to a download
* When you are linking to a resource that's to be downloaded rather than opened in the browser, you can use the download attribute.
* The download attribute can have a value to provide a default save filename
```html
<a
  href="https://download.mozilla.org/?product=firefox-latest-ssl&os=win64&lang=en-US"
  download>
  Download Latest Firefox for Windows (64-bit) (English, US)
</a>
```
```html
<a
  href="https://download.mozilla.org/?product=firefox-latest-ssl&os=win64&lang=en-US"
  download="firefox-latest-64bit-installer.exe">
  Download Latest Firefox for Windows (64-bit) (English, US)
</a>
```

