# Week 3: Code Away :surfer:

This week we're getting serious about coding.

## Day 1: You have more Heroes :two_women_holding_hands:
List and style your heroes.
 - Before you start coding, run the app
 - [Create mock heroes](https://angular.io/tutorial/toh-pt2#create-mock-heroes)
   - Feel free to add your own heroes!
 - [Displaying heroes](https://angular.io/tutorial/toh-pt2#displaying-heroes)
   - Add missing code to heroes.component.ts, don't remove the existing
 - [List heroes with *ngFor](https://angular.io/tutorial/toh-pt2#list-heroes-with-ngfor)
   - You should now see your heroes in the browser
 - [Style the heroes](https://angular.io/tutorial/toh-pt2#style-the-heroes)
   - Our file is called "heroes.component.scss"
   - Add the styles from [heroes.component.css](https://angular.io/tutorial/toh-pt2#final-code-review)
 - Last but not least: Commit your changes
 
## Day 2: Master / Detail :mag:
When the user clicks a hero in the master list, the component should display the selected hero's details at the bottom of the page.
 - Before you start coding, run the app
 - [Add a click event binding](https://angular.io/tutorial/toh-pt2#add-a-click-event-binding)
 - [Add the click event handler](https://angular.io/tutorial/toh-pt2#add-the-click-event-handler)
 - [Add a details section](https://angular.io/tutorial/toh-pt2#add-a-details-section)
 - [Style the selected hero](https://angular.io/tutorial/toh-pt2#style-the-selected-hero)
 - Don't forget to commit your changes
 
## Day 3: Split your App :broken_heart:
Split the heroes component in two. 
 - [Create a feature component](https://angular.io/tutorial/toh-pt3#create-a-feature-component)

## Day 4: Serve the Heroes :nail_care:
Services provide access to your app's data.
 - [Add services](https://angular.io/tutorial/toh-pt4)
 - Make sure to read all the explanations, so you gain a deeper understanding

## Day 5: Navigate your Heroes :ship:
Your app needs more than one screen.
 - [Add in-app navigation with routing](https://angular.io/tutorial/toh-pt5)
 - Make sure to read all the explanations, so you gain a deeper understanding  

## Day 6: Fix the Tests :sweat_drops:
We wrote a lot of code and forgot about the automated tests.
 - Go to your app's repository on the GitHub website
   - Check for commits by your tutor
   - Review them and synchronize in Visual Studio Code
 - Make sure all your unit and e2e tests still pass
   ```
   ng test
   ```
   ```
   ng e2e
   ```
   - You should always run your tests after you made changes, they will be easier to fix then
 - Repair problems in the unit tests
   - You will need to adjust heroes.component.spec.ts to the changes you did in heroes.component.ts
   - We now have a list of heroes instead of a single hero
     - Let's check the name of the first hero
   - Replace
     ```
     expect(component.hero.name).toEqual
     ```
   - By
     ```
     expect(component.heroes[0].name).toEqual
     ```
   - Now rerun
     ```
     ng test
     ```
   - You should be able to fix the problem now
 - Repair problems in the e2e tests

## Day 7: Go Mobile :iphone:
Put your app on your phone!
 - Install the NativeScript command line interface
   ```
   npm install --global nativescript
   ```
 - Add NativeScript to your app
   ```
   ng add @nativescript/schematics
   ```
 - Run your app to check that it still works as before in the web browser
 - Build the NativeScript app
   ```
   tns preview
   ```
