# Menu Item component
> Dev implemntation ticket: [COM-2930](https://everfi.atlassian.net/browse/COM-2930)    
Type: Functional, Visual  

<!-- include: cypress/integration/blacksmith/menuItem.js -->

### COM-2930

Menu Item - When visiting the Menu Item component - the menu is closed by default\
WHEN- user visits the Menu Item component\
THEN- user see the component in its default state

Wating on  component elements

visual check -  Default View

### COM-2930

Menu Item - Clicking the menu-1 button expands the menu drawer\
WHEN: User clicks the MENU button\
THEN: The drawer menu expands to a visible state

user clicks the menu-1 button

After clicking the menu-1 button wait for drawer to be visible
drawer should have / be populated with descendants of `div`\

visual check - menu-1 drawer in the expanded state

### COM-2940

Menu Item - The expanded menu-1 drawer has two tabs - Navigation & Progress - both containing content\
GIVEN- The menu-1 drawer is in its expanded state\
WHEN- User clicks on either drawer tabs\
THEN- The user will be able to see each of the tabs content

After clicking the menu-1 button wait for drawer to be visible
drawer should have / be populated with descendants of `div`\

GIVEN- Tab1 - on initial view of expanding drawer
THEN- Tab1 will be active and in a visited state\

tab1's content pane has 93 `li` document-activity element links

GIVEN- User clicks tab2
WHEN- Tab2 is visible and active\
THEN- Tab2's contnet is visible

default-state- progressionDonut_1 = 18% percent graphed

default-state - progressionDonut_1 =  has 18% text

visual check -  Menu-1 - Second Menu Tab Expanded

### COM-2930

Menu Item - Clicking an expanded menu causes the drawer to close\
GIVEN- Menu-1 drawer is in the expanded-state\
WHEN- The user clicks Menu-1's xClose button\
THEN- Menu-1's draeer element closes from view

After clicking the menu-1 button wait for drawer to be visible
drawer should have / be populated with descendants of `div`\

GIVEN- The menu-1 drawer is expanded
WHEN- the user clicks the Xclose button\
THEN- The drawer menu is closed

WITH- the drawer menu closed
THEN- The drawer menue has a `hidden` style attribute\
THEN- The drawer menuy is not visible

visual check - Menu-1 - After Drawer is closed

### COM-2930

Menu Item - Menu-1- Progerssion Graph correctly displays its completed-state\
GIVEN- The user has visited all course pages setting them to a 'completed' state\
WHEN- The user expands Menu-1's drawer\
AND- Clicks tab2\
THEN- the Progression component's output zones reflect this course-completed state

user first completes all course content
marking each course page as completed\

user expands Menu-1 and clicks tab2

Need to wait for tab2's content to be visible, before taking a snap

completed-state- progressionDonut_1 = 33% percent graphed

completed-state - progressionDonut_1 =  has 33% text

visual check - Menu-1 -  Second Menu Tab Expanded with progression graph in completed-state

### COM-2930

Menu Item - Modal - Component Visual Check\
GIVEN- The Menu Item - Modal component page loads\
WHEN- An Applitools visual test is engaged\
THEN- The baseline screengrab will match the running test's snapshot

<!-- /include: cypress/integration/blacksmith/menuItem.js -->