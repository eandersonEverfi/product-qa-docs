Chart Component 
> com-2827


## COM-2827 - Row 1 - Verifying  default-states charts
GIVEN: User visits the chart component
WHEN: On default vew
THEN: Charts are displayed in the correct default-state
Type of test: Visual w/ applitools
     
Wait for row 1 container and charts to be visible 
cy.waitforEl(chartElements.stackRow1);
cy.waitforEl(chartElements.chartDoughnut);
cy.waitforEl(chartElements.chartPie);
cy.waitforEl(chartElements.chartBar);


TODO:
Need to get charts into a known-state
to be able to wait for = before taking a snapshot
    
Row 1: Taking snapshot of the default state

## COM-2827 - - Interacting with charts via input buttons
GIVEN: User visits an indivisual chart
WHEN: User clicks the provided set of input buttons
THEN: The interacted with chart displays new output data on the chart
     
