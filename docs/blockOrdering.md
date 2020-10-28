# Block Ordering component 
> Test Set: [ALP-292](https://everfi.atlassian.net/browse/ALP-292)  
Type: Functional, Visual   

<!-- include: cypress/integration/blockOrdering.js -->

### ALP-x1

block ordering - State 1 - By default user is presented with btn1 and a disabled btnEnd\
GIVEN- The block ordering component has loaded for the initial time\
WHEN- The user views the component page\
THEN- By default the user is presented with btn1 and a disabled btnEnd

by deffault
the comopenent page loads with\
button 1 as disabled\
button 2 as not visible\
end button is disabled + visible

visual check -  Default View

### ALP-x2

block ordering - State 2 - From the default view when clicking btn1, btn2 is then displayed as active, btnEnd is disabled\
GIVEN- The Block Ordering component has loaded\
WHEN- The user has clicked btn1\
THEN- btn2 is displayed as active
THEN- btnEnd is visible + in a disabled-state

visual check -  After clicking button 1

### ALP-x3

block ordering - State 3 - From state 2 - clicking btn2, all buttons are visible, btn1 + btn2 + btnExit are acvtive + success alert is visible\
GIVEN- The Block Ordering component has loaded\
WHEN- The user has clicked both btn1 + btn2\
THEN- btn1, btn2 and btnEnd will be visble + in an actve-state\
THEN- User will be presented with a success alert indicating that 'This page has been completed.'

visual check -  After clicking button 2

<!-- /include: cypress/integration/blockOrdering.js -->