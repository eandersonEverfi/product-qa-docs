# QA Feedback Custom block component
> Dev implemntation ticket: [COM-2450](https://everfi.atlassian.net/browse/COM-2450)    
Type: Functional, Visual

<!-- include: cypress/integration/qa_feedbackCustom.js -->

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

clicking on radio button 1 of 3

feedback message for radio 1/3 produces the correct feedback message

feedback message container has  thumbs-up svg

visual check -  User sees correct message after selecting first radio button

clicking on radio button 3/3

waiting for known state before snap

clicking radio 3/3 prduces the incorrect feedback message

feedback message container has  thumbs-down svg

visual check -  User sees incorrect message after selecting last radio button

<!-- /include: cypress/integration/qa_feedbackCustom.js -->