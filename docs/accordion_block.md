# Accordion Block Component  
> Test Set: [ALP-162](https://everfi.atlassian.net/browse/ALP-162)   
Type: Functional, Visual  

<!-- include: cypress/integration/accordion_block.js -->

### ALP-163

GIVEN: The accordion page loads\
WHEN: The accordion is in its default state\
THEN: All accordion nodes are closed by default

### ALP-164

WHEN: A closed node is clicked on\
THEN: That node expands\

### ALP-165

WHEN: An open accordion node is cliked on\
THEN: That clicked node closes

### ALP-166

GIVEN: The user visits the accordion block component\
WHEN: The user clicks on an accordion node\
THEN: The clciked on node expands\
THEN: The user Clicks on another accordion node\
THEN: The first accordion node closes\
AND: The second accordion node expands

### ALP-167

WHEN: A user clicks on an accordion node\
THEN: That clicked on node gets a checkmark icon\

### ALP-168

WHEN: the user clicks on an accordion node\
THEN: the user sees that node's unique content exposed

<!-- /include: cypress/integration/accordion_block.js -->