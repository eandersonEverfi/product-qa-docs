# Popover Component
> Test Set: [ALP-148](https://everfi.atlassian.net/browse/ALP-148)    
Type: Functional, Visual

<!-- include: cypress/integration/popover.js -->

### ALP 129

Popover - Popover windows are displayed when its link is clicked\
GIVEN- The Popover component has loaded\
WHEN- Popover component's link is clicked\
THEN- The Popover window of that clicked link is displayed revealing its unique content

waiting for the Top popover link loads

visual check - Default view -  User has not clicked the popover link

User clicks the Top Popover link

Post Click - Top popover link gets a class of 'clicked'

Post Click - Top Popover window presents itself

Expanded Top Popover window has the expected content

waiting for the position of the presented popover is in its final state before continuing with the test

visual check -  User sees the Top popover component's window expanded

### ALP 147

Popover - popovers with a button as trigger element\
GIVEN- The Popover component with a button as trigger element is loaded\
WHEN- The user clicks the button element\
THEN- The popover's window is in an expanded state

waiting for the Popover with button to load

visual check - default state -  User has not clicked on the popover button

user clicks the popover with button trigger

### post click of popover with button trigger results in

(1) popover button element gets a class of clicked\
(2) popover window is presented in an expanded-state\
(3) User sees the popover's unique content within the expanded window

waiting for the position of the presented popover is in its final state before continuing with the test

visual check -  User sees the Popover with button trigger window expanded

### ALP 142

Popover - Clicking an open Popover causes the Popover to close its window\
GIVEN- The Top popover is in an expanded state\
WHEN- The user clicks outside the confines of the popover's expanded window\
THEN- The expanded popover window will be in its closed-state

waiting for the Top popover component load

visual check - default state -  User has not clicked the Top popover link

### post click of Top Popover link results in

(1) popover link element gets a class of clicked\
(2) popover window is presented in an expanded-state\
(3) User sees the popover's unique content within the expanded window

waiting for the position of the presented popover is in its final state before continuing with the test

visual check -  User sees the Top Popover window expanded

user clicks outside the confines of the popover's expanded window

post click - popover window is not visible

visual check -  User clicks outside of the Top popover, and the popover window gets closed

<!-- /include: cypress/integration/popover.js -->