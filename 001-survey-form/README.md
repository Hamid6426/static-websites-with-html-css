# Build a Survey Form
## Objective
Build an app that is functionally similar to https://survey-form.freecodecamp.rocks. Do not copy this demo project.

## User Stories:
1. You should have a page title in an h1 element with an id of title
2. You should have a short explanation in a p element with an id of description
3. You should have a form element with an id of survey-form
4. Inside the form element, you are required to enter your name in an input field that has an id of name and a type of text
5. Inside the form element, you are required to enter your email in an input field that has an id of email
6. If you enter an email that is not formatted correctly, you will see an HTML5 validation error
7. Inside the form, you can enter a number in an input field that has an id of number
8. The number input should not accept non-numbers, either by preventing you from typing them or by showing an HTML5 validation error (depending on your browser).
9. If you enter numbers outside the range of the number input, which are defined by the min and max attributes, you will see an HTML5 validation error
10. For the name, email, and number input fields, you can see corresponding label elements in the form, that describe the purpose of each field with the following ids: id="name-label", id="email-label", and id="number-label"
11. For the name, email, and number input fields, you can see placeholder text that gives a description or instructions for each field
12. Inside the form element, you should have a select dropdown element with an id of dropdown and at least two options to choose from
13. Inside the form element, you can select an option from a group of at least two radio buttons that are grouped using the name attribute
14. Inside the form element, you can select several fields from a series of checkboxes, each of which must have a value attribute
15. Inside the form element, you are presented with a textarea for additional comments
16. Inside the form element, you are presented with a button with id of submit to submit all the inputs


<p id="description"><em>Thank you for taking the time to help us improve the certification</em></p>
    </div>
    <!--Survey form-->
    <div class="container">
            <label for="email" id="email-label">Email</label>
            <input type="email" id="email" name="email" required placeholder ="Enter your email">
            <label for="number" id="number-label">Age</label>
            <input type="number" id="number" name="number" min="1" max="130" placeholder ="Enter your age">
            <label for="dropdown">How satisfied are you with the overall structure of the certification program?</label>
            <select id="dropdown" name="dropdown">
                <option disabled selected="" value="">Select one of the options</option>
                <option value="incredible">☆☆☆</option>
                <option value="ok">☆☆</option>
                <option value="normal">☆</option>
                <option value="bad">Unsatisfied</option>
            </select>
            <div class="radio-check">
                <p>Would you reccommend this certification to your friend?</p>
                <label for="yes"><input type="radio" name="stay" id="yes" value="yes" checked>Yes</label>
                <label for="no"><input type="radio" name="stay" id="no" value="no">No</label>
                <label for="maybe"><input type="radio" name="stay" id="maybe" value="maybe">Maybe</label>
            </div>
            <div class="radio-check">
                <p>What did you learn the most? <span style="font-size: 15px;">(Check all that appy)</span></p>
                <label for="html"><input type="checkbox" name="Languages" id="html" value="html">HTML</label>
                <label for="css"><input type="checkbox" name="Languages" id="css" value="css">CSS</label>
                <label for="js"><input type="checkbox" name="Languages" id="js" value="js">JAVASCRIPT</label>
                <label for="bootstrap"><input type="checkbox" name="Languages" id="bootstrap" value="bootstrap">BOOTSTRAP</label>
                <label for="react"><input type="checkbox" name="Languages" id="react" value="react">REACT</label>
            </div>
            <div class="text-area">
                <label for="text-box">Do you have anything else that you would like us to know?</label>
                <textarea id="text-box" name="text-box" rows="6" placeholder="Tell us what you think!"></textarea>
            </div>
            <button id="submit" type="submit" form="survey-form" value="Submit">Submit</button>
        </form>
    </div>

    /* || RESPONSIVE */
@media only screen and (max-width: 768px) {
  .container {
      width: 80%;
      font-size: 17px;
  }
  input, select {
      font-size: 17px;
  }
  textarea  {
      font-size: 17px;
  }
  #submit {
      font-size: 17px;
  }
}