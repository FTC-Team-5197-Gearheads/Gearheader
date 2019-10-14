# Gearheader
Library with Robot Classes (as of now form 2018-19) Very primitive at moment
## Installation on to a Git Version Controlled Project via Git Submodule
### In Command Line
1. Go to your project folder in the command line
2. Run `git submodule init`
3. Run `git submodule add https://github.com/FTC-Team-5197-Gearheads/Gearheader.git`
### In Android Studio
4. Open your project in Android Studio and choose `File -> Sync with File System`
5. Choose `File -> Sync Project with Gradle Files`
6. Open `settings.gradle` and add this line: `include 'HOMAR-FTC-Library`
7. Open the `build.release.gradle` file under `TeamCode` (or wherever you will be writing your code) and add this line: `implementation project(':Gearheader')` within the curly brackets
8. Repeat step 7 for the `build.release.gradle` file under `FtcRobotController`
9. Repeat step 5
10. To test, go ahead and try to make an object of type `Lookeebot`. (make sure the editor imports `edu.boscotech.gearheads.gearheader.samplerobots`). If no errors arise, you are good to go.
### In Command Line
11. Then after, make sure to go back to the parent respository of your current project
## Maintainence
1. Run `git submodule update --remote` to be up to date with changes in the master branch.
## Adding features
1. Feel free to fork this library and send pull requests. 
