# Webpage Forms
* Forms provide a structured way to collect information from webpage visitors, such as a visitor’s first name, last name, address, email, and telephone number. 
* Visitors often complete webpage forms to register for an account or to make a purchase.
* A form consists of a starting `<form>` tag and an ending `</form>` tag. All form elements are contained with the `<form>` and `</form>` tags. 


## Form Controls (Input Controls)

* An **input control** is an interactive mechanism in which users enter text or make selections on a form.

* You define most controls in an HTML form by using the `type` attribute of the input element

```html
<form>
  <input type="text">
</form>
```

* Regardless of the specific type, each input control has attributes that are used more frequently than the others:
    * **name**, which identifies the specific information that is being sent when the form is submitted for processing. All controls have a name.
    * **id**, which provides a unique ID for the element. Use the id attribute to link a label element with an input control or other form element.
    * **value**, which specifies the value of an input element and varies depending on input type. 

## Labels
* A **label** is text describing the type of information to enter with an input control. 
* Form labels identify the type of information to enter into or select from an input control. You add a label to a form using the `label` element. 
* To connect a label to its control, include the `for` attribute with the same value as the input control’s `id` value. 

```html
<p>Choose your favorite Web language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```

## Input Type
* Note that all input should have a label for it. However, to keep this document concise, the labels are omitted.

### text 
* Creates a single-line field for text 
* You can use `maxlength` attribute for `text` input and another type of input to set the maximum length of the password.
```html
<input type="text" name="fName" id="fName">
<input type="text" name="uName" id="uName" maxlength=15>
```

### password 
* Creates a single-line field for a relatively small amount of text and masks the entered text as asterisks or bullets
```html
<input type="password" name="pw" id="pw">
<input type="password" name="pw" id="pw" maxlength=10>
```

### button
* Creates a button; typically used to run a script when clicked
```html
<input  type="button" 
        onclick="alert(‘Good Morning!’)"
        value="My Button">
```

### checkbox
* Creates a check box that the user can select one or many options
* To set a checkbox as the default, you use the `checked` attribute.
`<input>` tag
```html
<input type="checkbox" id="banana" name="fruit" value="banana" checked>
<label for="banana"> Banana </label>
<input type="checkbox" id="orange" name="fruit" value="orange">
<label for="orange"> Orange </label>
<input type="checkbox" id="lemon" name="fruit" value="lemon">
<label for="lemon"> Lemon </label>
```

### date
* Creates an input field used to contain a date; the field may appear as a date picker, depending on the browser.
```html
<input type="date" name="birthday">
```

### email
* An email control is a text box where visitors enter an email address. 
* Some browsers validate that the email address is in the proper format before submitting the form for processing. 
* If the email address is not in the proper format, the browser displays a message asking the user to correct the data.  
```html
<input type="email" name="email" id="email">
```

### file
* Creates a file-select field and a Browse button 
```html
<input type="file" name="doc">
```

### number 
* Creates an input field for a numeric value 
```html
<input type="number" name="cost">
```

### radio 
* Creates a radio button to allow the user to select one option 
```html
<input type="radio" id="AL" name="state" value="AL">
<label for="AL"> AL </label>
<input type="radio" id="AK" name="state" value="AK">
<label for="AK"> AK </label>
<input type="radio" id="AZ" name="state" value="AZ">
<label for="AZ"> AZ </label>
```

### range 
* Creates an input field for a value within a range; the field may appear as a slider control, depending on the browser
```html
<input type="range" name="survey" min="0" max="10">
```

### reset 
* Resets the form 
```html
<input type="reset" value="Reset Form">
```

### search 
* Creates an input field used as a search field 
```html
<input type="search" name="search">
```

### submit 
* Submits a form for processing 
```html
<input type="submit" value="Submit Form">
```

### tel 
* Creates an input field for a telephone number 
```html
<input type="tel" name="phone" id="phone">
```

### select
* A select control creates a selection menu from which the visitor makes one or more choices. 
* Instead of using the type attribute of the input element, you define a select control using the select and option elements. 
* You can also set a default option to be selected by default by adding the `selected` attribute to one of the `<option>` elements
```html
<select name="referral">
    <option>Advertisement</option>
    <option selected>Friend</option>
    <option>Google</option>
    <option>Social Media</option>
</select>
```


