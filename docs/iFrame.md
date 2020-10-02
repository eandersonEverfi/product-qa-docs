# iFrame Component
> Test Set: [ALP-216](https://everfi.atlassian.net/browse/ALP-216)    
Type: Functional, Visual  

<!-- include: cypress/integration/iFrame.js -->

### ALP-218

iFrame -- An iFrame is able to load in custom content\
GIVEN: the iFrame component loads\
THEN: THe user will be able to see custom content loaded inside the iFrame

verifying that the compopnent page has the expected header text

verifying that iFrame is loaded and pointing to to the everfi homepage

verifying that the iFrame contains expected content - the Everfi svg logo

visual check - Redacted/skipped due to iFrame content is dynamic

### ALP-222

iFrame - The user is able to interact with embedded iFrame content\
GIVEN: the iFrame component loads\
WHEN: The user clicks the internal iFrame hamburger menu button\
THEN: The hamburger menu expands

verifying that the compopnent page has the expected header text

verifying that iFrame is loaded and pointing to to the everfi homepage

verifying that the Hamburger menu button is visible within the iFrame

User clicks the Hamburger menu button

visual check post hamburger menu button\
verifying that the user sees the hamburger menue is expanded\

ALP-217 - iFrame REFRESH button\
iFrame - clicking the \'refresh\' button refreshes the iFrame\
Test is skipped

### ALP-213

iFrame - User is able to click an active button to navigate to a different page\
GIVEN: the iFrame component loads\
WHEN: The user clicks on the 'Open in new Window' button\
THEN: The URL associated with this button loads

verifying that the compopnent page has the expected header text

verifying that iFrame is loaded

clicking the  'Open in new Window' button

URL that is associated with this button is loaded

<!-- /include: cypress/integration/iFrame.js -->