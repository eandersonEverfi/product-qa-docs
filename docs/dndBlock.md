# Drag and Drop Block component
> Test Set: [ALP-286](https://everfi.atlassian.net/browse/ALP-286)    
Type: Functional, Visual  

<!-- include: cypress/integration/dndBlock.js -->

reusable function to first select a dragable and then dropping it into a drop zone

DnD1 - passing scenario
apple - drag to fruit drop zone\
pumpkin - drag to fruit drop zone\
carrot - drag to veg drop zone\
lemon - drag to fruit drop zone\
hot pepper - drag to fruit drop zone

DnD1 - failing scenario
apple - drag to veg drop zone\
pumpkin - drag to fruit drop zone\
carrot - drag to fruit drop zone\
lemon - drag to fruit drop zone\
hot pepper - drag to fruit drop zone

DnD2 - passing scenario
apple - drag to fruit drop zone\
pumpkin - drag to fruit drop zone\
carrot - drag to veg drop zone\
lemon - drag to fruit drop zone\
hot pepper - drag to fruit drop zone

DnD2 - failing scenario
apple - drag to fruit drop zone\
pumpkin - drag to fruit drop zone\
carrot - drag to fruit drop zone\
lemon - drag to fruit drop zone\
hot pepper - drag to fruit drop zone

### COM-x1

DnD block - User can drag 'draggables' options to predefined drop zones\

viz check  - Before sort

viz check - After sort

verifying - fruit drop zone has 4 dragables

verifying - veg drop zone has 1 dragable

### COM-x2

DnD block - User can get system feedback of the correctness of the user’s sorting by clicking the submit button\
GIVEN: The DnD with Submit component loads\
WHEN: The user selects and drags a dragable to a drop zone\
THEN: The selected dragable is dropped onto this specified drop zone\

waiting for dragables to be in view

verifying by default there are 5 dragable options in the options container

viz check - Before sort

running the DnD1 passing scenario

GIVEN:The user has run the DnD1 passing scenario\
WHEN:The user clicks the submit button\
THEN:the following conditions occur\

The feedback message text contains - 'Correct'

viz check - After submit - correct

reloading the component page and waiting for DnD1's dragable options

running the DnD1 failing scenario

GIVEN:The user has run the DnD1 failing scenario\
WHEN:The user clicks the submit button\
THEN:the following conditions occur\

The feedback message text contains -  'incorrect'

viz check - After submit - Incorrect

### COM-x3

DnD block - User can click the start over button to reset the interactive\
GIVEN: The DnD with Submit component loads\
WHEN: The user has already dragged some options to the drop zones\
THEN: The user can click the Reset button to reset the DnD1 component to its default state\
THEN: After clicking the Reset button\
THEN: User sees DnD1 component in its default configuration state

viz check - Before sort

running the Passing scenario

Post running - verifying by default there are 0 dragable options in the options container

viz check - Before Reset

After the Passing scenario compeltes the user clicks the Reset button
Then the draggables will be moved back to their default position\

Post reset -verifying by default there are 5 dragable options in the options container

viz check - After Reset

### COM-2902

DnD block - Instant Feedback - User gets system feedback of the correctness of the user’s sorting as soon as they complete the drag\
GIVEN: The DnD Instant Feedback component is loaded\
WHEN: The user moves a draggable option to a drop zone\
THEN: The user will get instant feedback on the correctness of this sorted/dragged action

wating for the default state

Verifying The 'Start over' button is disbaled, by default

moving the Apple dragable to the correct (fruit) drop zone

post drag
Verifying - Instant feedback is given\
Feedback contains "Correct" + "An apple is a fruit!"

Verifying The 'Start over' button is NOT disbaled, by default

moving the Apple dragable to the incorrect (veg) drop zone

post drag
Verifying - Instant feedback is given
Feedback contains "Incorrect" + "While all fruits are technically vegetables, that's not what we're after here."\

Verifying The 'Start over' button is NOT disbaled, by default

repositioning Apple to the 'correct' (fruit) drop zone

Verifying The 'Start over' button is NOT disbaled, by default

post drag
Verifying - Instant feedback is given\
Feedback contains "Correct" + 'An apple is a fruit!'

moving the Pumpkin dragable to the correct (fruit) drop zone

post drag
Verifying - Instant feedback is given\
Feedback contains "Correct" + 'A pumpkin is a fruit!'

Verifying The 'Start over' button is NOT disbaled, by default

### COM-2902

DnD block - Instant Feedback - Testing 'Correct' end-feedback state\
GIVEN: The DnD Instant Feedback component is loaded\
WHEN: The user drags all dragable options to the 'correct' state locations\
THEN: The end-state has the 'start over' button as disabled

verifying the default state

Options container has a total of 5 options

Default state has the 'start over' button as NOT disabled

Running the DnD2 passing state

### Post correct-state verification



Options container has 0 options

Fruit drop zone has 4 options

Veg drop zone has 1 options

### post correct-state

'Start over' button IS disabled

### COM-2902

DnD block - Instant Feedback - Testing 'incorrect' end-feedback state\
GIVEN: The DnD Instant Feedback component is loaded\
WHEN: The user drags all dragable options to the 'incorrect' state locations\
THEN: The end-state has the 'start over' button as NOT disabled

verifying the default state

Options container has a total of 5 options

Default state has the 'start over' button as NOT disabled

Running the DnD2 passing state

Options container has 0 options

Fruit drop zone has 5 options

Veg drop zone has 0 options

### post incorrect-state

'Start over' button IS disabled

<!-- /include: cypress/integration/dndBlock.js -->