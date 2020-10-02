# Modal Block component
> Test Set: [ALP-127](https://everfi.atlassian.net/browse/ALP-127)    
Type: Functional, Visual  

<!-- include: cypress/integration/modalBlock.js -->

### ALP-132 / ALP-139

Modal Block - Clicking link causes modal to open / reveals the modal\'s content and modal layout position\
GIVEN: An individual configuration of a modal link loads\
WHEN: The user clicks this specific modal's link\
THEN: Then the user will see presented that specific modal's window and content\
WHEN: The user clicks on the expanded modal's X-close button \
THEN: That expanded modal wondow will be closed, hidden from view

Verifying the Default Modal configuration

Post click of modal link - User sees open modal's specific content

visual check - After opeing the default modal

clicking x-close button

visual check - After clicking the x button

Verifying the Full Witdh Modal configuration

Post click of modal link - User sees open modal's specific content

visual check -  After opeing the full width modal

clicking x-close button

visual check -  After clicking the x button

Verifying the Full screen Modal configuration

Post click of modal link - User sees open modal's specific content

visual check -  After opeing the full screen modal

clicking x-close button

visual check -  After clicking the x button

Verifying the Nested Modal configuration

Post click of modal link - User sees open modal's specific content

visual check -  After opeing the nested modal

clicking x-close button

visual check-  After clicking the x button

Verifying the Lightbox Modal configuration

Post click of modal link - User sees open modal's specific content

visual check - After opeing the Lightbox modal

clicking x-close button

visual check -  After clicking the x button

Verifying the 'prevent_container_close' Modal configuration

Post click of modal link - User sees open modal's specific content

visual check -  After opeing the prevent_container_close modal

### GIVEN

The prevent_container_close modal is in an expanded state
WHEN: The user clicks outside the modal window
THEN: The system prevents the modal from closing

user clicks on the x-close button

Then the open modal closes

visual check -  After clicking the x button

Verifying the with close button icons Modal configuration

user clicks the modal's link

Post click of modal link - User sees open modal's specific content

verifying thumbs svgs are visible upon opening modal

visual check =  After opeing the modal with close button icons

clicking x-close button

visual check - After clicking the x button

Verifying the footer icons Modal configuration

Post click of modal link - User sees open modal's specific content

visual check -  After opeing the modal with footer class

clicking x-close button

visual check - After clicking the x button

### ALP-132 / ALP-139

Modal Block - Clicking Drawer Modal link causes drawer to open / reveals the drawer\'s content and drawer layout position\
GIVEN: An individual configuration of a drawer-modal link loads\
WHEN: The user clicks on this specific drawer-modal link
THEN: The user will see the respective drawer-modal expand into its open-state
GIVEN: The user clicks on an open-state drawer-modal's x-close button
THEN: This specific drawer-modal closes

Verifying the Left Modal Drawer configuration

Post clicking the drawer-modal link - user sees the expanded drawer-modal's content

Visual check -  After opeing the Left Drawer modal

Clicking the x-close button

drawer-modal window is closed

visual check - After clicking the x button

Verifying the Right Modal Drawer configuration

Post clicking the drawer-modal link - user sees the expanded drawer-modal's content

Visual check -  After opeing the Right Drawer modal

Clicking the x-close button

drawer-modal window is closed

Visual check - After clicking the x button

Verifying the Top Modal Drawer configuration

Post clicking the drawer-modal link - user sees the expanded drawer-modal's content

Visual check -  After opeing the Top Drawer modal

Clicking the x-close button

drawer-modal window is closed

Visual check - After clicking the x button

Verifying the Bottom Modal Drawer configuration

Post clicking the drawer-modal link - user sees the expanded drawer-modal's content

Visual check -  After opeing the Bottom Drawer modal

Clicking the x-close button

drawer-modal window is closed

Visual check - After clicking the x button

### ALP-231

Modal block - Closing methods - User has option to close the modal window with a \'close\' button\
GIVEN: An individual configuration of a modal link loads\
WHEN: The user clicks this specific modal's link\
THEN: Then the user will see presented that specific modal's window\
WHEN: The user clicks on the expanded modal's 'close' button \
THEN: That expanded modal wondow will be closed, hidden from view

<!-- /include: cypress/integration/modalBlock.js -->