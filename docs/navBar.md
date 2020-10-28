# Nav Bar component
> Dev implemntation ticket: [COM-1462](https://everfi.atlassian.net/browse/COM-1462)    
Type: Functional, Visual  

<!-- include: cypress/integration/navBar.js -->

### COM-2930

Nav Bar - When visiting the Nav Bar component - the menu is closed by default\
WHEN- user visits the Nav Bar component\
THEN- user see the component in its default state

Wating on  component elements

visual check -  Default View

### COM-2930

Nav Bar - Clicking the menu button expands the menu drawer\
WHEN: User clicks the MENU button\
THEN: The drawer menu expands to a visible state

user clicks the menu button

After clicking the menu button wait for drawer to be visible
drawer should have / be populated with descendants of `div`\

visual check - menu drawer in the expanded state

### COM-2930

Nav Bar - The expanded menu drawer has two tabs - Navigation & Progress - both containing content\
GIVEN- The menu drawer is in its expanded state\
WHEN- User clicks on either drawer tabs\
THEN- The user will be able to see each of the tabs content

After clicking the menu button wait for drawer to be visible
drawer should have / be populated with descendants of `div`\

GIVEN- Tab1 - on initial view of expanding drawer
THEN- Tab1 will be active and in a visited state\

tab1's content pane has 79 `li` document-activity element links

GIVEN- User clicks tab2
WHEN- Tab2 is visible and active\
THEN- Tab2's contnet is visible

default-state- progressionDonut_1 = 8% percent graphed

default-state - progressionDonut_1 =  has 8% text

visual check -  menu Second Menu Tab Expanded

### COM-2930

Nav Bar - Clicking an expanded menu causes the drawer to close\
GIVEN- Menu drawer is in the expanded-state\
WHEN- The user clicks Menu's xClose button\
THEN- Menu's draeer element closes from view

After clicking the menu button wait for drawer to be visible
drawer should have / be populated with descendants of `div`\

GIVEN- The menu drawer is expanded
WHEN- the user clicks the Xclose button\
THEN- The drawer menu is closed

WITH- the drawer menu closed
THEN- The drawer menue has a `hidden` style attribute\
THEN- The drawer menuy is not visible

visual check - After Drawer is closed

### COM-2930

Nav Bar - Progerssion Graph correctly displays its completed-state\
GIVEN- The user has visited all course pages setting them to a 'completed' state\
WHEN- The user expands menu's drawer\
AND- Clicks tab2\
THEN- the Progression component's output zones reflect this course-completed state

user first completes all course content
marking each course page as completed\

user visits the Progression component after completing all other course pages

user expands menu and clicks tab2

Need to wait for tab2's content to be visible, before taking a snap

completed-state- progressionDonut_1 = 16% percent graphed

completed-state - progressionDonut_1 =  has 8% text

visual check - menu -  Second Menu Tab Expanded with progression graph in completed-state

<!-- /include: cypress/integration/navBar.js -->