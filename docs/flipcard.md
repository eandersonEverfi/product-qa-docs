# Flipcard Component
> Test Set: [ALP-119](https://everfi.atlassian.net/browse/ALP-119)    
Type: Functional, Visual  

<!-- include: cypress/integration/blacksmith/flipcard.js -->

### ALP-210/ALP-211

flipcard > Component has a back and front-side, user can access each side via a click to the component to reveal the individual side's unique content\
GIVEN: The Filpcard component loads\
WHEN: A user cliks on a given flipcard\
THEN: The flipcard will respond by reversing to the opposite side of the flipcard, showing its unique content

### Default state, on load

verifying the front side

The flipcard is  marked in the DOM with a class of not being cliked yet

### Front of flipcard has text

"Font of flipcard"

verifying front flipcard image assets

visual check - front of card

clicking front of flipcard

post-click from default - card has class of 'flipped'

### Back of flipcard has text

'Back of flip card

verifying back flipcard image assets

visual check - back of card

clicking back of flipcard

### post-click - back of clipcard

Has class of 'clicked

user sees front of flipcard
Sees 'Front of flipcard' header text\

verifying front flipcard image assets

visual check of front of flipcard (second time)

<!-- /include: cypress/integration/blacksmith/flipcard.js -->