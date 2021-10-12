# Modal Block component
> Test Set: [ALP-127](https://everfi.atlassian.net/browse/ALP-127)    
Type: Functional, Visual  

<!-- include: cypress/integration/blacksmith/modalBlock.js -->

@param {boolean} dismiss default, lightbox

### ALP-132 / ALP-139

Modal Block - Clicking link causes modal to open / reveals the modal\'s
              content and modal layout position\
GIVEN: An individual configuration of a modal link loads\
WHEN: The user clicks this specific modal's link\
THEN: Then the user will see presented that specific modal's window and content\
WHEN: The user clicks on the expanded modal's X-close button \
THEN: That expanded modal window will be closed, hidden from view

Verifying the Default Modal configuration
Post click of modal link - User sees open modal's specific content

visual check - After opeing the default modal

Verifying the Full Width Modal configuration
Post click of modal link - User sees open modal's specific content

visual check -  After opeing the full width modal

Verifying the Full screen Modal configuration
Post click of modal link - User sees open modal's specific content

visual check -  After opeing the full screen modal

Verifying the Nested Modal configuration
Post click of modal link - User sees open modal's specific content

visual check -  After opeing the nested modal

Verifying the Lightbox Modal configuration
Post click of modal link - User sees open modal's specific content

visual check - After opeing the Lightbox modal

Verifying the 'prevent_container_close' Modal configuration
Post click of modal link - User sees open modal's specific content

visual check -  After opeing the prevent_container_close modal

### GIVEN

The prevent_container_close modal is in an expanded state
WHEN: The user clicks outside the modal window
THEN: The system prevents the modal from closing

Verifying the with close button icons Modal configuration
user clicks the modal's link. Post click of modal link - User sees
open modal's specific content.

verifying thumbs svgs are visible upon opening modal

visual check =  After opeing the modal with close button icons

Verifying the footer icons Modal configuration
Post click of modal link - User sees open modal's specific content

visual check -  After opeing the modal with footer class

Verifying the Left Modal Drawer configuration
Post clicking the drawer-modal link - user sees the expanded
drawer-modal's content

Visual check -  After opeing the Left Drawer modal

Verifying the Right Modal Drawer configuration
Post clicking the drawer-modal link - user sees the expanded drawer-modal's content

Visual check -  After opeing the Right Drawer modal

Verifying the Top Modal Drawer configuration
Post clicking the drawer-modal link - user sees the expanded drawer-modal's content

Visual check -  After opeing the Top Drawer modal

Verifying the Bottom Modal Drawer configuration
Post clicking the drawer-modal link - user sees the expanded drawer-modal's content

Visual check -  After opeing the Bottom Drawer modal

### ALP-231

Modal block - Closing methods - User has option to close the modal
              window with a \'close\' button\
GIVEN: An individual configuration of a modal link loads\
WHEN: The user clicks this specific modal's link\
THEN: Then the user will see presented that specific modal's window\
WHEN: The user clicks on the expanded modal's 'close' button \
THEN: That expanded modal wondow will be closed, hidden from view

<!-- /include: cypress/integration/blacksmith/modalBlock.js -->