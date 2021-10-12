# Viewport Filter component
> Dev implemntation ticket: [COM-2960](https://everfi.atlassian.net/browse/COM-2960)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/viewport_filter.js -->

run these test as if on a macbook 15
1440x900\

### it - shows Desktop Header and Desktop Description

GIVEN- The Viewport Filter component page has loaded\
WHEN- The viewport is sized as macbook 15 (1440x900)\
THEN- The user will see content specific to this viewport resolution

user sees header text with the following content
'Desktop Blocks'\

user sees description text with the following content
'These blocks will only render on desktop'\

The Desktop viewport only has two unique content blocks
The Header text\
The Description text

Desktop Viewport  contains the snippet block

visual check -  Desktop resolution - macbook 15

run these test as if on an iPhone X
375x812\

### it - shows Mobile Header and Mobile Description

GIVEN- The Viewport Filter component page has loaded\
WHEN- The viewport is sized as an iPhone X (375x812)\
THEN- The user will see content specific to this viewport resolution

user sees header text with the following content
'Mobile Blocks'\

user sees description text with the following content
'These blocks will only render on mobile'\

The Mobile viewport only has 3 unique content blocks
The Header text\
The Description text\
The Accordion Block

Mobile Viewport  contains the snippet block

visual check -  Mobile resolution - iPhone X

run these test as if on an "iPad Mini"
768x1024\

### it - shows Tablet Header and Tablet Description

GIVEN- The Viewport Filter component page has loaded\
WHEN- The viewport is sized as an "iPad Mini" (768x1024)\
THEN- The user will see content specific to this viewport resolution

user sees header text with the following content
'Tablet Blocks'\

The Tablet viewport only has two unique content blocks
The Header text\
The Description text - 'These blocks will only render on tablet'

Tablet Viewport  contains the snippet block

visual check -  Tablet resolution - iPad Mini

<!-- /include: cypress/integration/blacksmith/viewport_filter.js -->