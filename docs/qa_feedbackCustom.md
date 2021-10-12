# QA Feedback Custom block component
> Dev implemntation ticket: [COM-2450](https://everfi.atlassian.net/browse/COM-2450)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/qa_feedbackCustom.js -->

### COM-2450

QA Feedback Custom block - the user is able to select an "active" radio button\
GIVEN- The QA Feedback Custom Block component is loaded
WHEN- A user clicks on an active radio button\
THEN- That clicked on radio button becomes active

waiting for known state before snap

need to wait for radio form to be opaque or will get inconsistent snap results

visual check -  Before selecting the correct answer

clicking on radio button 1 of 3

radio button wrapper has the class of checked

visual check -  Radio Button was selected

### COM-2450

QA Feedback Custom block - user is able to select a radio button and get its corresponding response feedback message\
GIVEN- The QA Feedback Custom block is loaded\
WHEN- The user clicks on a radio button\
THEN- The user gets that selected's corresponding feedback message

waiting for known state before snap

the submit button is disabled by default

clicking on radio button 1 of 3

click submit button

Because the user submitted a Correct option - the Retry button does not exist

After submission of the form the SUBMIT button should be disabled

after submission of the form -- all form options should be disabled

the submit button is  disabled after submission of a correct answer

feedback message for radio 1/3 produces the correct feedback message

feedback message container has  thumbs-up svg

visual check -  User sees correct message after selecting first radio button

Reloading Page

clicking on radio button 3/3

waiting for known state before snap

click submit button

Because the user submitted an incorrect answer -- the RETRY button is presented to the user

The SUBMIT button should not exist

after submission of the form -- all form options should be disabled

the retry button is shown

the submit button is hidden

clicking radio 3/3 prduces the incorrect feedback message

feedback message container has  thumbs-down svg

visual check -  User sees incorrect message after selecting last radio button

### COM-5710- QA Feedback Custom block > when the user submits an incorrect option they are able to retry submission via a Retry button

GIVEN: The user has subbmited an incorrect assessment form option\
THEN: The user is presented with a RETRY button to allow the user to retry submitng the form again

<!-- /include: cypress/integration/blacksmith/qa_feedbackCustom.js -->