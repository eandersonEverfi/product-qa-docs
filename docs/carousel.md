# Carousel Component 
> Test Set: [ALP-115](https://everfi.atlassian.net/browse/ALP-115)     
Type: Functional, Visual

<!-- include: cypress/integration/carousel.js -->

### SMITH-25

Carousel - provides navigation (slide-dot button) control to allow viewing of content on the individual carousel sides\
GIVEN: The default carousel loads\
WHEN: The user clicks on individual slide-dot navigation elements\
THEN: The user is shown the respective slide-dot's slide

waiting for slide 1 text

clicking slide 2's slide-dot
User sees slide 2 in response\

clicking slide 3's slide-dot
user sees slide 3 in response\

clicking slide 1's slide-dot
User sees slide 1 in response\

### SMITH-25

Carousel - provides navigation (Left/Right button) controls to allow viewing of content on the individual carousel sides\
GIVEN: The default carousel loads
WHEN: The user clicks on the LEFT or RIGHT carousel arrows\
THEN: THE user see the Previous or Next slide in response

waiting for slide 1 text

waiting for the carousel's Prev and next burrons

prevBtn should not be visible
nextBtn should be visible\

visual check - use has switched to slide 2

After clicking the Next button
the previous button should be visible\
the next button should not be visible

visual check - use has switched to slide 3

Reversing direction tests

on silde 3
next button is not visible
previous button is visible\

click previous button

on silde 2
next button is visible
previous button is visible\

clicking the previous button

on silde 1
next button is visible
previous button is not visible\

### COM-1823

Carousel - provides navigation (keyboard) controls to allow viewing of content on the individual carousel sides\
GIVEN: The default carousel loads\
WHEN: The user clicked the right or left keys\
THEN: The system should respond by navigating the in the respective direction

waiting for slide 1 text

user cliks the right arrow key

user is navigated to slide 2

user cliks the right arrow key

user is navigated to slide 3

user cliks the left arrow key

user is navigated to slide 2

user cliks the left arrow key

user is navigated to slide 1

### COM-1823

Carousel > Sync Slider - Learner can use the slider syncing navigation to toggle between the slides on the main-slider to navigate both carousel slides.\
GIVEN: The Sync-slider carousel loads\
WHEN: The user clicks on smaller thumbnail sides\
THEN: The user navigates to the respective synched main side

waiting for slide 1/4

waiting for DOM style attributes

visual verification for slide 1/4
Main slide and respective sync-slide are lined up as expected\

clicking sync-slide 2/4

waiting for DOM style attributes

visual verification for slide 2/4
Main slide and respective sync-slide are lined up as expected\

clicking sync-slide 3/4

waiting for DOM style attributes

visual verification for slide 3/4
Main slide and respective sync-slide are lined up as expected\

clicking sync-slide 4/4

waiting for DOM style attributes

visual verification for slide 4/4
Main slide and respective sync-slide are lined up as expected\

<!-- /include: cypress/integration/carousel.js -->