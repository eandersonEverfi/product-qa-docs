# Image Component
> Dev implemntation ticket: [COM-2916](https://everfi.atlassian.net/browse/COM-2916)    
Type: Functional, Visual  

<!-- include: cypress/integration/imageStack.js -->

### run these test as if on a macbook 15

Desktop resolution - macbook 15\
1440x900

it - shows Desktop state correctly

waiting for all content blocks

waiting for images

Decorative Image should have alt = null

Meaningful image should have alt = 'Alt text goes here'

GIVEN- User is on a macbook 15
WHEN- They visit the component\
THEN- The desktop images are shown\
AND- The images are in a desktop layout

Visual Check -  Desktop resolution - macbook 15

### run these test as if on an iPhone X

Mobile resolution - iPhone X\
375x812

it -  shows mobile state correctly

waiting for all content blocks

waiting for images

Decorative Image should have alt = null

Meaningful image should have alt = 'Alt text goes here'

GIVEN- User is on a iPhone X
WHEN- They visit the component\
THEN- The mobile images are shown\
AND- The images are in a mobile layout

Visual Check - Mobile resolution - iPhone X

### run these test as if on an iPad Mini

Tablet resolution - iPad Mini\
768x1024

it - shows tablet state correctly

waiting for all content blocks

waiting for images

Decorative Image should have alt = null

Meaningful image should have alt = 'Alt text goes here'

GIVEN- User is on a iPad Mini
WHEN- They visit the component\
THEN- The tablet images are shown\
AND- The images are in a tablet layout

visual check -  Tablet resolution - iPad Mini

<!-- /include: cypress/integration/imageStack.js -->