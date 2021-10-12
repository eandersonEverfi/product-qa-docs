# QA Feedback2 component
> Test Set: [ALP-130](https://everfi.atlassian.net/browse/ALP-130)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/qa_feedback2.js -->

### ALP 149

QA Feedback2 - the user is able to select an "active" radio button\
GIVEN- The QA Feedback2 component is loaded\
WHEN- A user clicks on an active radio button\
THEN- That clicked on radio button becomes active

waiting for defualt state of the component

visual check -  Before selecting the correct answer

user checks radio button 1/3

user verifies that radio button 1/3 is checked

### ALP 150

QA Feedback2 - user is able to select a radio button and get its corresponding response feedback message\
GIVEN- The QA Feedback2 component is loaded\
WHEN- The user clicks on a radio button\
THEN- The user gets that selected's corresponding feedback message

waiting for defualt state of the component

user checks radio button 1/3

user verifies that radio button 1/3 is checked

submit button enables when user checks an answer

feedback message contains expected text

qa feedback container has class 'correct'

qa feedback container has thumbs-up svg

visual check -  User sees Correct message after selecting first radio button

<!-- /include: cypress/integration/blacksmith/qa_feedback2.js -->