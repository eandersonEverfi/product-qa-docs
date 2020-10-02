# Icon Component
> Test Set: [ALP-123](https://everfi.atlassian.net/browse/ALP-123)    
Type: Functional, Visual  

<!-- include: cypress/integration/icon.js -->

### ALP-199

icon - by default the tabpanel loads focus on the first tab within the panel\
GIVEN: The icon component page loads\
WHEN: The user views the Tab with icons component\
THEN: The user will see by default the tabpanel loads focus on the first tab within the panel

waiting for the default view

Visual check - Tabpanel default view

### ALP-199

icon - clicking on a individual tab of a tabpanel causes focus to switch to that clicked on tab\
GIVEN: The icon component page loads\
WHEN: The user views the Tab with icons component\
AND: The user clicks on the invidual tabs of the tabpanel\
THEN: On click - the focus will switch to that clicked on tab

waiting for the default view

Visual check - Tabpanel default view - Tab one has focus

clicking on Tab 2

post click of Tab 2 - waiting for Tab 2 View

visual check - Tab 2 has focus

clicking on Tab 3

post click of Tab 3 - waiting for Tab 3 View

visual check - Tab 3 has focus

### ALP-202

icon - With tab focus the user is able to see that individual tab\'s unique content\
GIVEN: The icon component page loads\
WHEN: The user views the Tab with icons component\
WHEN: The user clicks on the invidual tabs of the tabpanel\
THEN: with tab focus the user is able to see that individual tab\'s unique content

waiting for the default view

Visual check - User sees Tab 1's unique content

Verification - Tab 1 - user sees unique copy content

clicking on Tab 2

post click of Tab 2 - waiting for Tab 2 View

Visual check - User sees Tab 2's unique content

Verification - Tab 2 - user sees unique copy content

clicking on Tab 3

post click of Tab 3 - waiting for Tab 3 View

Visual check - User sees Tab 3's unique content

Verification - Tab 3 - user sees unique copy content

<!-- /include: cypress/integration/icon.js -->