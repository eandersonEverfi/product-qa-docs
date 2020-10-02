# Assessment Block with no Slug component 
> Test Set: [ALP-151](https://everfi.atlassian.net/browse/ALP-151)     
Type: Functional, Visual

<!-- include: cypress/integration/assessment_block_with_no_slug.js -->

### COM-2107

assessment block no slug - the user is able to select an "active" radio button\
GIVEN: The assessment form block loads\
WHEN: The user selects an active radio button\
THEN: Then the selected radio button becomes active

waiting for radio button

waiting for the radio button form to be visible on the page

visual check -  Before selecting the correct answer

clicking the CORRECT radio button

waiting for the radio button form to be visible on the page

visual check -  'Correct' Radio Button was selected

### COM-2107 - assessment block no slug - user is able to select a radio button and get its corresponding response feedback message

GIVEN: The assessment form block loads\
WHEN: The user clicks on a radio button\
THEN: The user gets its corresponding response feedback message

waiting for radio button

clicking the CORRECT radio button

waiting for the feedback message container

waiting for the feedback message container's class to the expected state = 'correct'

waiting for the radio button form to be visible on the page

waiting for the svg thumbs-up

visual check -  User sees Correct message

clicking the INCORRECT radio button

waiting for the radio button form to be visible on the page

waiting for the svg thumbs-down

visual check -  User sees 'incorrect' Message

<!-- /include: cypress/integration/assessment_block_with_no_slug.js -->