# Accordion Block Component  
> Test Set: [ALP-162](https://everfi.atlassian.net/browse/ALP-162)   
Type: Functional, Visual  

<!-- include: cypress/integration/accordion_block.js -->

### ALP-163 - accordion > all accordions node are closed by default

GIVEN: The accordion page loads\
WHEN: The accordion is in its default state\
THEN: All accordion nodes are closed by default

### ALP-164 - accordion > clicking on a closed accordion node expands that clicked node

WHEN: A closed node is clicked on\
THEN: That node expands\

after expanding first node - waiting for accordion node to have max-height of  576px

### ALP-165 - accordion > clicking on an open accordion node closes that clicked node

WHEN: An open accordion node is cliked on\
THEN: That clicked node closes

after expanding first node - waiting for accordion node to have max-height of  576px

### ALP-166 - accordion > only one accordion node can be opened at a time

GIVEN: The user visits the accordion block component\
WHEN: The user clicks on an accordion node\
THEN: The clciked on node expands\
THEN: The user Clicks on another accordion node\
THEN: The first accordion node closes\
AND: The second accordion node expands

after expanding first node - waiting for accordion node to have max-height of  576px

waitng for expanded node elemsnts button 1 and 2

### ALP-167 - accordion > expanding an accordion node adds a check mark to this node on opening

WHEN: A user clicks on an accordion node\
THEN: That clicked on node gets a checkmark icon\

after expanding first node - waiting for accordion node to have max-height of  576px

### ALP-168 - accordion > Upon expanding an accordion node the user sees this node's unique content

WHEN: the user clicks on an accordion node\
THEN: the user sees that node's unique content exposed

after expanding first node - waiting for accordion node to have max-height of  576px

### COM-1853 - accordion - all stepper accordion nodes are closed by default

GIVEN: A stepper accordion loads\
WHEN: The stepper accordion is in its default state\
THEN: All accordion nodes are closed by default

### COM-1853 - accordion - Stepper behavior on-click

GIVEN: user clicks on a stepper accordion that is configured to have multiple bellows open at once
WHEN: the first node is clicked\
THEN: That clicked node expands\
AND: a second node is clicked\
THEN: the second node epands while the first node stays expanded

clicking on the first stepper node

verifying expanded node is expanded and waiting for its expansion

waiting for node content

clicking on the 2nd stepper node

verifying expanded node is expanded and waiting for its expansion

closing the last stepper node

closing the first stepper node

veriyfing that the last stepper node is closed

verifying there a total of 2 checkmarks

<!-- /include: cypress/integration/accordion_block.js -->