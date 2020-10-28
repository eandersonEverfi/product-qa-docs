# Page Skip 1+2 Component
> Test Set: [ALP-2134](https://everfi.atlassian.net/browse/ALP-2134)    
Type: Functional

<!-- include: cypress/integration/pageSkip.js -->

ALP-2134;
page skip - Navigation Links skipped - dictated by submitting form with certain radios selected\

### GIVEN user clicks radio button x (and submits form) = page navigation result

- Radio 1 = Selecting this option will skip the "Page Skip 2" page during page navigation\
- Radio 2 = Selecting this option will skip the "Page Skip 1" page during page navigation\
- Radio 3 = Selecting this option will skip both of the above pages during page navigation

selecting Radio 1 + clicking Nav Skip-Link 2 = '/page-skip-california-doc'

selecting Radio 1 + clicking Nav Skip-Link 1 = page-skip-1-doc NOT skipped

selecting Radio 2 + clicking Nav Skip-Link 1 = '/page-skip-2-doc'

selecting Radio 2 + clicking Nav Skip-Link 2 = page-skip-2-doc NOT skipped

selecting Radio 3 + clicking Nav Skip-Link 1 = '/page-skip-california-doc'

selecting Radio 3 + clicking Nav Skip-Link 2 = '/page-skip-california-doc'

<!-- /include: cypress/integration/pageSkip.js -->