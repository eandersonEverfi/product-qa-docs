# Progression Component
> Test Set: [ALP-359](https://everfi.atlassian.net/browse/ALP-359)    
Type: Functional, Visual

<!-- include: cypress/integration/progression.js -->

### ALP-x1

progression - State Check- Default view - progression component\
GIVEN- User visits the BS2 course in the default state (no pages in the coures have been marked as complete)\
WHEN- The user visits the Progression component\
THEN- The user will see the Progression component's output zones reflect this default state

User verifies the progression component loads - on visit

By Default -  progressionBar_1 = 0%

By Default -  progressionBar_2 = 0%

By Default - progressionDonut_1 = 0% percent graphed

By Default - progressionDonut_1 =  has 0% text

By Default - progressionDonut_2 = 0% percent graphed

By Default - progressionDonut_2 =  has 0% text

By Default - document_percentage_1 =  0%

By Default - document_percentage_2 =  0%

progressionIndex_1 + progressionIndex_2
Indicate that the Progression component contains "Page 59 of 83"\

Visual Check - Defualt state of the Progression Component

### ALP-x2

progression - State Check-  \'Completed\' state - progression component\
GIVEN- The user has visited all course pages setting them to a 'completed' state
WHEN- The user visits the Progression component\
THEN- The user will see the Progression component's output zones reflect this course-completed state

user first completes all course content
marking each course page as completed\

user visits the Progression component after completing all other course pages

complete-state- progressionBar_1 set to 100%

complete-state- progressionBar_2 set to 100%

complete-state- progressionDonut_1 = 16% percent graphed

complete-state - progressionDonut_1 =  has 16% text

complete-state- progressionDonut_2 = 16% percent graphed

complete-state - progressionDonut_2 =  has 16% text

complete-state - document_percentage_1 =  1000%

complete-state - document_percentage_2 =  1000%

progressionIndex_1 + progressionIndex_2
Indicate that the Progression component contains "Page 59 of 83"\

Visual Check - complete-state of the Progression Component

<!-- /include: cypress/integration/progression.js -->