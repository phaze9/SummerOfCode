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
   - Notice how you now only have one outgoing change, namely the file .gitignore
 - Click Synchronize Changes :doughnut: in the blue bar on the bottom left of Visual Studio
   - Open your heroes repository on the GitHub website
   - Notice how all your changes are visible there
 - Go back to the Source Control tab in Visual Studio
   - Enter a commit message: Updated .gitignore
   - Add the file .gitignore
   - And commit  
