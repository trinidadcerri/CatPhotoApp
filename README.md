# responsive-web-design-01

--- HTML5 THEORY: ---
                                      <element attribute="value">

Things I've learn in this challenge:


*COMMENTS IN HTML --> Commenting allows you to leave messages without affecting the browser display. It also allows you to make code inactive. A comment in HTML starts with <!--, contains any number of lines of text, and ends with -->.
   <!-- TODO: Remove h1 -->

*CONTENT AREAS --> HTML5 has some elements that identify different content areas. These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.
All pages should begin with <!DOCTYPE html>. This special string is known as a declaration and ensures the browser tries to meet industry-wide specifications.

<!DOCTYPE html>
<html>
  <head>
    <title>The title element determines what browsers show in the title bar or tab for the page.</title>
    <html lang="en">
    <meta charset="UTF-8">
  </head>
  <body>
    <main>
      <h1>CatPhotoApp</h1>
      <section>
        <h2>Cat Photos</h2>
        <!-- TODO: Add link to cat photos -->
        <p>See more cat photos in our gallery.</p>
      </section>
      <section>
        <h2>Cat Photos</h2>
        <!-- TODO: Add link to cat photos -->
        <p>See more cat photos in our gallery.</p>
      </section>
    </main>
    <footer>
    </footer>
  </body>
</html>

*NESTING AND INDENTATION --> All other elements must be descendants of this html element. All page content elements that should be rendered to the page go inside the body element.
Puts elements inside the main element. Nested elements should be placed two spaces further to the right of the element they are nested in. This spacing is called indentation and it is used to make HTML easier to read.
<main>
  <h1>CatPhotoApp</h1>
  <h2>Cat Photos</h2>
  <!-- TODO: Add link to cat photos -->
  <p>See more cat photos in our gallery.</p>
</main>

*H1-H6 HEADING ELEMENTS --> The h1 through h6 heading elements are used to signify the importance of content below them. The lower the number, the higher the importance, so h2 elements have less importance than h1 elements. Only use one h1 element per page and place lower importance headings below higher importance headings.
  <h1>Hello World</h1>
    <h2>Hello World</h2>
      <h3>Hello World</h3>
        <h4>Hello World</h4>
          <h5>Hello World</h5>
            <h6>Hello World</h6>

*P ELEMENT --> The p element is used to create a paragraph of text on websites.
  <p>Cat Photos</p>

*IMG ELEMENT (SELF-CLOSING TAG) --> You can add images to your website by using the img element. img elements have an opening tag without a closing tag. A tag for an element without a closing tag is known as a self-closing tag.
<img>

*HTML ATTRIBUTES --> are special words used inside the opening tag of an element to control the element's behavior.
When elements have multiple attributes, the order of the attributes doesn't matter.
*** SCR ATTRIBUTE: The src attribute in an img element specifies the image's URL (where the image is located).
  <img src="https://cdn.freecodecamp.org/platform/universal/fcc_secondary.svg">
*** ALT ATTRIBUTE: All img elements should have an alt attribute. The alt attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load.
  <img src="cat.jpg" alt="A cat">
*** TARGET ATTRIBUTE: a target attribute with the value _blank to the anchor (a) element's opening tag makes the link opens in a new tab.
  <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
*** HREF ATTRIBUTE: Other types of content can also be turned into a link by wrapping it in anchor tags: Turn the image into a link by surrounding it with necessary element tags.
  <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>

*ANCHOR (a) ELEMENT --> You can link to another page with the anchor (a) element. A link's text must be placed between the opening and closing tags of an anchor (a) element (turn the words into a link)
  <a href='https://freecodecamp.org'>link to cat pictures</a>
  OR inside a p tag
  <p>See more <a href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>

*LISTS:
***UNORDERED LIST
Within the ul element nest three list items. Use list item (li) elements to create items in a list.
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>

***ORDERED LIST
The code for an ordered list (ol) is similar to an unordered list, but list items in an ordered list are numbered when displayed.
<ol>
  <li>flea treatment</li>
  <li>thunder</li>
  <li>other cats</li>
</ol>

*FIGURE ELEMENT: represents self-contained content and will allow you to associate an image with a caption.
Nest an image within a figure element.
<figure>
  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
</figure>
**FIGCAPTION: A figure caption element is used to add a caption to describe the image contained within the figure element. For example,
<figcaption>A cute cat</figcaption>

*ELEMENTS FOR TEXT:
**EMPHASIZE --> wrapping something in an emphasis em element
<figcaption>Cats <em>love</em> lasagna.</figcaption>
**STRONG --> The strong element is used to indicate that some text is of strong importance or urgent.
<figcaption>Cats <strong>hate</strong> other cats.</figcaption>

*ADD A WEB FORM:
**FORM ELEMENT --> to get information from the user
  <form>
  </form>
**ACTION ATTRIBUTE --> The action attribute indicates where form data should be sent.
  <form action="/submit-url"></form> tells the browser that the form data should be sent to the path /submit-url.
**INPUT ELEMENT (SELF CLOSING)--> The input element allows you several ways to collect data from a web form. Like img elements, input elements are self-closing and do not need closing tags. Is nest within the form element
  <input>
**TYPE ATTRIBUTE --> There are many kinds of inputs you can create using the type attribute. You can easily create a password field, reset button, or a control to let users select a file from their computer. Example: a text field to get text input from a user by adding the type attribute with the value text to the input element:
  <input type="text">
**NAME ATTRIBUTE --> In order for a form's data to be accessed by the location specified in the action attribute, you must give the text field a name attribute and assign it a value to represent the data being submitted.
  <input type="text" name="email">
**PLACEHOLDER TEXT -->  is used to give people a hint about what kind of information to enter into an input.
  <input type="text" name="catphotourl" placeholder="cat photo URL">
**REQUIRED ATTRIBUTE --> To prevent a user from submitting your form when required information is missing, you need to add the required attribute to an input element. There's no need to set a value to the required attribute. Instead, just add the word required to the input element, making sure there is space between it and other attributes.
  <input type="text" name="catphotourl" placeholder="cat photo URL" required>
**BUTTON ELEMENT --> Use the button element to create a clickable button. For example, <button>Click Here</button> creates a button with the text Click Here. The default behavior of clicking a form button without any attributes submits the form to the location specified in the form's action attribute.
  <button>Submit</button>
**TYPE ATTRIBUTE --> since both input and button elements are inline elements, which don't appear on new lines. The button will submit the form by default. However, relying on default behavior may cause confusion. Has to add the type attribute with the value submit to the button to make it clear that it is a submit button.
  <button type="submit">Submit</button>
**LABEL ELEMENTS --> label elements are used to help associate the text for an input element with the input element itself (especially for assistive technologies like screen readers).
TYPE --> RADIO
Have to nest the radio type button inside a label element. For example:
Type radio are generally used in radio groups—collections of radio buttons describing a set of related options.
    Only one radio button in a given group can be selected at the same time. Radio buttons are typically rendered as small circles, which are filled or highlighted when selected. Notice that both radio buttons can be selected at the same time. To make it so selecting one radio button automatically deselects the other, both buttons must have a name attribute with the same value.
    *They are called radio buttons because they look and operate in a similar manner to the push buttons on old-fashioned radios, such as the one shown below. Checkboxes are similar to radio buttons, but with an important distinction: where multiple controls exist, radio buttons allow one to be selected out of them all, whereas checkboxes allow multiple values to be selected.
    <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
    <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
TYPE --> CHECKBOX
Forms commonly use checkboxes for questions that may have more than one answer. There's another way to associate an input element's text with the element itself. You can nest the text within a label element and add a for attribute with the same value as the input element's id attribute. Add the name attribute with the value personality to the checkbox input element. While you won't notice this in the browser, doing this makes it easier for a server to process your web form, especially when there are multiple checkboxes.
Like radio buttons, form data for selected checkboxes are name / value attribute pairs. While the value attribute is optional, it's best practice to include it with any checkboxes or radio buttons on the page.
    <input id="loving" type="checkbox" name="personality" value="loving"> <label for="loving">Loving</label>
    <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
    <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic"> Energetic</label>
**FIELDSET ELEMENT -->  is used to group related inputs and labels together in a web form. fieldset elements are block-level elements, meaning that they appear on a new line.
**LEGEND ELEMENT --> The legend element acts as a caption for the content in the fieldset element. It gives users context about what they should enter into that part of the form.
<fieldset>
  <legend>Is your cat an indoor or outdoor cat?</legend>
  <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
  <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
</fieldset>
<fieldset>
  <legend>What's your cat's personality?</legend>
  <input id="loving" type="checkbox" name="personality" value="loving"> <label for="loving">Loving</label>
  <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
  <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic"> Energetic</label>
</fieldset>
**CHECKED ATTRIBUTE --> In order to make a checkbox checked or radio button selected by default, you need to add the checked attribute to it. There's no need to set a value to the checked attribute. Instead, just add the word checked to the input element, making sure there is space between it and other attributes.
<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
<input id="loving" type="checkbox" name="personality" value="loving" checked> <label for="loving">Loving</label>

HTML FORM:
<section>
  <h2>Cat Form</h2>
  <form action="https://freecatphotoapp.com/submit-cat-photo">
    <fieldset>
      <legend>Is your cat an indoor or outdoor cat?</legend>
      <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
      <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
    </fieldset>
    <fieldset>
      <legend>What's your cat's personality?</legend>
      <input id="loving" type="checkbox" name="personality" value="loving" checked> <label for="loving">Loving</label>
      <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
      <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic">Energetic</label>
    </fieldset>
    <input type="text" name="catphotourl" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</section>

*ID ATTRIBUTE --> The id attribute is used to identify specific HTML elements. Each id attribute's value must be unique from all other id values for the entire page.
  <label><input id="indoor" type="radio"> Indoor</label>
