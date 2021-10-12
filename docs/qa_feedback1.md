# QA Feedback1 component
> Dev implemntation ticket: [COM-1218](https://everfi.atlassian.net/browse/COM-1218)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/qa_feedback1.js -->

### COM-1218

QA Feedback1 - the user is able to select an "active" radio button\
GIVEN- The QA Feedback1 component is loaded\
WHEN- A user clicks on an active radio button\
THEN- That clicked on radio button becomes active

waiting for known state before snap

need to wait for radio form to be opaque or will get inconsistent snap results

visual check - Before selecting radio button

clicking on radio button 1 of 3

radio button wrapper has the class of checked

visual check -  Radio Button was selected

### COM-1218

QA Feedback1 - user is able to select a radio button and get its corresponding response feedback message\
GIVEN- The QA Feedback1 component is loaded\
WHEN- The user clicks on a radio button\
THEN- The user gets that selected's corresponding feedback message

waiting for known state before snap

clicking on radio button 1 of 3

submit button enables when user checks an answer

after submission of the form -- all form options should be disabled

on submit of a wrong option the retry button is shown

The SUBMIT button does not exist

feedback message for radio 1/3 produces the 'not correct' feedback message

visual check -  User sees 'incorrect message' feedback after selecting first radio button

user clicks the retry button

clicking on radio button 3/3

waiting for known state before snap

submit button enables when user checks an answer

after submission of the form -- all form options should be disabled

After form submit -- the SUBMIT button should be disabled

Because the user submitted a correct answer the RETRY button should not exist

clicking radio 3/3 produces 'correct' feedback message

need to wait for SVGs so they appear in snaps

visual check -  User sees 'correct message' feedback after selecting last radio button

<!-- /include: cypress/integration/blacksmith/qa_feedback1.js -->