# Advanced text formatting

* The elements described in this section are less known, but still useful to know about (and this is still not a complete list by any means).
* Here you'll learn about marking up quotations, description lists, computer code and other related text, subscript and superscript, contact information, and more.

# Description lists
* The purpose of the description lists is to mark up a set of items and their associated descriptions, such as terms and definitions, or questions and answers. 
* Description lists use a different wrapper than the other list types `<dl>`; in addition each term is wrapped in a `<dt>` (description term) element, and each description is wrapped in a `<dd>` (description definition) element.

```html
<dl>
    <dt>Python</dt>
    <dd>This is the easiest programming language</dd>
    <dt>Rust</dt>
    <dd>This is the hardest programming language</dd>
</dl>
```
* It is permitted to have a single term with multiple descriptions

```html
<dl>
    <dt>Python</dt>
    <dd>This is the easiest programming language</dd>
    <dd> To say hello world `print("Hello World")` </dd>
    <dt>Rust</dt>
    <dd>This is the hardest programming language</dd>
    <dd> To say hello world `println!("Hello World")` </dd>
</dl>
```

# Blockquotes
* If a section of block level content (be it a paragraph, multiple paragraphs, a list, etc.) is quoted from somewhere else, you should wrap it inside a `<blockquote`> element to signify this, and include a URL pointing to the source of the quote inside a `cite` attribute.
```html
<blockquote cite="https://classic.set.or.th/en/regulations/simplified_regulations/dw_p1.html#:~:text=Definition,under%20the%20conditions%20provided%20therein"> Derivative Warrants (DW) refers to an instrument in which the issuer gives the holders the right to buy (Call Warrant) the underlying asset at the predetermined time or period of time, under the conditions provided therein</blockquote>
```

# Contact detail
HTML has an element for marking up contact details — _<address>_.
```html
<address>Chris Mills, Manchester, The Grim North, UK</address>
```

# Superscript and subscript
* We use `<sup>` to handle superscript, place the text above the line.
* We use `<sub>` to handle subcript, place the text under the line.

```html
<p>My birthday is on the 25<sup>th</sup> of May 2001.</p>
<p>
  Caffeine's chemical formula is
  C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>.
</p>
<p>If x<sup>2</sup> is 9, x must equal 3 or -3.</p>

```