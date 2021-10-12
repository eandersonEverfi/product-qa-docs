# Rank component
> Test Set: [ALP-223](https://everfi.atlassian.net/browse/ALP-223)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/rank.js -->

### ALP-224 / ALP-226

Rank - mouse control - user is able to drag and snap an individual node-elements into a different node-slot and get feedback for sort order\
GIVEN- The 'click to submit' Rank component has loaded\
WHEN- When the user drags a node-elemet into different node-slots and clicks submit\
THEN- The user will get feedback for sort order

waiting for default component elements to load on the page

by default the 'check the order' button should not be disabled

visual check- 'click to submit' Rank component - Default View

user completes draging pieces in the 'correct' order and submits

post click - the 'check the order' button should now be disabled

user gets the sort feedback message indicating success on a correct-sort

visual check - 'click to submit' Rank component -  After Correct-sort

user manually refreshes the component page

user completes draging pieces in the 'incorrect' order and submits
Incorrect sort - in this order (top down)
Banana, Apple, Orange

post click - the 'check the order' button should not be disabled

user gets the sort feedback message indicating failure on a incorrect-sort

visual check - 'click to submit' Rank component -  After incorrect-sort

user moves the 'banana' piece to the correct drop zone and submits

The user now gets the  sort feedback message indicating success on a correct-sort

post click -
the 'check the order' button should now be disabled
the user gets the sort feedback message indicating success on a correct-sort

visual check -  'click to submit' Rank component - After correcting incorrect-sort

### COM-xx

mouse control - Auto-Submit with correct feedback\
GIVEN- The 'Auto submit' Rank component has loaded\
WHEN- the user drags a node-elemet into different node-slots\
THEN: The interactive will Auto submit\
THEN- The user will get feedback for sort order

waiting for default component elements to load on the page

visual check- Auto-Submit - Default view

user completes draging pieces in the 'correct' order

post sort
interactive auto-submits\
all 3 dragables get a check mark\
feedback message indicating a success is presented to the user

user gets the sort feedback message indicating success on a correct-sort

visual check- Auto-Submit - After Correct-sort

user manually refreshes the component page

user completes draging pieces in the 'incorrect' order
Incorrect sort - in this order (top down)
Apple, Orange, Banana

post sort -
interactive auto-submits\
only 'orange' gets a check mark\
sort feedback message is not shown\
only one check mark is visible

visual check - Auto-submit - Rank component -  After incorrect-sort

'Auto-Submit' - user fixes incorrect sourt

visual check -  'Auto-Submit' Rank component - After correcting incorrect-sort

<!-- /include: cypress/integration/blacksmith/rank.js -->