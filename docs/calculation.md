# Calculation component 
> Test Set: [ALP-171](https://everfi.atlassian.net/browse/ALP-171)    
Type: Functional, Visual 

<!-- include: cypress/integration/blacksmith/calculation.js -->

### COM-1164 - Calculation - College Savings Calculator -- required field data is needed for form submit

GIVEN: The College Savings Calculator loads\
WHEN: the user submits a blank College Savings Calculator form\
THEN: The default values in the output zones stays unchanged

visual check -  before blank CS calc form submit

leaving calculation form black and lciking the submit button

visual check -  after blank CS calc form submit

verifying post submit - there is no change to the component page

### COM-1164

Calculation - College Savings Calculator -- with user data added to the required fields the calculation form submits and adds data to output zones\
GIVEN: The College Savings Calculator loads\
WHEN: user data is added to the required fields\
AND: The form is submitted\
THEN: data is added to the College Savings Calculator's output zones

input data is added to form fields

College Savings Calculator output zones post sumbit show expected data

### COM-1164

Calculation - slider -- has slider-handle input mechanism\
WHEN: The calculation-slider component loads\
THEN: A input slider handle is provided\

### COM-1164

Calculation - slider - Interest Rate (Compounded Monthly) -- has PLUS/MINUS buttons input mechanism\
WHEN: The calculation-slider component loads\
THEN: PLUS/MINUS buttons input mechanism buttons are presented\

injecting input data (to 1.5) into the calculation-slider component

verifying that both  the +/- buttons are not in a disabled state

COM-1164
GIVEN: The calculation-slider Interest Rate (Compounded Monthly) component loads\
WHEN: The user engages with the input mechanisms\
THEN: the output is seen in data-output zones in the form of numerical data

### GIVEN

The calculation-slider Interest Rate (Compounded Monthly) component is in its default state
WHEN: The PLUS button is clicked once\
THEN: The top slider output value = 1

Then the MINUS button is clicked once\
This resets the calculation output zones as default values

User sets slider value to = 1

All output zones for the calculation-slider Interest Rate (Compounded Monthly) component are updated with expected values

### COM-1164

Calculation - slider -slider Interest Rate (Compounded Monthly)- when the input mechanism has reached its highestlowest achievable data-input the +/- buttons should disable to indicate this\
GIVEN: The calculation-slider --slider Interest Rate (Compounded Monthly) component is loaded\
WHEN: the input mechanism has reached its highestlowest achievable data-input\
THEN: the +/- buttons should disable to indicate this

### GIVEN

setting slider to max range value

### THEN

The top slider output value = `2`

### THEN

 the bottom output values are set to the expected values

### WHEN

Slider is set to MAX value
THEN: the + button is in its diabled state\
THEN: the - button is in its active state

### GIVEN

setting slider to min range value

### THEN

The top slider output value = `0`

### THEN

 the bottom output values are set to the expected values

### WHEN

Slider is set to MIN value
THEN: the - button is in its diabled state\
THEN: the + button is in its active state

<!-- /include: cypress/integration/blacksmith/calculation.js -->