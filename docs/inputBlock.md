# Input Block Component
> Test Set: [ALP-125](https://everfi.atlassian.net/browse/ALP-125)    
Type: Functional, Visual  

<!-- include: cypress/integration/inputBlock.js -->

### ALP-149

input - the user is able to select an \'active\' radio button\
GIVEN: The Field/input Block component loads\
WHEN: The user sees an active radio button\
THEN: The user is able to select this radio button by clicning on it

waiting for the 'Radio button' form
Verifying none of the radio buttons are in a deactived state\

clicking on radio button 1

radio button 1 becomes selected

visual check - user sees radio 1 checked

clicking on radio button 2

radio button 2 becomes selected

visual check - user sees radio 2 checked

clicking on radio button 3

radio button 3 becomes selected

visual check - user sees radio 3 checked

### ALP-156

input - with radio button forms the user is only able to select one option\
GIVEN: The Field/input Block component loads\
WHEN: The user first clicks on one active radio button\
AND: The user clicks on a second active radio button\
THEN: The first radio button deselects and the second radio button becomes selected

waiting for the 'Radio button' form
Verifying none of the radio buttons are in a deactived state\

clicking on radio button 1

radio button 1 becomes selected

visual check -  User sees ONLY radio1 checked

clicking on radio button 2

radio button 2 becomes selected

visual check -  User sees ONLY radio2 checked

### ALP-157

input - with checkbox forms the user is able to select multiple options\
GIVEN: The 'Checkbox' form loads\
WHEN: The user first clicks on one active checkbox\
AND: The user clicks on a second active checkbox\
THEN: Both the first and second checkboxes stay selected

### ALP-158/ALP-159

input - the user is able to select an \'active\' checkbox. Cant select diabled checkboxes\
GIVEN: The 'checkbox' form loads\
WHEN: A user clicks an 'active' checkbox\
THEN: This checkbox is selected\
WHEN: A user clicks a 'disabled' checkbox\
THEN: This 'disabled' checkbox is NOT selected

### ALP-160/ALP-159

input - the user is able to select \'active\' buttons. Cant select disabled buttons\
GIVEN: The 'Radio button' form loads\
WHEN: A user clicks on a inactive button\
THEN: Post-click this clicked on button will NOT gain focus

### ALP-161

input - the user is able to select multiple buttons at once\
GIVEN: The 'Radio button' form loads\
WHEN: A user clicks multiple buttons, within the same form\
THEN: These multiple clicked on buttons will have gained focus

### ALP-179

input - there are fields that have by default are pre-populated with text or numbers\
GIVEN: The 'input Feild' forms load\
WHEN: The user sees the 'Text field with initial value' form\
THEN: The user will see a given pre-populated text within this form

### ALP-182

input - Text field with minimum & maximum length validation (2 characters minimum, 6 characters maximum)\
GIVEN: The 'Input Field' forms load - with the 'Text field with minimun & maximum length validation' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP-180

input - Text field with minimum length (2 or more characters required)\
GIVEN: The 'Input Field' forms load - with the 'Text field with minimun length validation' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP-183

input - Text field with Regex validation (must start with letter A in uppercase)\
GIVEN: The 'Input Field' forms load - with the 'Text field with Regex validation' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP-184

input - Field with multiple validations and errors display (must start with letter A in uppercase, 2 characters minimum, 6 characters maximum.)\
GIVEN: The 'Input Field' forms load - with the 'Field with multiple validations and errors display' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP-184

input - Default number field -- this field is required by default, and must only numeric\
GIVEN: The 'Number Input' forms load - with the 'Default number field' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP-190

input - Number field with value validation value must be between 5 and 10\
GIVEN: The 'Number Input' forms load - with the 'Number field with value validation' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP-190

input - Number field with buttons -- value must be between 5 and 10\
GIVEN: The 'Number Input' forms load - with the 'Number field with buttons + value validation' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP-192/APL-191

input - when the field has reached its max and min range the component will update its style to indicate the range limit has been reached\
GIVEN: The 'Number Input' forms loads - with the 'Number field with buttons' field\
WHEN: The field has reached its max and min range\
THEN: The component will update its style to indicate the range limit has been reached

### ALP 185

input - Select option input - by default on viewing the select option element the user sees the default option selected\
GIVEN: The 'Select option input' component loads\
WHEN: The user sees the select-dropdown field\
THEN: A default option is selected

### ALP-186/ALP-187

input - Select option input - clicking causes the component to expand, reveling all options available / user can select specific options from the menu\
GIVEN: The 'Select option input' component loads\
WHEN: The user selects an option from the select-dropdown field\
THEN: The chosen option gets selected

<!-- /include: cypress/integration/inputBlock.js -->