# Summer Of Code ☀️

![Logo](https://github.com/phaze9/SummerOfCode/blob/master/SummerOfCode.png?raw=true)

Let's learn how to code! On GitHub you can develop lot's of fun stuff, even games! It is challenging, fun and rewarding to learn coding, so get ready 🚀

If you get stuck: Ask Google, play around until it works or find a tutor.

## Day 1: GitHub
GitHub is where developers meet.
- Check out the [GitHub](https://github.com) website, create an account and find out how it works. 
- Follow phaze9.
- Install the GitHub app.

## Day 2: Fork SummerOfCode🍴
The GitHub website is great for small changes.
- [Fork](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) the SummerOfCode project.
- Edit the file README.md to improve the instructions for SummerOfCode. 
  -  Find out how [Markdown](https://guides.github.com/features/mastering-markdown/) syntax works.
- Submit a [pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork) for your changes from the GitHub web interface.

## Day 3: Visual Studio Code
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
  
## Day 4: Terminal
The terminal/shell is old but gold.
- Open a Terminal window, then  copy or type the commands listed below (text with gray background).
- Change to the project directory
    ```
    cd ~/Projects/SummerOfCode
    ```
- Add the phaze9 version to your SummerOfCode repository
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
- Edit the file README.md in VisualStudio
- Create a pull request for README.md from the GitHub tab in VisualStudio
  - [Working with GitHub in VS Code](https://code.visualstudio.com/docs/editor/github)
