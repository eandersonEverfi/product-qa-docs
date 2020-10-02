# I-spy Component
> Test Set: [ALP-122](https://everfi.atlassian.net/browse/ALP-122)    
Type: Functional, Visual  

<!-- include: cypress/integration/iSpy.js -->

### ALP-129

iSpy - Popover windows are displayed when its hotspot is clicked\
GIVEN: The iSpy component has loaded\
WHEN: The user clicks on a individual hotspot\
THEN: A Popover window is shown to the user in response

waiting for hotspot 1

visual check -  default page view

clicking hotspot 1

Post hotspot 1 click
Verify - hotspot 1 has a class of clicked\
Verify - hostspot 1 has the check svg visible\
verify - hotspot 1 now displays the popover

Hotspot 1's popover has specific text shown

waiting for the position of the presented tooltip is in its final state before continuing with the test

visual check - post hotspot 1 click

clicking hotspot 2

Post hotspot 2 click
Verify - hotspot 2 has a class of clicked\
Verify - hostspot 2 has the check svg visible\
verify - hotspot 2 now displays the popover

Hotspot 2's popover has specific text shown

waiting for the position of the presented tooltip is in its final state before continuing with the test

visual check - post hotspot 2 click

clicking hotspot 3

Post hotspot 3 click
Verify - hotspot 3 has a class of clicked\
Verify - hostspot 3 has the check svg visible\
verify - hotspot 3 now displays the popover

Hotspot 3's popover has specific text shown

waiting for the position of the presented tooltip is in its final state before continuing with the test

visual check - post hotspot 3 click

### ALP-142

iSpy - Clicking an open Popover causes the Popover to close its window\
GIVEN: The iSpy component has loaded\
WhEN: The user clicks on an expanded popover\
THEN: The popover closes\

clicking hotspot 1 - to reveal the popover

post click hp1 - popover is visible

clicking the background image to cause the expanded popover to close

visual check - verifying popover for hp1 has closed

clicking hotspot 2 - to reveal the popover

post click hp2 - popover is visible

clicking the background image to cause the expanded popover to close

visual check - verifying popover for hp2 has closed

clicking hotspot 3 - to reveal the popover

post click hp3 - popover is visible

clicking the background image to cause the expanded popover to close

visual check - verifying popover for hp2 has closed

### ALP-xx

iSpy - after the user views all popover, the NEXT button will activate\
GIVEN: The iSpy component has loaded\
WhEN: The user viewed all popovers\
THEN: the NEXT button will activate

by default the NEXT button is disabled

visual verification - by default the NEXT button is disabled

clicking on the disabled NEXT button

Verify - User stays on the iSpy component page

GIVEN:The user has clicked on all hotspots\
THEN:All hotspots are set to a completed state

visual check - post clicking on all hotspots - NEXT button is in the active state

GIVEN:The user clicks on an active-state NEXT button\
THEN:The user is taken to a new component page

<!-- /include: cypress/integration/iSpy.js -->