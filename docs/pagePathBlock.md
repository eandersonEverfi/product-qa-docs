# Page-path block Component
> Test Set: [ALP-293](https://everfi.atlassian.net/browse/ALP-293)    
Type: Functional, Visual  

<!-- include: cypress/integration/pagePathBlock.js -->

ALP-x1
GIVEN: The page-path block component loads\
WHEN: The user complets all provided paths\
THEN: Each of the completed paths are marked as complete

Functional path to completing an individual path A/B

wait for main component container to load

Click path a or b

once clicked the user is taken to the First subpage

user clicks First subpage's Example link

user is taken to the path's Last subpage

user is provided a link and clicks it

user is taken back to the  main component page

Completing Path A

user waits for the compoent's main page

verify - the NEXT button is in a disabled state

Visual Check - Default state of component on initial load

user clicks the Path A link - following the functional steps

verify - the NEXT button is in a disabled state

Visual Check - After completing functional steps for Path A - Path A is marked as complete

Main component page has updated copy - "Path A completed."

Completing Path B

user clicks the Path B link - following the functional steps

Visual Check - After visitng both Paths A and B

Path A + B are marked as complete

Main component page has updated copy
"Path A completed."\
"Path B completed."

compoent is marked as compelte in the DOM

verify - the NEXT button is in an active state

<!-- /include: cypress/integration/pagePathBlock.js -->