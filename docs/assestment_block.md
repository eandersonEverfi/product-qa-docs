# Assessment Block - All at Once component 
> Test Set: [ALP-113](https://everfi.atlassian.net/browse/ALP-113)   
Type: Functional, Visual  

<!-- include: cypress/integration/blacksmith/assestment_block.js -->

### COM-1110 - assessment > assesment the user is able to select an "active" radio button

GIVEN: The assessment form block loads\
WHEN: The user selects a active radio button\
THEN: Then the selected radio button becomes active

waiting for the assessment form to completely load

verifying the submit button is diabled by default

clicking radio button 1/3

verifying that radiobutton 1/3 is indeed checked

verifying the submit button is not disabled

after submission of the form -- all form options should be disabled

feedback message for radio 1/3 produces the 'correct answer' feedback message

verifying that the feedback message has a class of 'correct'

Since a correct answer option was selected, the Retry should not exist

waiting for the svg thumbs-up

### COM-1110 - assessment > user is able to select a radio button and get its corresponding response feedback message

GIVEN: The assessment form block loads\
WHEN: The user clicks on a radio button\
THEN: The user gets its corresponding response feedback message

verifying the submit button is diabled by default

clicking CORRECT radio button 1/3

verifying that radiobutton 1/3 is indeed checked

verifying the submit button is not disabled

after submission of the form -- all form options should be disabled

feedback message for radio 1/3 produces the 'correct answer' feedback message

verifying feedback container has the expected class 'correct'

verifying that radiobutton 2/3 is indeed checked

verifying the submit button is not disabled

after submission of the form -- all form options should be disabled

feedback message for radio 2/3 produces the 'incorrect answer' feedback message

verifying feedback container has the expected class 'incorrect'

Since an incorrect answer option was selected, the Retry should exist and be active

The SUBMIT button should not exist

### COM-5710- assessment > the user is able to retry their submitted option via a Retry button

GIVEN: The user has subbmited an assessment form option\
THEN: The user is presented with a RETRY button to allow the user to retry submitng the form again

<!-- /include: cypress/integration/blacksmith/assestment_block.js -->