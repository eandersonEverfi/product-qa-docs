# Navigate Component
> Test Set: [ALP-128](https://everfi.atlassian.net/browse/ALP-128)    
Type: Functional, Visual  

<!-- include: cypress/integration/navigate.js -->

### ALP-149

navigate - user is able to select an \'active\' radio button\
GIVEN- The Navigate component has loaded\
WHEN- The user clicks an active radio button
THEN- Then that clicked on button becomes selected

waiting for the assessment questions to be visiable

user clicks on active-state radio button 1/3

post-click - radio button becomes selected

post-click - user gets feedback message

visual check -  After Select

### ALP-150

navigate - the user is able to select a radio button and get its corresponding response feedback message\
GIVEN- The Navigate component has loaded\
WHEN- The user clicks a radio button\
THEN- The user will get its corresponding response feedback message

waiting for the assessment questions to be visiable

### Radio button 1/3 tests

Radio button is in an active state\
Clicking radio button produces the `failureHeader` feedback message response

After clicking radio button 1/3
assesment button is still in a disabled state\
forward button is still in a disabled state

visual check -  After Select - Option A

### Radio button 2/3 tests

Radio button is in an active state\
Clicking radio button produces the `failureHeader` feedback message response

After clicking radio button 2/3
assesment button is still in a disabled state\
forward button is still in a disabled state

visual check -  After Select - Option B

### Radio button 3/3 tests

Radio button is in an active state\
Clicking radio button produces the `successHeader` feedback message response

After clicking radio button 3/3
assesment button converts to an active state\
forward button converts to an active state

visual check -  After Select - Option C

### ALP-154

navigate - user is able to submit the form once all required radio button options are filled\
GIVEN- The Navigate component has loaded\
WHEN- all required radio button options are filled (of the Assessment Form)\
THEN- user is able to submit the form

waiting for the assessment questions to be visiable

user clciks on radio button 3/3

post-click - user is presented with the `successHeader` feedback message

After clicking radio button 3/3
assesment button converts to an active state\
forward button converts to an active state

visual check -  After Select - Option C

user clicks on the now active assesment button

usser is taken to the ordering-doc page

### ALP-159

navigate - the user is not able to select disabled elements\
GIVEN- The Navigate component has loaded\
WHEN- The user clicks on a disabled-state element\
THEN- No action occurs

waiting for the disabled button

visual check -  Before click of disabled button

user clicks on the disabled button
Result = no action\

visual check -  After click of disabled button

### ALP-213

navigate - User is able to click an active button to navigate to a different page\
GIVEN- The Navigate component has loaded\
WHEN- The user clicks on active elements
THEN- The user will be navigated to that element's expected ending target location

### Back Button tests

in an active-state, by default\
Clicking takes the user to - modal-doc page

### Custom Path Button tests

in an active-state, by default\
Clicking takes the user to - /examples-activity/progress-timeline (external domain)

### Warp Button tests

in an active-state, by default\
Clicking takes the user to - /examples-activity/progress-timeline (external domain)

### Home tests

in an active-state, by default\
Clicking takes the user to - index.html# page

submitting Assessment form with Option 'C' selected

### Forward Button tests

in a deactivated-state, by default - user has to submit the Assessment Form first\
Clicking (active-sate) takes the user to - ordering-doc page

<!-- /include: cypress/integration/navigate.js -->