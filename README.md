# GraphAssistant
Graphing Assistant for Use in Algebra and Calculus Classes

## What is GitHub?
Officially, GitHub is a "web-based Git repository hosting service". In laymans terms, it's a free online service to store and share code. In more technical terms, "Git" is a freely availible version control software, and GitHub is where it's all stored. It allows you to revert to previous versions of your codebase, as well as create copies, known as branches, of the code and merge them (allowing multiple people to edit code at the same time). 

Every project is stored in what's called a repository, or "repo" for short, which is linked to your user account. This allows each repo to be accessed at github.com/USERNAME/REPONAME. Editing a shared codebase on GitHub follows a simple procedure:

1. Create an account!
2. Fork the repo

   This means making a copy of the repo. This is a way to make sure you can play with the code however you like, and keep it separate from the production (in use) code. You can keep this code up to date by syncing it, but we'll get to that later.

3. Create a branch (optional)

   Branches are copies of the code (which is techincally also a copy). While the main code resides on the "Master" branch, features in development have their own branches. For example, if you were building a new toolbar, but also adding a search feature, you would create two branches, hypothetically named "Toolbar" and "Search." The purpose of this is to prevent a small bug in the Toolbar from preventing testing the Search function. 

   While often times branching code is used as an alternative to forking code, we won't be doing this. It does offer the benefit of others seeing and editing your branches, but it's literally harder to do (more commands). Instead you can use branches to keep your own code separated if you desire.

4. Make your edits
5. Commit!

   There are three levels of saved files in Git. The first is your working directory, which is updated every time you save your code. The second is the staging area, where code is permenantly saved on to your local disk. This is done by what's called "committing." Commits must be paired with a message, which generally explains what edits are contained. Messages typically look something like "Update readme.md" or "Fix toolbar bug." The grammar is weird.

6. Pull your changes

   The hird level of saved files in Git is the official repo. While you can "push" commits to your own individual project repos, there are often conflicting commits within shared codebases. This is solved by using "pull". This pushes the code to the official repo, but does not add it to the actual codebase. Instead, others can edit and make comments to your commit, until it is deemed satisfactory. Then it is "merged," where it replaces the old code.

## Getting Started on the Project

### Set up React-Native (Enable your computer to run the app)


1. Make sure you have Mac OS Version 10.11.5 or later
2. Install Xcode 8 or later
3. Open Xcode and navigate to Preferences->Components
4. Install Command Line Tools and iOS 10.1 Simulator
5. Test the simulator by navigating to Xcode->Open Developer Tool->Simulator
6. Install Homebrew by pasting the following command into Terminal

  ```
  /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
  ```
7. Install [npm](https://nodejs.org/en/)
8. Make sure the iOS Simulator is downloaded and functional (Availible under m
9. Install the React-Native dependencies by pasting the following commands into Terminal

  ```
  brew install node
  brew install watchman
  ```
10. Install React-Native by pasting the following command into Terminal

  ```
  npm install -g react-native-cli
  ```
  Note: If you get a permission error, paste the following command instead
  
  ```
  sudo npm install -g react-native-cli
  ```
  If you get the error "Cannot find module 'npmlog'" paste the following command and then try again
  
  ```
  curl -0 -L http://npmjs.org/install.sh | sudo sh
  ```
11. Test that it all works by pasting the following commands (one at a time)

  ```
  mkdir ~/Documents/React-Native-Projects
  cd ~/Documents/React-Native-Projects
  react-native init TestProject
  cd TestProject
  react-native run-ios
  ```

### Setting up the App
1. Fork the app

   First click fork on the project page, then click "Clone or download," copy the URL, and enter the following commands (substitute the URL where shown)
   
  ```
  cd ~/Documents/React-Native-Projects
  git clone URLGOESHERE
  git remote add upstream https://github.com/tanabs18/GraphAssistant.git
  git remote -v
  ```
  
2. Run it!

  ```
  cd ~/Documents/React-Native-Projects
  react-native run-ios
  ```
  
3. Update it (when necessary)

  ```
  cd ~/Documents/React-Native-Projects
  git fetch upstream
  git checkout master
  git merge upstream/master
  ```
  
## How to contribute (Commands included)

## Credits (In no particular order)
| Management | Programmers |
| :-------------: |:-------------:|
| Mr. Feldman | Brian Tanabe |
| Alexander Czarnecki | Armin Thomas |
| Bradley Hart | William Ryan |
