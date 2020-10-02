# Assessment with redirect template  
> Dev Implementation ticket: COM-xx  
Type: Visual   

<!-- include: cypress/integration/assessment_block_redirect.js -->

### COM-x1 - Redirect Assessment > Onloading of component the user will see a loading spinner

GIVEN: The Redirect Assessment Block component loads\
THEN: The user will be presented with a loading spinner

Waiting for default elements\
(1) Page container\
(2) Outter Assessment component container\
(3) Page contains the word 'Redirect'

Within the Assessment component there is a spinner Conainer
Within the Spinner Container is a visible loading spinner SVG

visual check -  On Load user sees assessment with spinner

<!-- /include: cypress/integration/assessment_block_redirect.js -->