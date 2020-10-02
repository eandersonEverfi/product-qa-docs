# Inline Block Component
> Test Set: [ALP-124](https://everfi.atlassian.net/browse/ALP-124)    
Type: Functional, Visual  

<!-- include: cypress/integration/inline.js -->

### ALP-203

inline - Drawer Component: type \'top\' - Clicking the component button will add a drawer at the top of the browser window\
GIVEN: The inline Component loads\
WHEN: The user clicks on a drawer link\
THEN: A drawer is added at the top of the browser window

waiting for default view

visual check- default view

clicking the first drawer link

waiting for the expanded drawer header to be visible

waiting for the expanded drawer body content to be visible

visual check- expanded drawer

### ALP-207

inline - Drawer Component - clicking the \'X\' button causes the visible drawer to close\
GIVEN: The inline Component loads\
WHEN: The user clicks on the x-close button of an expanded drawer\
THEN: The expanded drawer closes

waiting for default view

visual check- default view

clicking on the first drawer link

waiting for the expanded drawer header to be visible

waiting for the expanded drawer body content to be visible

visual check- expanded drawer

clicking on the x-close button

post click of x-close button- drawer is not visible

visual check- post closing drawer - drawer is not visible

### ALP-129/ALP-144

inline - Popover windows are displayed when its link is clicked showing its content\
GIVEN: The inline Component loads\
WHEN: The user click on a popover link\
THEN: The user sees the popover expand

waiting for default view

visual check- default view

clicking the popover link

Post popover link click
Verify - popover link has a class of clicked\
verify - popover link now displays the popover

waiting for the position of the presented popover is in its final state before continuing with the test

visual check - post popover link click

### ALP-142

inline - clicking an open Popover causes the Popover to close its window\
GIVEN: The inline Component loads\
WHEN: The user clicks on the x-close button of an expanded popover\
THEN: The expanded popover will close

waiting for default view

clicking the popover link

Post popover link click
Verify - popover link has a class of clicked\
verify - popover link now displays the popover

waiting for the position of the presented popover is in its final state before continuing with the test

visual check - post popover link click

clicking the popover link on an expanded-state popover

post click - popover is not vidible

visual check - post click of popover x-close button - popover is not visible

### ALP-x1

inline - Typing into a text field the user should be able to see their entered text contained in this field\
GIVEN: The inline Component loads\
WHEN: The user types text into a text field\
THEN: The user will see that typed text within the text filed itself

waiting for default view

visual check- default view

User types text into the text field

verification - user sees the text they typed = within the text field itself

visual check post tying text into text field

<!-- /include: cypress/integration/inline.js -->