# Progressive Disclosure component
> Dev implemntation ticket: [COM-2821](https://everfi.atlassian.net/browse/COM-2821)    
Type: Functional, Visual

<!-- include: cypress/integration/progressiveDisclosure.js -->

Default View - state 1

waiting for outer component container

waiting for SVG elements

Expecting all chat cards to be disabled besides - chat card #1

Execting Previous button to be disabled and Next button to be active

chart card 1 should be visiable with opacity = 1

state 2

waiting for outer component container

waiting for SVG elements

Navigating to page 2 by clickign the NEXT button

waiting for chat cards 1+2 to be visible

all other chat cards are hidden/not visible

state 3

waiting for outer component container

waiting for SVG elements

Navigating to page 3 by clickign the NEXT button - twice

waiting for chat cards 2+3 to be visible

all other chat cards are hidden/not visible

state 4

waiting for outer component container

waiting for SVG elements

Navigating to page 3 by clickign the NEXT button - three times

verifying button states

waiting for chat cards 3+4 to be visible

all other chat cards are hidden/not visible



clicking pervious button

on next page previous button is active

on page 3 of 4

clicking pervious button

on next page previous button is active

on page 2 of 4

clicking pervious button

on next page previous button is disabled

on page 1 of 4

waiting for page 1/1 to be in a known state

Default View - state 1

waiting for outer component container

waiting for SVG elements

Expecting all chat cards to be disabled besides - chat card #1

Execting Next button to be active and visible

chart card 1 should be visiable with opacity = 1

state 2

waiting for outer component container

waiting for SVG elements

Navigating to page 2 by clickign the NEXT button

waiting for chat cards 1+2 to be visible

Card #3 is invisible

state 3

waiting for outer component container

waiting for SVG elements

Navigating to page 3 by clickign the NEXT button - twice

need to wait to click on the NEXT button or will cause the button stay visible

bottom NEXT button is disabled and not visible

waiting for chat cards 1+2+3 to be visible

<!-- /include: cypress/integration/progressiveDisclosure.js -->