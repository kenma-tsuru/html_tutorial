# Image in HTML

* In this lesson, we'll review at how to use `<img>` in depth


## How do we put an image on a webpage?
* In order to put a simple image on a web page, we use the `<img>` element.
* This element requires two attributes to be useful: `src` and `alt`. 
* The `src` attribute contains a **URL** pointing to the image you want to embed in the page. The `src` attribute can be a *relative URL* or an *absolute URL*. 
  * An absolute URL contains the entire address from the protocol (HTTPS) to the domain name (www.example.com) such as http://www.example.com/xyz.html
  * The relative URL, on the other hand, does not use the full web address and only contains the location following the domain such as /xyz.html (xyz.html)
* If your image is called `dinosaur.jpg`, and it sits in the same directory as your HTML page, you could embed the image like so:

```html
<img src="dinosaur.jpg" alt="Dinosaur" />
```

* If the image was in an `images` subdirectory, which was inside the same directory as the HTML page, then you'd embed it like this:

```html
<img src="images/dinosaur.jpg" alt="Dinosaur" />
```

* You can also embedd the image using its absolute URL

```html
<img src="https://www.example.com/images/dinosaur.jpg" alt="Dinosaur" />
```

* Embedding the image using absolute URL is **not recommended**. You should host your own images. It is generally considered unethical, since someone else would be paying the bandwidth costs for delivering the image when someone visits your page. It also leaves you with no control over whether the image is removed or replaced with something embarrassing.

## Alternative text

* The `alt` attribute we'll look at is alt. Its value is supposed to be a textual description of the image, for use in situations where the image cannot be seen/displayed or takes a long time to render because of a slow internet connection.jpg

```html
<img
  src="images/dinosaur.jpg"
  alt="The head and torso of a dinosaur skeleton;
          it has a large head with long sharp teeth" />
```

* The reason why you would ever see or need alt text? It can come in handy for a number of reasons:
  * The user is visually impaired, and is using a screen reader to read the web out to them. 
  * The browser doesn't support the image type.
  * You may want to provide text for search engines to utilize
  * Users have turned off images to reduce data transfer volume and distractions.
