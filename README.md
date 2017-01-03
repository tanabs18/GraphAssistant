# GraphAssistant
Graphing Assistant for Use in Algebra and Calculus Classes
## Setting up React-Native (Enabling your computer to run the app)
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

## Setting up the App
1. Clone the app
  ```
  
  ```
## Contributing
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D
## History
TODO: Write history
## Credits
TODO: Write credits
## License
TODO: Write license
