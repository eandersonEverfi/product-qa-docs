# Switch Block Component
> Dev implemntation ticket: [COM-2799](https://everfi.atlassian.net/browse/COM-2799)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/switch.js -->

### COM-2799

Switch Block - user has an assessment form to choose 1 of 3 players\
GIVEN: The Switch Block has loaded for the initial time\
WHEN: The user is presented with the page's default view\
THEN: The user sees an assessment form

waiting for page know-state

visual check -  default state - after page loads

### COM-2799

Switch Block - Selecting radio button 1 - produces expected content\
GIVEN- The Switch Block component loads\
WHEN- The user selects radio button 1\
THEN- The Switch Block component produces expected content

waiting for page know-state

clicking on radio button 1
verifying radio button 1 is checked\

waiing for switch container to load picture - has height greater than 0

waiting for SVGs to be visible

Visual Check -  radio button 1 - after selection - expected content is shown

### COM-2799

Switch Block - Selecting radio button 2 - produces expected content\
GIVEN- The Switch Block component loads\
WHEN- The user selects radio button 2\
THEN- The Switch Block component produces expected content

waiting for page know-state

clicking on radio button 2
verifying radio button 2 is checked\

waiing for switch container to load picture - has height greater than 0

waiting for SVGs to be visible

Visual Check -  radio button 2 - after selection - expected content is shown

### COM-2799

Switch Block - Selecting radio button 3 - produces expected content\
GIVEN- The Switch Block component loads\
WHEN- The user selects radio button 3\
THEN- The Switch Block component produces expected content

waiting for page know-state

clicking on radio button 3
verifying radio button 3 is checked\

waiing for switch container to load picture - has height greater than 0

waiting for SVGs to be visible

Visual Check -  radio button 3 - after selection - expected content is shown

<!-- /include: cypress/integration/blacksmith/switch.js -->