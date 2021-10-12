# Carousel Component 
> Test Set: [ALP-115](https://everfi.atlassian.net/browse/ALP-115)     
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/carousel.js -->

### SMITH-25

Carousel (dark version) - provides navigation (Left/Right button) controls
to allow viewing of content on the individual carousel sides

GIVEN: The dark container carousel loads
WHEN: The user clicks on the LEFT or RIGHT carousel arrows
THEN: THE user see the Previous or Next slide in response

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

Carousel > Sync Slider - Learner can use the slider syncing navigation to
toggle between the slides on the main-slider to navigate both carousel slides.

GIVEN: The Sync-slider carousel loads
WHEN: The user clicks on smaller thumbnail sides
THEN: The user navigates to the respective synched main side

waiting for slide 1/4

waiting for DOM style attributes

Visual verification for slide 1/4
Main slide and respective sync-slide are lined up as expected\

clicking sync-slide 2/4

waiting for DOM style attributes

Visual verification for slide 2/4
Main slide and respective sync-slide are lined up as expected\

clicking sync-slide 3/4

waiting for DOM style attributes

Visual verification for slide 3/4
Main slide and respective sync-slide are lined up as expected\

clicking sync-slide 4/4

waiting for DOM style attributes

Visual verification for slide 4/4
Main slide and respective sync-slide are lined up as expected\

<!-- /include: cypress/integration/blacksmith/carousel.js -->