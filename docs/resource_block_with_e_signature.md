# Resource Block with E-Signature Block component
> Test Set: [ALP-138](https://everfi.atlassian.net/browse/ALP-138)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/resource_block_with_e_signature.js -->

### ALP-132

resource block with esignature - Clicking link causes modal to open\
GIVEN- The resource block with esignature component has loaded\
WHEN- The user clicks on the modal link\
THEN- The modal window will be presented to the user - revealing the modal's content

verifying base component page content is loaded

Visual check - default view\
Before clicking resource link

Visual check - After clicking resource link

### ALP-234

resource block with esignature - User is able to click viewpolicy link and see PDF content\
GIVEN- THe user has expanded the resource modal\
WHEN- The user clicks on the resource modal's resource link\
THEN- The user is automatically downloads PDF policy
  AND- The user completes filling out he e-signature name field and checks e-signature checkbox
  AND- The user receives successful confirmation

user clicks the  in-modal "visit resource" link and gets served a downloadable PDF

post-click of the esign checkbox
esign checkbox is visibly 'checked'\
esign checkbnox gets the class of 'signed'\

post-click of the esign checkbox
user gets a system message of "Thanks for signing!"

### ALP-231

Resourse block with e-signature -  User has option to close the modal window\
GIVEN- The Resourse block with e-signature loads\
WHEN- The user expands the resource modal\
THEN- The user will be presened with two options to close the open modal\
WHEN - The user clicks on either of the closing options\
THEN- The modal will close

User clicks the Xclose button of the expanded modal

post-click of the xClose button - modal is closed and not visible

user reopens the resource modal for the second time

user clicks on the close button

post-click of the close button - modal closes and is not visible

<!-- /include: cypress/integration/blacksmith/resource_block_with_e_signature.js -->