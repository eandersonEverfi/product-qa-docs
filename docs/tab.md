# Tabs Component
> Test Set: [ALP-135](https://everfi.atlassian.net/browse/ALP-135)    
Type: Functional, Visual

<!-- include: cypress/integration/tab.js -->

### ALP 199

tabs - By default the tabpanel loads focus on the first tab within the panel\
GIVEN- The tabs component page loads\
THEN- By default the user will see the tabpanel loads focus on the first tab within the panel

by defualut tab 1/3 has a sate of visited

by defualut tab 1/3 has a sate of active

by defualut tab 1/3 has a visible svg checkmark

Visual check - default state -  First tab of the panel is focused

### ALP 200

GIVEN- The Tabs component has loaded\
WHEN- The user has clicked on an individual tab\
THEN- This causes focus to switch to that clicked on tab

by defualut tab 1/3 has a sate of active

by defualut tab 1/3 has a sate of visited

by defualut tab 1/3 has a visible svg checkmark

Visual check - default state -  First tab of the panel is focused

user clicks tab 2/3

Tab 2/3 gains focus

Visual check-  Focus is switched to clicked tab

### ALP 201

GIVEN- The Tabs component has loaded\
WHEN- The user clicks on a tab\
THEN- this causes a checkmark to be added to that clicked on tab

by defualut tab 1/3 has a sate of active

by defualut tab 1/3 has a sate of visited

by defualut tab 1/3 has a visible svg checkmark

Visual check - default state -  First tab of the panel is focused

User clicks Tab 3/3

Tab 3/3 gains focus - with a state of visited

Tab 3/3 now has a visible svg checkmark

visual check - Tab 3/3  has checkmark after it was clicked

### ALP 202

GIVEN- The Tabs component has loaded\
WHEN- The user clicks on a tab\
THEN- With tab focus the user is able to see that individual tab's unique content

by defualut tab 1/3 has a sate of active

by defualut tab 1/3 has a sate of visited

by defualut tab 1/3 has a visible svg checkmark

Visual check - default state -  First tab of the panel is focused

User clicks on tab 2/3

Tab 2/3 gains focus - with a state of visited

With focus gained on tab 2/3
User sees the tab's unique text content\

visual check -  User is able to see the tabs content

<!-- /include: cypress/integration/tab.js -->