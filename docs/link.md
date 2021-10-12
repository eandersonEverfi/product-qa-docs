# Link Component
> Test Set: [ALP-126](https://everfi.atlassian.net/browse/ALP-126)    
Type: Functional, Visual  

<!-- include: cypress/integration/blacksmith/link.js -->

### ALP-214

link - User is able to click an active link to navigate to a different course location\
GIVEN: The Link block component loads\
WHEN: The user clicks on an active link\
THEN: The user is taken to the expected couse location

verifying the link  to new window is present

visual check - default view of the Link block componet - user sees link to new window

user clicks the link to new window - href includes 'giphy'

post click - user verifys they are on the expected giphy page

visual check post click - user sees link content in new window

### ALP-214

link - Links can have two types of tooltips - One that is activated by a click the other by a rollover\
GIVEN: The Link block component loads\
WHEN: The user interacts with a tooltip\
THEN: THe user sees the tooltip presented - post click or rollover

user sees the tooltip link

user sees that this link contains 'I have a tooltip on right' text

user rolls over this link

visual check - post rollover - user sees tooltip presented on the right

user sees a link with a popover on top

user clicks on link

post click - user sees popover with its specific text

visual check - user sees tooltip post click

### ALP-139

link - modal content is visible\
GIVEN: The Link block component loads\
WHEN: The user expands a modal by clicking on its respective link\
THEN: The user will see this expanded modals content

user sees modal link and clicks it

expanded modal has Header with specific text

visual check - post modal expanded

### ALP-132

link - clicking link causes modal to open\
GIVEN: The Link block component loads\
WHEN: The user expands a modal by clicking on its respective link\
THEN: user sees the modal in its expanded state

visual check - default view of Link Block - contains the link to new modal

user clicks on modal link

expanded modal has Header with specific text

visual check - post modal expanded

### ALP-131

link - User has option to close the modal window\
GIVEN: The Link block component loads\
WHEN: The suer clicks on the X-close button of and expanded modal\
THEN: The expanded modal closes\
WHEN: The suer clicks on the 'close' button of and expanded modal\
THEN: The expanded modal closes

user sees the modal link and clicks it

visual check - post exanded the modal

user sees the X-close button and clicks it

Visual check - post click of the X-close button- modal is closed/not visible

user re-expands/opens modal by clicking the link

visual check - expanded modal

user clicks the 'close' button of an expanded modal

Visual check - post click of the 'close' button- modal is closed/not visible

### COM-x1

link - On click: Links can direct users to other internal pages or externial pages\
GIVEN: The Link block component loads\
WHEN: The user clicks on links to other internal pages or externial pages\
THEN: The suer is taken to the that clicked on links expected destination

verifying that link 1 loads - 'Warp to Examples Module'

<!-- /include: cypress/integration/blacksmith/link.js -->