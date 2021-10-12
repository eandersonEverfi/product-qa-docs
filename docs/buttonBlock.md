# Button Block component 

> Test Set: [ALP-330](https://everfi.atlassian.net/browse/ALP-330)  
Type: Functional, Visual    

<!-- include: cypress/integration/blacksmith/buttonBlock.js -->

### button block - Rolling over the button produces a tooltip

GIVEN: The button with tool tip is loaded\
WHEN: The user rollls over the button\
THEN: The tooplip is presented to the user

visual check -  Default State

makes sure the  button with tooltip is centered verticall in the viewport

force = true prevent scrolling so the tippy is on the right side of the button

waiting for the position of the presented tooltip is in its final
state before continuing with the test

visual check -  After btn rollover

### button block - Clicking the Required button causese the Next button to activate

GIVEN: The Required Button is loaded
WHEN: The user clicks this Required Button\
THEN: A podal is presented\
THEN: The Next Button turns from the default state of `inactive` to an `active` state

waiting for and verifying the existance of the Required button

visual check -  Default state Required Button Container

visual check -  Default state Next Button

the default state of the Next button should be disabled

modal should present

visual check -  After clicking the Required button - modal appears

next button should now be in an `active` state

### button block - On click: Buttons can direct users to other internal pages or externial pages

GIVEN: The Buttons to Other Modules container loads\
WHEN: The user clicks on either of the two container buttons\
THEN: The user is taken to the respective button's expected URL

Button to Other Module container loads

### visual check -  Default State

Buttons to Other Modules

verifying that button 1 loads

click on button 1

user is taken to the expected page

user goes back to the BS2 Button Block page

verifying that button 2 loads

click on button 2

user is taken to the expected page

### button block - On click: buttons can show hidden content

GIVEN: The buttons can show hidden content container loads\
THEN: In the button's default state - the checkmark is hidden from view\
WHEN: The user clicks on the button\
THEN: Then a checkmark is presented to the user

Button Using Hide Until Clicked loads

button's checkmark is hidden - has class indicating it's non-clicked state

### visual check -  Default State

Button Using Hide Until Clicked

clicking button causes the checkmark to be visible and class indicates a clicked state

### visual check -  After Click State

Button Using Hide Until Clicked

<!-- /include: cypress/integration/blacksmith/buttonBlock.js -->