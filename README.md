# Gearheader
Library with Robot Classes (as of now form 2018-19) Very primitive at moment
## Installation (for both first time installaiton and first time pulls from a remote repository)
### Downloading
#### Option A. In Command Line (for those using Git Submodules)
1. Go to your project folder in the command line
2. Run `git submodule init`
##### Varient 1. First time installation to repository
3. Run `git submodule add https://github.com/FTC-Team-5197-Gearheads/Gearheader.git`
##### Varient 2. Downloading to a repo that already references this submodule in `.gitmodules`
3. Delete the `Gearheader` directory in your project folder
4. Run `git submodule update `
5. In Android Studio do a sync `File -> Sync with File System` and `File -> Sync with Gradle File System`. You are done! No need to do the next steps below.
#### Option B. Manual Installation (for those who do not want to use Git)
1. Download the Zip file from the latest (or desired )version in [Releases](https://github.com/FTC-Team-5197-Gearheads/Gearheader/releases)
2. Unzip it
3. Move it under the directory of your current Android Studio Project
### In Android Studio (for all methods)
4. Open your project in Android Studio and choose `File -> Sync with File System`
5. Choose `File -> Sync Project with Gradle Files`
6. Open `settings.gradle` and add this line: `include ':Gearheader'`. For those doing manual installation its `include ':Gearheader-[Version Number]'` (basically, it should match the name of the folder)
7. Open the `build.release.gradle` file under `TeamCode` (or wherever you will be writing your code) and add this line: `implementation project(':Gearheader')` within the curly brackets
8. Repeat step 7 for the `build.release.gradle` file under `FtcRobotController`
9. Repeat step 5
10. To test, go ahead and try to make an object of type `Lookeebot`. (make sure the editor imports `edu.boscotech.gearheads.gearheader.samplerobots`). If no errors arise, you are good to go.
### In Command Line (for Git Submodules (Option B))
11. Then after, make sure to go back to the parent respository of your current project and commit these changes. 
## Maintainence
### For those who installed using Option A
1. Run `git pull` from the submodule directory (`[Your Project]/Gearheader`)to be up to date. Don't worry. Only stable changes will be pushed on master. Then in the parent repo, commit these chabges
### For those who installed Option B
1. Repeat steps for Installation
## Adding features
1. Feel free to fork this library and send pull requests. 
