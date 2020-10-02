# Horizontal-Scroll Component
> Test Set: [ALP-121](https://everfi.atlassian.net/browse/ALP-121)    
Type: Functional, Visual  

<!-- include: cypress/integration/horizontal_scroll.js -->

### ALP-212

horizontal scroll > Default Config - User is able to horizontally scroll within the component to see all of the embedded content\
GIVEN: The Default Config Horizontal Scroll component loads\
WHEN: The user engages a scrolling action with the mouse\
THEN: The component will allow the user to see all of the content within the scrollable area

Default Config
By default\
The right edge button will be visible\
The left edge button will be hidden

Visual check Default view of Default Config

user scrolls the Default Config version to the right

post scrolling to the right
The right edge button will be hidden\
The left edge button will be visible

Visual check Post right scrolling view of Default Config

### COM-xx

horizontal scroll > With Cards Config - User is able to horizontally scroll within the component to see all of the embedded content\
GIVEN: The with cards Horizontal Scroll component loads\
WHEN: The user engages a scrolling action with the mouse\
THEN: The component will allow the user to see all of the content within the scrollable area\
AND: User can interact with embdeed content within the scrollable area

With Cards version
By default\
The right edge button will be hidden\
The left edge button will be hidden

The ebedded content has cards that have the following copy
(1) Card Title\
(2) Learn More

Verification - there are a total of 4 cards within the scrollable area

Visual check Default view of With Cards version

user scrolls the With Cards version to the right

post scrolling to the right
The right edge button will be hidden\
The left edge button will be visible

Visual check Post right scrolling view of With Cards version

Scrolling the With Cards version to the left

post scrolling to the left
The right edge button will be visible\
The left edge button will be hidden

GIVEN:The user clicks a modal "Learn More" link
WHEN:The modal opens and become visible to the user\
THEN:The user can see a modal header and x-close button

visual verification of open modal - post clikcing the Learn More link

<!-- /include: cypress/integration/horizontal_scroll.js -->