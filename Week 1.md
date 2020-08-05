# Week 1: Get Started :construction:

## Day 1: GitHub :cat:
GitHub is where developers meet.
- Check out the [GitHub](https://github.com) website, create an account and find out how it works
- Follow phaze9
- Install the GitHub mobile app

## Day 2: Fork SummerOfCode :fork_and_knife:
The GitHub website is great for small changes.
- [Fork](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) the SummerOfCode project
- Edit the file README.md to improve the instructions for SummerOfCode
  - Find out how [Markdown](https://guides.github.com/features/mastering-markdown/) syntax works
  - [Markdown Emojis](https://gist.github.com/rxaviers/7360908)
  - Use the 'Preview changes' button to see the formatted text
- When you are finished, commit your changes
  - Briefly describe what you did in the Commit changes text field 
- Submit a [pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork) for your changes from the GitHub web interface

## Day 3: Visual Studio Code :floppy_disk:
Serious development requires serious tools.
- Install [Visual Studio Code](https://code.visualstudio.com/)
- Install the [GitHub Pull Requests and Issues extension](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)
  - From the Extensions tab on the left side of Visual Studio
  - You should now have a new GitHub tab in the Visual Studio sidebar
- [Install Git](https://git-scm.com/download/)
  - The Source Control tab in the sidebar should no longer complain that Git is not installed
- Setup the SummerOfCode project from your GitHub fork
  - Create a new folder "Projects" under your user directory in Explorer or Finder
  - Clone your repository from GitHub into Projects under the Source Control tab
  
## Day 4: Terminal :computer:
The terminal/shell is old but gold.
- Open a Terminal and go to the SummerOfCode project:
  - On Mac/Linux:
    - Open a Terminal window, then  copy or type the commands listed below (text with gray background).
    - Change to the project directory
    ```
    cd ~/Projects/SummerOfCode
    ```
  - on Windows: 
    - Open an Explorer window, navigate to your Projects directory, right-click on "SummerOfCode" and choose "Git Bash here"
- Add the phaze9 version to your SummerOfCode repository AFF
    ```
    git remote add upstream https://github.com/phaze9/SummerOfCode.git
    ```
- Pull the latest changes from phaze9/SummerOfCode
    ``` 
    git pull upstream master
    ```
- Apply the changes to your version on GitHub
    ```
    git push
    ```
- Edit the file README.md in Visual Studio Code
- Create a pull request for README.md from the GitHub tab in Visual Studio
  - [Working with GitHub in VS Code](https://code.visualstudio.com/docs/editor/github)

## Day 5: Sharpen your Tools :key:
A tiny bit more setup work and you're good to go.  
 - Tell git who you are
   - Enter the following commands in a Terminal window (On Windows: use the "Git Bash" window)
   - Replace First Last by your first and last names
     ```
     git config --global user.name "First Last"
     ```
   - Replace my@email.com by the email address you used to sign up for GitHub
     ```
     git config --global user.email my@email.com
     ```
   - Verify the configuration
     ```
     git config -l
     ```
 - Download and install the LTS (long term support) version of [Node.js](https://nodejs.org/)
 - Finally we will install the Angular CLI (command line interface) from a Terminal window
   ```
   sudo npm install -g @angular/cli
   ```
   - On Windows: open the PowerShell and type
     ```
     sudo npm install -g @angular/cli
     ```
 - Verify the installation by listing the available Angular commands
   ```
    ng
   ```
   - On Windows: you might need to use 
     ```
     npx ng
     ``` 
     in the PowerShell    

## Day 6: Angular Heroes :ok_woman:
Angular is a great way to conquer the web.
 - Change to your Projects folder in a terminal window
   ```
   cd ~/Projects
   ```
 - Create the Heroes application
   ```
   ng new heroes
   ```
   - Would you like to add Angular routing? (y/N) 
     - Enter / Return to confirm (We will add routing later)
   - Which stylesheet format would you like to use?
     - Use arrow keys to select SCSS, confirm with Enter
 - Change to the application folder
   ```
   cd heroes
   ```
 - Run the application
   ```
   ng serve --open
   ```
 - Now open the heroes folder in Visual Studio Code
   - Select File -> Open from the menu, then choose the heroes folder
 - [Make changes to the application](https://angular.io/tutorial/toh-pt0#make-changes-to-the-application)
   - Observe how the app changes in your web browser after each of the following steps
     - Don’t forget to save the changes in Visual Studio
   - [Change the application title](https://angular.io/tutorial/toh-pt0#change-the-application-title)
   - [Add application styles](https://angular.io/tutorial/toh-pt0#add-application-styles)
     - Our style file is called styles.scss
 
## Day 7: Back to GitHub :arrow_backward:
Publish your work on GitHub and run the tests.
 - Open the Source Control tab in Visual Studio
   - Enter a commit message: Changed application title and styles
   - Click the :heavy_plus_sign: button next to the three files you changed yesterday
   - Commit the changes using the :heavy_check_mark: button
 - Click on the three dots icon on the top right of the Source Control tab
   - Select Publish Branch...
   - Hit Return to publish to a new heroes repository on your GitHub
   - In the list of files to include deselect the folowing
     - .DS_Store (if it exists)
     - .git
     - node_modules
   - Press OK
 - Now open your [GitHub](https://www.github.com/) in the browser
   - Click on Repositories and look at the contents of your new private heroes repo
   - Read the instructions for your heroes app on GitHub
 - Make sure you have the Chrome browser installed: [Chrome](https://www.google.com/chrome/)
 - Run the following commands in a Terminal and watch what they do
   - Always change to your application folder first
     ```
     cd ~/Projects/heroes
     ```
   - Build your application
     ```
     ng build
     ```
   - Run the unit tests
     ```
     ng test
     ```
     - Press Ctrl-C in the Terminal to stop
   - Run the end-to-end tests
     ```
     ng e2e
     ```
   - Start the application like we did yesterday
     ```
     ng serve --open
     ```
