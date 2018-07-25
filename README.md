# Angular-Developer

## Code source
Code example comes from Angular tutorial: [Tour of Heroes](https://angular.io/tutorial)<br>
Direct link: https://angular.io/generated/zips/toh-pt6/toh-pt6.zip

## User tasks

### Hero age

- As a User I want to be able store hero age
  - age is positive integer number
  - hero must be at least 18 years old, and cannot be older that 500 years
    - validation required
    - show red message next to age edit control
  - age isn't presented on list of heroes
  - age value is optional
  
### Hero experience

- As a User I want to see hero experience on hero details screen
  - hero level is presented below hero age input
  - there are following experience values:
    - junior for age below 100
    - professional for age >=100 and <250
    - expert for age >=250
    - undetermined for empty age
    
### Messages section
- As a User I want to not see messages section on production environment
  - keep it for development only
  
### Navbar buttons
- As a User I want see highlighted current navigation button
  - for route `/dashboard` button Dashboard should be highlighted
  - for route `/heroes` button Heroes should be highlighted
  - for other routes no navigation button highlighted

### Hero search
- As a User I want search result to appear after at least two chars typed

- As a User I want search result style to be dependent on hero experience
  - green text color for junior
  - black text color for professional
  - blue  text color for expert
  - gray test color for undetermined

### Heroes list
- As a User I want to see hero's age and experience on heroes list

- As a User I want to see total number of heroes below list
  - just below list paragraph should appear
  - content: "Total number of heroes is: x."

### changes in progress
- As a User I want unsaved data to be protected 
  - all route changing operations (like nav bar or back button) should check for unsaved data
  - checking should work for changing details and adding new hero
  - the simple confirmation message should be displayed, like: your data could be lost, are you sure yes/not?
  - when user choose 'yes', route change can go on
  - when user choose 'no', route change should be canceled

## Refactoring tasks

### Model driven forms
- please refactor all forms to be model driven

### observable and async
- please refactor lists to expose observable to template, and use `async` pipe to get value

### SCSS
- please refactor code to use SCSS instead of CSS

## Technical tasks

### ng lint
- command `ng lint` does not work, please fix the problem

### code coverage
- unit test code coverage analytics does not work, please fix problem
- `ng test -cc` should produce code coverage report
- **all your code should be reasonable covered by unit and protractor tests**
