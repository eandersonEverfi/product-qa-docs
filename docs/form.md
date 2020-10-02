# Form Component
> Test Set: [ALP-120](https://everfi.atlassian.net/browse/ALP-120)    
Type: Functional, Visual  

<!-- include: cypress/integration/form.js -->

### ALP 149

form - the user is able to select an active radio button\
GIVEN: The Basic form with reset button component loads\
WHEN: A user clicks an 'active' radio button\
THEN: This radio button is selected

### ALP-156

form - with radio button forms the user is only able to select one option\
GIVEN: The Basic form with reset button component loads\
WHEN: The user first clicks on one active radio button\
AND: The user clicks on a second active radio button\
THEN: The first radio button deselects and the second radio button becomes selected

### ALP-157

form - with checkbox forms the user is able to select multiple options\
GIVEN: The Basic form with reset button component loads\
WHEN: The user first clicks on one active checkbox\
AND: The user clicks on a second active checkbox\
THEN: Both the first and second checkboxes stay selected

### ALP 158

form - the user is able to select an 'active' checkbox\
GIVEN: The Basic form with reset button component loads\
WHEN: A user clicks an 'active' checkbox\
THEN: This checkbox is selected

### ALP 159

form - the user is not able to select disabled elements\
GIVEN: The Basic form with reset button component loads\
WHEN: A deactivated radio button loads\
THEN: This radio button should have a diaabled class\

### ALP 178

form - required text fields - before submit the user must add input into the required text fields\
GIVEN: Basic form with feedback & reset button loads\
WHEN: A user does not fillout required fields with data\
THEN: These required fields will be flagged with a required message

### ALP 179

fields with initial values - there are fields that have by default are pre-populated  with text or numbers\
GIVEN: The Basic form with reset button component loads\
WHEN: The 'name' text field loads\
THEN: The user will see pre-populated text within this text field

### ALP 181

form - text field validation - Text field with minimum length (4 characters)\
GIVEN: The Basic form with reset button component loads - with the 'minimum length (4 characters)' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP 185

form - Select Dropdown - by default on viewing the select option element the user sees the default option selected\
GIVEN: The Basic form with reset button component loads\
WHEN: The user sees the select-dropdown field\
THEN: A default option is selected

### ALP 187

form - Select Dropdown - user can choose an option from the list by clicking on it\
GIVEN: The Basic form with reset button component loads\
WHEN: The user selects an option from the select-dropdown field\
THEN: The chosen option gets selected

### ALP 189

form - number field validation - Default number field -- this field is required by default, and must only numeric\
GIVEN: The Basic form with reset button component loads - with the 'Default number' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP 190

form - number field validation - Number field with value validation -- value must be between 5 and 10\
GIVEN: The Basic form with reset button component loads - with the 'Number field with value validation' field\
WHEN: The user add valid data into the filed\
THEN: The form will show no validation errors\
Otherwise - with invalid field data the user will be informed with a validation error message

### ALP-191

form - Number field with buttons - User can increment and decrease the field's data input value via PLUS and MINUS buttons\
GIVEN: The Basic form with reset button component loads - with the 'Number field with buttons' field\
WHEN: The user clicks on the provided PLUS and MINUS buttons\
THEN: The in-field data will respond (respectively) by incrementing or decreasing as in input value

### ALP-192

form - Number field with buttons - when the field has reached its max and min range the component will update its style to indicate the range limit has been reached\
GIVEN: The Basic form with reset button component loads - with the 'Number field with buttons' field\
WHEN: The field has reached its max and min range\
THEN: The component will update its style to indicate the range limit has been reached

### ALP-194

form - Rating field with icons - by default no stars are selected\
GIVEN: The Basic form with reset button component loads - with the 'Rating field with icons' field\
THEN: By default no stars are selected

### ALP-195

form - field validation - Rating field with icons -- This field is required\
GIVEN: The Basic form with reset button component loads - with the 'Rating field with icons' field\
WHEN: The user submits the form without at first adding data to this Rating field\
THEN: In response this Rating field will be marked with a Required validation error message

### ALP 246

form - User gets error message when required fields are not filled out\
GIVEN: Basic form with feedback & reset button loads\
WHEN: The user does not fill out all the required fields\
THEN: The form's respective fields are marked with a Required validation error message

### ALP 247

form - When the user fills out required field, no error message appears\
GIVEN: Basic form with feedback & reset button loads\
WHEN: The user fills out all the required fields\
THEN: The form's respective fields are void of any Required validaion error messages

### ALP 249

form - user leaves required field blank, then clicks reset\
GIVEN: Basic form with feedback & reset button loads\
WHEN: The user fills out all the required fields\
THEN: The form's respective fields are void of any Required validaion error messages

### ALP 248

form - user leaves required field blank, then clicks reset\
GIVEN: Basic form with feedback & reset button loads\
WHEN: The user leaves all fields blank\
THEN: On fie4lds with a default prepopulated value - this value persists after the form reset

### COM-xx

Form - After the user fills out all requied fields the user can submit the form and get a feedback message\
GIVEN: Basic form with feedback & reset button loads\
WHEN: A user initially submits the form without filling out required fields\
THEN: The skiped required fields will be marked with an error Required validation error message\
WHEN: The user then fills out all required fields with data\
THEN: The form submits - void of any error error Required validation error messages\
THEN: The form gets a Feedback message on successful form submit

<!-- /include: cypress/integration/form.js -->