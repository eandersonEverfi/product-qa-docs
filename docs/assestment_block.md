# Assessment Block - All at Once component 
> Test Set: [ALP-113](https://everfi.atlassian.net/browse/ALP-113)   
Type: Functional, Visual  

<!-- include: cypress/integration/assestment_block.js -->

### COM-1110 - assessment > assesment the user is able to select an "active" radio button

GIVEN: The assessment form block loads\
WHEN: The user selects a active radio button\
THEN: Then the selected radio button becomes active

waiting for the assessment form to completely load

clicking radio button 1/3

verifying that radiobutton 1/3 is indeed checked

verifying that the feedback message has a class of 'correct'

### COM-1110 - assessment > user is able to select a radio button and get its corresponding response feedback message

GIVEN: The assessment form block loads\
WHEN: The user clicks on a radio button\
THEN: The user gets its corresponding response feedback message

clicking CORRECT radio button 1/3

verifing CORRECT feedback container content

verifying feedback container has the expected class 'correct'

clicking INCORRECT radio button 2/3

verifing INCORRECT feedback container content

verifying feedback container has the expected class 'incorrect'

<!-- /include: cypress/integration/assestment_block.js -->