# Document and website structure

## Overview
*  This section looks into how to plan a basic website structure, and write the HTML to represent this structure.

## Basic sections of a document
* **header**: Usually a big strip across the top with a big heading, logo, and perhaps a tagline. This usually stays the same from one webpage to another.
* **navigation bar**: Links to the site's main sections; usually represented by menu buttons, links, or tabs.
* **main content**: A big area in the center that contains most of the unique content of a given webpage
* **sidebar**: Some peripheral info, links, quotes, ads, etc. Usually, this is contextual to what is contained in the main content (for example on a news article page, the sidebar might contain the author's bio, or links to related articles) but there are also cases where you'll find some recurring elements like a secondary navigation system.
* **footer**: A strip across the bottom of the page that generally contains fine print, copyright notices, or contact info. It's a place to put common information (like the header) but usually, that information is not critical or secondary to the website itself.
* Example: https://www.wsj.com/

## HTML for structuring content
* To implement such semantic mark up, HTML provides dedicated tags that you can use to represent such sections:
  * header: `<header>`.
  * navigation bar: `<nav>`.
  * main content: `<main>` and `<div>` elements.
  * sidebar: `<aside>`; often placed inside `<main>`.
  * footer: `<footer>`.
* Example: glassdor web clone

## Non-semantic wrappers
* Sometimes you'll come across a situation where you can't find an ideal semantic element to group some items together or wrap some content. Sometimes you might want to just group a set of elements together to affect them all as a single entity with some CSS or JavaScript. 
* For cases like these, HTML provides the `<div>` and `<span>` elements. You should use these preferably with a suitable class attribute, to provide some kind of label for them so they can be easily targeted.
* `<span>` is an inline non-semantic element, which you should only use if you can't think of a better semantic text element to wrap your content, or don't want to add any specific meaning.

```html
<p>
  The King walked drunkenly back to his room at 01:00, the beer doing nothing to
  aid him as he staggered through the door
  <span class="editor-note">
    [Editor's note: At this point in the play, the lights should be down low]
  </span>.
</p>

```

* `<div>` is a block level non-semantic element, which you should only use if you can't think of a better semantic block element to use, or don't want to add any specific meaning

```html
<div class="shopping-cart">
  <h2>Shopping cart</h2>
  <ul>
    <li>
      <p>
        <a href=""><strong>Silver earrings</strong></a>:
        $99.95.
      </p>
      <img src="../products/3333-0985/thumb.png" alt="Silver earrings" />
    </li>
    <li>…</li>
  </ul>
  <p>Total cost: $237.89</p>
</div>

```

<!-- end of today -->