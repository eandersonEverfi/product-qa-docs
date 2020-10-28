# Twine component
> Test Set: [ALP-300](https://everfi.atlassian.net/browse/ALP-300)    
Type: Functional, Visual

<!-- include: cypress/integration/twine.js -->

### ALP-x1

twine - Clinking the blur in/out buttons cause lottie animations\
GIVEN- The Twine component has loaded\
WHEN- The user clicks the blur in/out buttons
THEN- The Lottie responds with expected animation behavior

waiting for buitton 2/3 and clappersnap svg to load onto the page

visual check -  Default - Before clicking the 'blur' button - clappersnap is not blured

user clicks button 2/3

clappersnap becomes blured

visual check -  After clicking 'blur' button - clappersnap is in a blured-state

user clicks button 3/3

clappersnap responds by reverting to default (unblured state)

visual check -  After clicking the 'unblur' button - clappersnap reverts to unblured-state

### ALP-x2

twine -  clicking the "unblur" button causes a code snippet to fade out\
GIVEN- The Twine component has loaded\
WHEN- clicking the "unblur" button
THEN- Code snippet fades out

waiting for button 3/3

Visual Check -  Before clicking the 'unblur' button - code sinppet is visible

user clicks button 3/3

visual check - After clicking the 'unblur' button - code snippet is invisible

### ALP-x3

twine - interacting with a slider transforms a lottie animation\
GIVEN- The Twine component has loaded\
WHEN- The user interacts with the slider controll\
THEN- The lottie responds with transform animations

waiting for slider controll and  mallMorph container

visual check -  Default state of lottie

user slides slide controll to val = `10`

visual check -  state of lottie post slide input

<!-- /include: cypress/integration/twine.js -->