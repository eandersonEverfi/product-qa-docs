# Assessment Block One at a Time component 
> Dev Implementation ticket: [COM-2448](https://everfi.atlassian.net/browse/COM-2448)  
Type: Functional, Visual   

<!-- include: cypress/integration/blacksmith/assestment_block2.js -->

### COM-2448 - Assessment2 - User can select from options within a radio button form

GIVEN: The user loads the Assessment 2 component\
WHEN: The user selects a radio button from the form\
THEN: The selected radio button will be in a selected state\

Waiting for the main component  container to be visible

verifying the submit button is diabled by default

visual check -  Before selection - default view

waiting for the radio button options group to become visible

clicking radiobutton 1/3 and verifying that it gets a checked-state

verifying the submit button is not disabled

visual check -  After selection

### COM-2448 - Assessment2 - user gets all three question correct: Conclusion page correctly indicates this

GIVEN: The user loads the Assessment 2 component\
WHEN: The user selects all correct answers to each set of questions\
THEN: The user will get a passing score of 100 on the conclusion page

Waiting for the main component  container to be visible

verifying the submit button is diabled by default

waiting for the question label subhead to appear

verifying page subtitle

verifying page x of y counter

selecting radio 1of3

after submission of the form -- all form options should be disabled

the retry button is shown

feedback message for radio 1/3 produces the 'correct answer' feedback message

User is taken to page 2/3

need to do the cy.contains or the dom change will not be found on page navigation

verifying page subtitle

verifying page x of y counter

Selecting radio 2/3 then submitting the form

after submission of the form -- all form options should be disabled

the retry button is shown

feedback message for radio 2/3 produces the 'correct answer' feedback message

User is taken to page 3/3

verifying page subtitle

verifying page x of y counter

Selecting radio 1/3 then submitting the form

after submission of the form -- all form options should be disabled

the retry button is shown

the continue button is hidden on the last  page

feedback message for radio 1/3 produces the 'correct answer' feedback message

final feedback container is empty and not visible

final feedback container has class = perfect

final score = 100

visual check -  User gets the final feedback score = 100

### Assessment2 - user gets all three question incorrect: Conclusion page correctly indicates this

GIVEN: The user loads the Assessment 2 component\
WHEN: The user selects all incorrect answers to each set of questions\
THEN: The user will get a failing score of 0 on the conclusion page

verifying the submit button is diabled by default

verifying page subtitle

verifying page x of y counter

selecting radio 2/3

after submission of the form -- all form options should be disabled

the retry button is shown

feedback message for radio 2/3 produces the 'incorrect answer' feedback message

User is taken to page 2/3

need to do the cy.contains or the dom change will not be found on page navigation

verifying page subtitle

verifying page x of y counter

Selecting radio 2/3 then submitting the form

after submission of the form -- all form options should be disabled

the retry button is shown

feedback message for radio 1/3 produces the 'incorrectcorrect answer' feedback message

User is taken to page 3/3

verifying page subtitle

verifying page x of y counter

Selecting radio 2/3 then submitting the form

after submission of the form -- all form options should be disabled

the retry button is shown

the continue button is hidden on the last  page

feedback message for radio 2/3 produces the 'incorrect answer' feedback message

GIVEN:The user has gotten all three questions incorrect\
WHEN:The final results container loads\
THEN:There should be a list of three individual feedback messages\
THEN:Each of these feedback messages will be specific to the questions the user got incorrect

feedback results container has an array with 3 objects that contains feedback text as detailed

feedback message container has class = failed

final score = 0

visual check -  User gets the final feedback score = 0

### Assessment2 - user gets 2 out of 3 correct: Conclusion page correctly indicates this Conclusion page correctly indicates this

GIVEN: The user loads the Assessment 2 component\
WHEN: The user 2 out of 3 correct\
THEN: The user will get a failing score of `66.67` on the conclusion page

verifying the submit button is diabled by default

verifying page subtitle

verifying page x of y counter

selecting radio 1of3

after submission of the form -- all form options should be disabled

the retry button is shown

feedback message for radio 1/3 produces the 'correct answer' feedback message

User is taken to page 2/3

need to do the cy.contains or the dom change will not be found on page navigation

verifying page subtitle

verifying page x of y counter

Selecting radio 2/3 then submitting the form

after submission of the form -- all form options should be disabled

the retry button is shown

feedback message for radio 2/3 produces the 'correct answer' feedback message

User is taken to page 3/3

verifying page subtitle

verifying page x of y counter

Selecting radio 3/3 then submitting the form

after submission of the form -- all form options should be disabled

the retry button is shown

the continue button is hidden on the last  page

feedback message for radio 3/3 produces the 'incorrect answer' feedback message

GIVEN:The user has gotten 2 of 3 questions correct\
WHEN:The final results container loads\
THEN:There should be a list of 1 individual feedback messages\
THEN:Each of these feedback messages will be specific to the questions the user got incorrect

user final score

visual check - User gets the final feedback score = 66.67

### COM-5710- assessment2 > the user is able to retry their submitted option via a Retry button

GIVEN: The user has subbmited an assessment form option\
THEN: The user is presented with a RETRY button to allow the user to retry submitng the form again

On the Final Results page

Back on Page 1 of 3

<!-- /include: cypress/integration/blacksmith/assestment_block2.js -->