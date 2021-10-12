# Quiz component
> Dev implemntation ticket: [COM-2819](https://everfi.atlassian.net/browse/COM-2819)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/quiz.js -->

clicking the Finish button

### COM-2819

Quiz - user gets all three question correct- Conclusion page correctly indicates this\
GIVEN- The Quiz component is presented to the user\
WHEN- The user selects the correct answer on all three pages\
THEN- The user gets a 100% passing grade on the conclusion page

user selects on each of the three quiz pages
page1- radio 1 --> correct
Page2- radio 2 --> correct
Page3- radio 1 --> correct

User is presented with the conclusion page with a perfect grade

visual check-  User gets a pefect feedback response (3 of 3 correct)

### COM-2819

GIVEN- The Quiz component is presented to the user\
WHEN- The user selects the incorrect answer on all three pages\
THEN- The user gets a 0% failing grade on the conclusion page

user selects on each of the three quiz pages
page1- radio 1 --> incorrect\
Page2- radio 2 --> incorrect\
Page3- radio 1 --> incorrect

User is presented with the conclusion page with a failing grade

visual check-  User gets a failed feedback response (0 of 3 correct)

GIVEN- The Quiz component is presented to the user
WHEN- The user answers the quiz with 1 out of 3 answers being correct\
THEN- The user gets a `33.33% failing grade on the conclusion page

user selects on each of the three quiz pages
page1- radio 1 --> correct
Page2- radio 2 --> incorrect
Page3- radio 1 --> incorrect

User is presented with the conclusion page with a failed grade

visual check-  User gets a failed feedback response (1 of 3 correct)

GIVEN- The Quiz component is loaded
WHEN- The user visits each page of the Quiz\
THEN- The individual Quiz pages are updated to indicate what page the user is on

verifying page subtitle

verifying page x of y counter

visual check -  Quiz page 1 of 3

going to page 2 of 3 by clicking radio button

verifying page subtitle

verifying page x of y counter

going to page 3 of 3 by clicking radio button

verifying page subtitle

verifying page x of y counter

<!-- /include: cypress/integration/blacksmith/quiz.js -->