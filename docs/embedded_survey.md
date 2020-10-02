# Embedded Survey component
> Test Set: [ALP-118](https://everfi.atlassian.net/browse/ALP-118)    
Type: Functional, Visual  

<!-- include: cypress/integration/embedded_survey.js -->

### ALP-152

embedded survey > by default the form submit button is in a deactivated state\
GIVEN: The embedded survey component loads\
THEN: By default the 'submit' button is a deactivated state

Next and Send buttons should be diabled

visual check by default the 'send' button is in a deactivated state

### ALP-153

embedded survey > After the user selects all required fields the send button is in its active state\
GIVEN: The embedded survey component loads\
WHEN: All required fields are selected\
THEN: The 'send' button is in an active state

Next and Send buttons should be diabled

visual check - by default the 'send' button is in a deactivated state

user clicks the first radio button option in the frist group

user clicks the first radio button option in the second group

send button is now active

Next button is in a deactivated state

visual check - post required fields selected -  'Send' button is in activated state

### ALP-154

embedded survey > user is able to submit the form once all required radio button options are filled\
GIVEN: The embedded survey component loads\
WHEN: All required fields are selected\
THEN: The user is able to submit the survey form\
THEN: After the form is submitted the Next button becomes active

Next and Send buttons should be diabled

visual check by defaulty the 'send' button is in a deactivated state

user clicks the first radio button option in the frist group

user clicks the first radio button option in the second group

send button is now active

Next button is in a deactivated state

visual check post required fields selected -  'Send' button is in activated state

User clicks the active-state 'send' button

send button is now disabled

Next button is now active

Visual Check Post clicking 'send' buitton - Form is submitted

<!-- /include: cypress/integration/embedded_survey.js -->