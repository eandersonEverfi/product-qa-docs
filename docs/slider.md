# Slider Component
> Test Set: [ALP-133](https://everfi.atlassian.net/browse/ALP-133)    
Type: Functional, Visual

<!-- include: cypress/integration/slider.js -->

### ALP 173

GIVEN- The Slider with steps buttons and labels component has loaded\
THEN- The user sees that the Slider component has a slider-handle input mechanism

visual check -  Slider has slider-handle mechanism

### ALP 174

GIVEN- The Slider with steps buttons and labels component has loaded\
THEN- The user sees that the Slider component has PLUS/MINUS buttons input mechanism

visual check -  Slider has mins and plus button

### ALP 175

GIVEN- The Slider with steps buttons and labels component has loaded\
WHEN- The user interacts/clicks the Slider component's PLUS/MINUS buttons\
THEN- The output is seen in data-output zones in the form of numerical data

user clicks the Slider's PLUS button

Visual check -  User sees slider numbers after clicking plus button

user clicks the slider's MINUS button

Visual check -  User sees slider numbers after clicking minus button

### ALP 175

GIVEN- The Slider with steps buttons and labels component has loaded\
WHEN- The input mechanism has reached its highest achievable data-input\
THEN- The user cant input higher input values\
AND- The Slider UI changes to indicate this state

verifies that the PLUS/MINUS buttons are present

The PLUS button is clicked 100x (from the default state)

The PLUS button converts to a 'disabled' state once reaching this peak/max level of data-input

visual check -  User reaches maximum input available

### ALP 177

GIVEN- The Slider with steps buttons and labels component has loaded\
WHEN- The input mechanism has reached its lowest achievable data-input\
THEN- The user cant input lower input values\
AND- The Slider UI changes to indicate this state

verifies that the PLUS/MINUS buttons are present

User clicks the PLUS button twice

User clicks the MINUS button twice

The MINUS button converts to a 'disabled' state once reaching this lowest level of data-input

visual check -  User reaches to minimum input available

<!-- /include: cypress/integration/slider.js -->