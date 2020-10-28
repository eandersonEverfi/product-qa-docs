# Progressive Disclosure component
> Dev implemntation ticket: [COM-2821](https://everfi.atlassian.net/browse/COM-2821)    
Type: Functional, Visual

<!-- include: cypress/integration/progressiveDisclosure.js -->

### COM-2821

progressive Disclosure - Top - Verifying view #1 state\
GIVEN- The 'top' progressive disclosure component loads\
WHEN- The user visits the component page for the first time\
THEN- The user will be presented with the top component's default view state - page 1

Default View - state 1

waiting for outer component container

waiting for SVG elements

Expecting all chat bubble-cards to be disabled/hidden from view -  besides for the chat bubble-card 1

Expecting 'Top' Previous button to be disabled and Next button to be active

chart bubble-card 1 should be visiable with opacity = 1

visual check - Top -  State 1/Default view -page 1

### COM-2821

progressive Disclosure - Top - Verifying view #2 state\
GIVEN- The 'top' progressive disclosure component loads\
WHEN- The user clicks on the 'top' NEXT button
THEN- The user will be presented with the 'top' #2 state view - page 2

state 2 - User has clicked the NEXT button to get to page 2

waiting for outer component container

waiting for SVG elements

Navigating to page 2 by clickign the NEXT button

NEXT button is NOT disabled

waiting for chat cards 1+2 to be visible

all other chat cards are hidden/not visible

visual check -  Top -  State 2 - page 2

### COM-2821

progressive Disclosure - Top - Verifying view #3 state\
GIVEN- The 'top' progressive disclosure component loads\
WHEN- The user clicks on the 'top' NEXT button twice (to get to page 3)
THEN- The user will be presented with the 'top' #3 state view - page 3

state 3 - User has clicked the NEXT button twice to get to page 3

waiting for outer component container

waiting for SVG elements

Navigating to page 3 by clicking the NEXT button - twice

NEXT button for both clicks should NOT be disabled

waiting for chat cards 2+3 to be visible

all other chat cards are hidden/not visible

visual check -  Top -  State 3 - page 3

### COM-2821

progressive Disclosure - Top- Verifying view #4 state & user can reverse naviagte back to page 1\
GIVEN- The progressive Disclosure 'top' component loads \
WHEN-The user has clicked the NEXT button for the final time to get to page 4
THEN- The user has seen all of the bubble-cards for the 'top' component - state #4
WHEN- The user is on the final page (page 4) of the 'top' component
AND - The user clicks the BACK button -  back to page 1
THEN - The user will see the 'top' component's first page/state #1

state 4 - user has clicked on the NEXT button to get to page 4

waiting for outer component container

waiting for SVG elements

Navigating to page 4 by clicking the NEXT button - three times

verifying button states

waiting for chat cards 3+4 to be visible

all other chat cards are hidden/not visible

visual check -  Top -  State 4 - page 4

GIVEN- The user has landed on page 4
WHEN- The user clicks the previous button on each subsequent page\
THEN- The user will be back on page 1 of the interactive

clicking pervious button

on next page previous button is active

on page 3 of 4

clicking pervious button

on next page previous button is active

on page 2 of 4

clicking pervious button

on next page previous button is disabled

on page 1 of 4

waiting for page 1/4 to be in a known state

visual check - Top- Back on page 1

### COM-2821

progressive Disclosure - Bottom - Verifying view #1 state\
GIVEN- The 'bottom' progressive disclosure component loads\
WHEN- The user visits the component page for the first time\
THEN- The user will be presented with the 'bottom' component's default view state

Default View - state 1 - page 1

waiting for outer component container

waiting for SVG elements

Expecting all chat cards to be disabled besides - chat card #1

Expecting Next button to be active and visible

chart card 1 should be visiable with opacity = 1

visual check -  Bottom- State 1 view/default view - page 1

### COM-2821

progressive Disclosure - Bottom- Verifying view #2 state\
GIVEN- The 'bottom' progressive disclosure component loads\
WHEN- The user clicks on the NEXT button
THEN- The user will be presented with the 'bottom' #2 state view - page 2

state 2 - User has clicked the NEXT button to get to page 2

waiting for outer component container

waiting for SVG elements

Navigating to page 2 by clicking the NEXT button

waiting for chat cards 1+2 to be visible

Card #3 is invisible

visual check -  Bottom- State 2 view/page 2

### COM-2821

progressive Disclosure - Bottom: Verifying view #3 state\
GIVEN- The progressive Disclosure 'bottom' component loads\
WHEN-The user has clicked the NEXT button for the final time to get to page 3
THEN- The user has seen all of the chat cards for the 'bottom' component - state #3

state 3 - user has clicked on the NEXT button to get to page 3

waiting for outer component container

waiting for SVG elements

Navigating to page 3 by clicking the NEXT button - twice

need to wait to click on the NEXT button or will cause the button stay visible

bottom NEXT button is disabled and not visible

waiting for chat cards 1+2+3 to be visible

visual check -  Bottom- State 3 view/page 3

<!-- /include: cypress/integration/progressiveDisclosure.js -->