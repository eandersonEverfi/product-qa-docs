# Resource Block with E-Signature Block component
> Test Set: [ALP-138](https://everfi.atlassian.net/browse/ALP-138)    
Type: Functional, Visual

<!-- include: cypress/integration/resource_block_with_e_signature.js -->

### ALP-132

resource block with esignature - Clicking link causes modal to open\
GIVEN- The resource block with esignature component has loaded\
WHEN- The user clicks on the modal link\
THEN- The modal window will be presented to the user - revealing the modal's content

verifying base component page content is loaded

Visual check - default view\
Before clicking resource link

user clicks the modal link

once modal is verified as open
User can see the modal content\

Visual check - After clicking resource link

### ALP 233

resource block with esignature - E-signature checkbox is engaged only after viewing required content\
GIVEN- The resource block with esignature component has loaded\
AND- The user has expanded the resource modal\
WHEN- The user attempts to engage the eSign checkbox, before the user visits the view resourse link\
THEN- The system will pervent this, until the user visits the in-modal resource link, beforehand

user clicks the modal link

once modal is verified as open
User can see the modal content\

Visual check - After clicking resource link

user clicks the esign checkbox

esign chckbox is NOT checked

visual check -  Before clicking in-modal "visit resource" link

user clicks the in-modal "visit resource" link

post-click of the "visit resource" link
"visit resource" link gets the class of 'clicked'\

user clicks the esign checkbox

post-click of the esign checkbox
esign checkbox is visibly 'checked'\
esign checkbnox gets the class of 'signed'\

post-click of the esign checkbox
user gets a system message of "Thanks for signing!"

visual check - After clicking in-modal "visit resource" link + checking the esign checkbox

### ALP-234

resource block with esignature - User is able to click viewpolicy link and see its content\
GIVEN- THe user has expanded the resource modal\
WHEN- The user clicks on the resource modal's resource link\
THEN- The user is taken to that links's location

user clicks the modal link

the  in-modal "visit resource" link has an href that includes 'wiki/Made-up_words'

user clicks the  in-modal "visit resource" link and gets served the expcted link-page

### ALP-231

Resourse block with e-signature -  User has option to close the modal window\
GIVEN- The Resourse block with e-signature loads\
WHEN- The user expands the resource modal\
THEN- The user will be presened with two options to close the open modal\
WHEN - The user clicks on either of the closing options\
THEN- The modal will close

user clicks the modal link

once modal is verified as open
User can see the modal content\

visual check -  After modal expands

User clicks the Xclose button of the expanded modal

post-click of the xClose button - modal is closed and not visible

visual check -  modal is closed by 'x' button

user reopens the resource modal

visual check -  After modal expands for the second time

user clicks on the close button

post-click of the close button - modal closes and is not visible

visual check -  modal is closed by 'close' button

<!-- /include: cypress/integration/resource_block_with_e_signature.js -->