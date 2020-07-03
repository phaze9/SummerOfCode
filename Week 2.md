If you can't remember how to do something we already did, look it up in [last week's curriculum](https://github.com/phaze9/SummerOfCode/blob/master/Week%201.md)!

## Day 1: Git and Test :hotsprings:
 - Open the Projects/heroes folder in Visual Studio Code
   - Open the Source Control tab
   - Note that many new files are listed
   - These were created by the "ng build" command we ran yesterday
 - Edit the file .gitignore
   - Add a new line at the end
     ```
     /dist
     ```
   - And save the file using Cmd/Ctrl-S
   - Now you should only have one outgoing change, the file .gitignore
 - Click Synchronize Changes :doughnut: in the blue bar on the bottom left of Visual Studio
   - Open your heroes repository on the GitHub website
   - Notice how all your changes from yesterday  are visible there
 - Go back to the Source Control tab in Visual Studio
   - Enter a commit message: Updated .gitignore
   - Add the file .gitignore :heavy_plus_sign:
   - And commit  
 - Yesterday you might have noticed that some tests we ran in the Terminal failed
   - We broke these when we changed the application two days ago
   - Let's fix them!
 - Open a Terminal and change to the ~/Projects/heroes folder
   - Then run
     ```
     ng test
     ```
   - One test succeeded, two failed
 - AppComponent > should have as title 'heroes'
   - Open the file app.component.spec.ts in Visual Studio
   - Change line 22 until the test succeeds
     - The test is rerun automatically when you save the file
   - Look at the [changes we did at the end of day 6](https://angular.io/tutorial/toh-pt0#change-the-application-title) to get an idea what you need to fix 
 - AppComponent > should render title
   - Change line 29 in the same file to
     ```
     expect(compiled.querySelector('h1').textContent).toContain('Tour of Heroes');  
     ```
 - Don't forget to commit and synchronize your changes
 
