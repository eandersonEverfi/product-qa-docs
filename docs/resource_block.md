# Resource Block component
> Test Set: [ALP-232](https://everfi.atlassian.net/browse/ALP-232)    
Type: Functional, Visual

<!-- include: cypress/integration/resource_block.js -->

### ALP-132

resource block - Clicking link causes modal to open\
GIVEN- The resource block component loads\
WHEN- The user clicks on the modal link\
THEN- The modal window will be presented to the user - revealing the modal's content

verifying base component page content is loaded

Visual check - default view\
Before clicking resource link

user clicks the modal link

once modal is verified as open
User can see the modal content\

Visual check - After clicking resource link

### ALP-231

resource block - User has option to close the modal window\
GIVEN- The resource block component loads\
WHEN- The user expands the resource modal\
THEN- The user will be presened with two options to close the open modal\
WHEN - The user clicks on either of the closing options\
THEN- The modal will close

verifying base component page content is loaded

clicking on the resouce modal's link

once modal is verified as open
User can see the modal content\

Visual check - After clicking resource link

user clicks the x-close button

user verifies modal is in its closed-state

Visual check - modal is closed via x button

User reopens the modal

visual check -  modal is open a second time

user clicks the close button

user verifies modal is in its closed-state

Visual check - modal is closed via close button

### ALP-141

Resource block - Modals that contain resource links as its unique content will take a user to an expected location\
GIVEN- THe user has expanded the resource modal
WHEN- The user clicks on the resource modal's resource link
THEN- The user is taken to that links's location

verifying base component page content is loaded

clicking on the resouce modal's link

Once modal has expanded
User visits resource link\
Verifies the resource link is the correct page

<!-- /include: cypress/integration/resource_block.js -->