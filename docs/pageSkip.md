# Page Skip 1+2 Component
> Test Set: [ALP-2134](https://everfi.atlassian.net/browse/ALP-2134)    
Type: Functional

<!-- include: cypress/integration/blacksmith/pageSkip.js -->

ALP-2134;
page skip - Navigation Links skipped - dictated by submitting form with certain radios selected\

### GIVEN user clicks radio button x (and submits form) = page navigation result

- Radio 1 = Selecting this option will skip the "Page Skip 2" page during page navigation\
- Radio 2 = Selecting this option will skip the "Page Skip 1" page during page navigation\
- Radio 3 = Selecting this option will skip both of the above pages during page navigation

selecting Radio 1 = 'page skip 2' not in DOM

selecting Radio 1 + clicking Nav Skip-Link 1 = page-skip-1-doc NOT skipped

selecting Radio 1 + visiting Skip-Link 2 = page-skip-2-doc IS skipped, user lands on /page-skip-california-doc

selecting Radio 2 = 'page skip 1' not in DOM

selecting Radio 2 + clicking Nav Skip-Link 2 = page-skip-2-doc NOT skipped

selecting Radio 2 + visiting Skip-Link 1 = page-skip-1-doc IS skipped, user lands on /page-skip-2-doc

selecting Radio 3 = 'page skip 1' & 'page skip 2' not in DOM

selecting Radio 3 + visiting Skip-Link 1 or 2 = page-skip 1+2 IS skipped, user lands on /page-skip-california-doc

<!-- /include: cypress/integration/blacksmith/pageSkip.js -->