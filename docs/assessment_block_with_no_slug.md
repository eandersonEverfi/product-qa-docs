# Assessment Block with no Slug component 
> Test Set: [ALP-151](https://everfi.atlassian.net/browse/ALP-151)     
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/assessment_block_with_no_slug.js -->

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

### COM-2107 - assessment block no slug - user is able to select a radio button & Click on submit button and get its corresponding response feedback message

GIVEN: The assessment form block loads\
WHEN: The user clicks on a radio button and Click on submit button\
THEN: The user gets its corresponding response feedback message

waiting for radio button

clicking the CORRECT radio button

clicking the Submit button

Because the user submitted a Correct option - the Retry button does not exist

After submission of the form the SUBMIT button should be disabled

waiting for the feedback message container

waiting for the feedback message container's class to the expected state = 'correct'

waiting for the radio button form to be visible on the page

waiting for the svg thumbs-up

visual check -  User sees Correct message

clicking the INCORRECT radio button

waiting for the radio button form to be visible on the page

clicking the Submit button

Because the user submitted an incorrect answer -- the RETRY button is presented to the user

The SUBMIT button should not exist

waiting for the svg thumbs-down

visual check -  User sees 'incorrect' Message

### COM-5710- assessment block no slug > when the user submits an incorrect option they are able to retry submission via a Retry button

GIVEN: The user has subbmited an incorrect assessment form option\
THEN: The user is presented with a RETRY button to allow the user to retry submitng the form again

<!-- /include: cypress/integration/blacksmith/assessment_block_with_no_slug.js -->