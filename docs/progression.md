# Progression Component
> Test Set: [ALP-359](https://everfi.atlassian.net/browse/ALP-359)    
Type: Functional, Visual

<!-- include: cypress/integration/blacksmith/progression.js -->

### ALP-x1

progression - State Check- Default view - progression component\
GIVEN - User visits the BS2 course in the default state (no pages in
        the coures have been marked as complete)\
WHEN - The user visits the Progression component\
THEN - The user will see the Progression component's output zones reflect this default state

Page number progression
 - Unit test coverages the calucuation
 - Invoke component and block to create a known state before
   performing a visual assertion

### ALP-x2

progression - State Check-  \'Completed\' state - progression component\
GIVEN - The user has visited all course pages setting them to a 'completed' state
WHEN - The user visits the Progression component\
THEN - The user will see the Progression component's output zones reflect
      this course-completed state

- user first completes all course content
- marking each course page as completed
- seeding course complete-state

<!-- /include: cypress/integration/blacksmith/progression.js -->