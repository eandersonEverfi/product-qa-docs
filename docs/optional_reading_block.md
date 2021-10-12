# Optional Reading Block Component
> Test Set: [ALP-131](https://everfi.atlassian.net/browse/ALP-131)    
Type: Functional, Visual  

<!-- include: cypress/integration/blacksmith/optional_reading_block.js -->

### ALP-132

optional reading - Clicking link causes modal to open\
GIVEN- The Optional Reading component has loaded\
WHEN- The user clicks on the modal link\
THEN- The modal window expands revealing it's unique content

waiting on the modal link

visual check - Default View -  Before clicking modal link

Verifying the Modal configuration

Post click of modal link - User sees open modal's specific content

visual check - After opeing the modal

### ALP-231

Optional Reading Block - User has option to close the modal window\
GIVEN- The Optional Reading Block's modal is in its expanded/open state\
WHEN- The user clicks on the Xclose or Close button\
THEN- The expanded modal will cose from view

waiting for the modal link

visual check - Default View -  Before clicking modal link

Verifying the Default Modal configuration

Post click of modal link - User sees open modal's specific content

visual check - After opeing the modal

clicking x-close button

post clicking Xclose button - modal converts to not being visible

visual check - After clicking the Xclose button

user expands the modal

user verifies that the modal window is in its expanded state

user verifies that the Close button is visible

user clicks the Close button

post click of the Close button - user verifies that the Modal Window has been closed from view

<!-- /include: cypress/integration/blacksmith/optional_reading_block.js -->