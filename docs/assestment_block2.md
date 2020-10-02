# Assessment Block One at a Time component 
> Dev Implementation ticket: [COM-2448](https://everfi.atlassian.net/browse/COM-2448)  
Type: Functional, Visual   

<!-- include: cypress/integration/assestment_block2.js -->

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
THEN: The user will get incremental feedback about the correctness of their option choices on each assessment page\
THEN: The user will get a passing score of 100 on the conclusion page

Waiting for the main component  container to be visible

verifying the submit button is diabled by default

waiting for the question label subhead to appear

verifying page subtitle

verifying page x of y counter

selecting radio 1of3

User is taken to page 2/3 - score of submitted option is shown now

visual check -  User gets feedback from page 1/3 selection = correct

need to do the cy.contains or the dom change will not be found on page navigation

verifying page subtitle

verifying page x of y counter

Selecting radio 2/3 then submitting the form

User is taken to page 2/3 - score of submitted option is shown now

visual check -  User gets feedback from page 2/3 selection = correct

verifying page subtitle

verifying page x of y counter

Selecting radio 1/3 then submitting the form

On subit the user is shown their final score total

final feedback container is empty and not visible

final feedback container has class = perfect

final score = 100

visual check -  User gets the final feedback score = 100

### Assessment2 - user gets all three question incorrect: Conclusion page correctly indicates this

GIVEN: The user loads the Assessment 2 component\
WHEN: The user selects all incorrect answers to each set of questions\
THEN: The user will get incremental feedback about the correctness of their option choices on each assessment page\
THEN: The user will get a failing score of 0 on the conclusion page

verifying page subtitle

verifying page x of y counter

selecting radio 1of3

User is taken to page 2/3 - score of submitted option is shown now

visual check -  User gets feedback from page 1/3 selection = incorrect

need to do the cy.contains or the dom change will not be found on page navigation

verifying page subtitle

verifying page x of y counter

Selecting radio 2/3 then submitting the form

User is taken to page 2/3 - score of submitted option is shown now

visual check -  User gets feedback from page 2/3 selection = incorrect

verifying page subtitle

verifying page x of y counter

Selecting radio 1/3 then submitting the form

On submit the user is shown their final score total

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
THEN: The user will get incremental feedback about the correctness of their option choices on each assessment page\
THEN: The user will get a failing score of `66.66666666666666` on the conclusion page

verifying page subtitle

verifying page x of y counter

selecting radio 1of3

User is taken to page 2/3 - score of submitted option is shown now

visual check -  User gets feedback from page 1 of 3 selection = correct

need to do the cy.contains or the dom change will not be found on page navigation

verifying page subtitle

verifying page x of y counter

Selecting radio 2/3 then submitting the form

User is taken to page 2/3 - score of submitted option is shown now

visual check -  User gets feedback from page 2 of 3 selection = correct

verifying page subtitle

verifying page x of y counter

Selecting radio 1/3 then submitting the form

On submit the user is shown their final score total

GIVEN:The user has gotten 2 of 3 questions correct\
WHEN:The final results container loads\
THEN:There should be a list of 1 individual feedback messages\
THEN:Each of these feedback messages will be specific to the questions the user got incorrect

user final score

visual check - User gets the final feedback score = 66.66666666666666

<!-- /include: cypress/integration/assestment_block2.js -->