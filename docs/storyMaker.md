# Story Maker component
> Dev implemntation ticket: [COM-3063](https://everfi.atlassian.net/browse/COM-3063)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/storyMaker.js -->

### COM-3063

Story Maker - The default view is displaying correctly\
WHEN- The Story Maker component loads for the first time\
THEN- The default view is seen

waitng for elemnts to load on the page

asserting passage text tile

asserting the 'back' button is diabled

asserting expected image is on page

assrting that there are 4 visible buttons on the page

visual check - Default view on first load

### COM-3063

GIVEN- The user is interacting with the 'Looks for the skipper to harass' pathing branch\
WHEN- The user clicks through the interavtive by clicking on all of the available buttons in the path\
THEN- The user will be able to see all ending state pages with the expected title

Waiting for links to be visible on the page

### clicks button

 "Looks for the skipper to harass"

aserting there are 2 visible links on the page

asserting the 'back' button is not diabled

### clicks button

 "They go fishing"

aserting there are 2 visible links on the page

asserting the 'back' button is not diabled

### clicks button

 "Skipper smacks Gilligan with his hat"

User is at end-state page with expected title

asserting the 'back' button is not diabled

visual check -  'But Gilligans ducks just in time.' page

user manually refreshes the component page

Waiting for links to be visible on the page

### clicks button

 "Looks for the skipper to harass"

aserting there are 2 visible links on the page

asserting the 'back' button is not diabled

### clicks button

 "Gilligan playfully grabs the skipper's hat."

User is at end-state page with expected title

asserting the 'back' button is not diabled

asserting expected image is on page

visual check -  'Gilligan sees the skipper has gone completely bald overnight...' page

user manually refreshes the component page

Waiting for links to be visible on the page

### clicks button

 "Looks for the skipper to harass"

aserting there are 2 visible links on the page

asserting the 'back' button is not diabled

### clicks button

 "They go fishing"

aserting there are 2 visible links on the page

asserting the 'back' button is not diabled

### clicks button

 "Skipper agrees to fish in Gilligan's new spot."

User is at end-state page with expected title

asserting the 'back' button is not diabled

visual check -  'The two friends catch a mess of fish.' page

### COM-3063

Story Maker - User can use the 'back button' to go to the preceding page\
GIVEN- The user is on the end-sate page for the 'Looks for the skipper to harass' pathing branch\
WHEN- The user clicks the 'back' button on each subpage of this path\
THEN- The user will be naviagated to each preceding page until they reach the first/default page of the interactive

Waiting for links to be visible on the page

### clicks button

 "Looks for the skipper to harass"

aserting there are 2 visible links on the page

asserting the 'back' button is not diabled

### clicks button

 "They go fishing"

aserting there are 2 visible links on the page

asserting the 'back' button is not diabled

### clicks button

 "Skipper smacks Gilligan with his hat"

User is at end-state page with expected title

asserting the 'back' button is not diabled

user clicks the 'back' button

user is on the  'Gilligan says he knows a great spot to fish' page

asserting the 'back' button is not diabled

user clicks the 'back' button

user is on the  'Gilligan finds the skipper at the lagoon...' page

asserting the 'back' button is not diabled

user clicks the 'back' button

user is on the  'Gilligan wakes up on a deserted island and he...' page

asserting the 'back' button is diabled

User has returned back to the  first/default page of the interactive

asserting expected image is on page

assrting that there are 4 visible buttons on the page

visual check - Back on the fist page

<!-- /include: cypress/integration/blacksmith/storyMaker.js -->