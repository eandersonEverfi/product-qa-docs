# Modal Menu component
> Test Set: [ALP-290](https://everfi.atlassian.net/browse/ALP-290)    
Type: Functional, Visual  

<!-- include: cypress/integration/modalMenu.js -->

### ALP-x1

Modal Menu - State Check: Default view\
GIVEN- The user is visiting the BS2 course for the frist time\
WHEN- The Modal Menu component loads\
THEN- `Module 1` will reflect this default state within its output zones

`Module 1` is visible

CTA button has a class of `not-started`

The course footer has a class of `not-attempted`

### The progress bar is set to `width

0%;`

The Left Nav has zero checkmarks

visual check - Default State

### ALP-x2

GIVEN- The user visits the Modal Menu within its default state\
WHEN- The user clicks on the CTA button\
THEN- The `Module 1` output zones will be updated to reflect this

`Module 1` is visible

User clicks the CTA button

Post-Click- CTA button's class is updated to `in-progress`

### Post-Click

footer's class remains unchanged =  'not-attempted'

### Post-Click - progress bar updates to  'width

51%;'

Post-Click - Left Nav bar indicates completion states of pages by adding 41 check marks

Post-Click - URL is updated to '~/index.html#documentation'

Visual Check - After clicking the CTA button

### ALP-x3

Modal Menu - State Check: \'Completed\' state\
GIVEN- The user has visited all course pages setting them to a 'completed' state\
AND- User answered Assessments with a 100% passing grade\
WHEN- The user visits the Modal Menu  component\
THEN- The user will see the Modal Menu  component's output zones reflect this course-completed state

user visits the module-menu-doc component after completing all other course pages

`Module 1` is visible

Post BS2 course completion - CTA button's class is set to  'completed'

Post BS2 course completion\
Module 1 footer contains\
(1) score = '100%'\
(2) button to retake assessment (directs users to '/qa-feedback-doc')\
(3) Footer set to class = 'passed'

### Post BS2 course completion -  progress bar is set to width

100%;'

Post BS2 course completion -  Left Nav bar has all pages with a checkmark (totalling 78 toat checkmarks)

visual check -  'Completed' state

<!-- /include: cypress/integration/modalMenu.js -->