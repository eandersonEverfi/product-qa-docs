# Assessment Block with All Correct Answers component 

> Test Set: [ALP-333](https://everfi.atlassian.net/browse/ALP-333)\
Type: Functional, Visual     

<!-- include: cypress/integration/blacksmith/assessment_block_with_all_correct_answers.js -->

### COM-1110

GIVEN: The assessment form block loads\
WHEN: The user selects an active radio button\
THEN: Then the selected radio button becomes active

waiting for radio button

waiting for the radio button form to be visible on the page

clicking radio button

verifying radio button is checked

waiting for the radio button form to be visible on the page

visual check -  After selecting radio button

### COM-1110

GIVEN: The assessment form block loads\
WHEN: The user clicks on a radio button\
WHEN: The user clicks on the submit button\
THEN: The user gets its corresponding response feedback message

waiting for radio button

clicking radio button

clicking the submit button

waiting for feedback message to be visible

waiting for feedback message to have the status of 'correct'

waiting for the svg thumbs-up

visual check -  User sees Correct message for radio

### Functional Check

\
ALP-149 > Assessment Block with All Correct Answers - user is able to select an "active" radio button

### Functional Check

\
ALP-150 > Assessment Block with All Correct Answers - user is able to select a radio button and get its corresponding feedback message

<!-- /include: cypress/integration/blacksmith/assessment_block_with_all_correct_answers.js -->