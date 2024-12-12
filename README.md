![alt text](./images/AdobeStock_902503425.jpeg "Agile Software Development")
# Introduction to CAB302

This exercise is to familiarise you with cloning projects from a remote Git repository so that you can work on them in IntelliJ IDEA on your own machine. Most CAB302 practicals will work this way - the first step you will take is cloning a Git repository.

First, you need to run IntelliJ and get ready to clone from a remote version control system. There are two main ways you might do this. Note that these instructions are for Windows, but everything should be fairly similar in Linux and MacOS (Git will not have the filename `git.exe`, of course).

### Confirm Git Installation

When you launch IDEA, if you had a project open when you last used it, that project will re-open automatically. If the last project was closed, you may also have a list of recently opened projects displayed on the welcome screen.
![IntelliJ IDEA launcher screenshot](./images/IntelliJStartUpOptions.png)

However, if this is your first time launching IDEA or you closed the current project, you will be greeted by the IntelliJ IDEA launcher, which will look something like the following **(Note: The version numbers may be slightly different depending on the installation date)**:
![IntelliJ IDEA launcher screenshot](./images/intellij1.png)

From here, you can click **'Get from VCS'** to clone a project from a remote repository. If you try this and you get a message saying that Git is not installed, then you need to install Git first. If you've installed Git and it still gives you this message, you will need to configure IntelliJ IDEA to explicitly define the Git executable location.

From the File menu in IntelliJ IDEA, click 'Settings', then select 'Version Control', and finally Git. The screen will appear as shown below with a section to enter 'Path to Git executable'. In Windows, it will generally be in 'Program Files\Git\cmd\git.exe'. The important point is that you need to provide the location of 'git.exe' and not just the install directory for Git. 
![IntelliJ Settings Version Control](./images/GitConfigCorrect.png)

There is a folder icon you can use to browse with Windows explorer to help locate the Git executable. If you followed the CAB302 IDE Configuration Video setup guide then hopefully this will not be an issue. However, if you installed the applications in the wrong order then it is possible IntelliJ IDEA does not know the Git executable location. 
![IntelliJ Settings Version Control Not Installed](./images/GitNotInstalled.png)

Once you have located the Git exectable there is a 'Test' button in the Version Control section of IntelliJ IDEA settings - click the 'Test' button and if you have found the Git executable (git.exe) then the display will show the version installed on your system.
**NOTE: Do not check 'Set this path only for the current project'** as you will need Git for the entire semester in CAB302.
![IntelliJ Settings Version Control Git Testing](./images/SelectingGitIntelliJ.png)

### Cloning a project from within IntelliJ IDEA 

If you already working in IntelliJ, and you need to clone a repository, you will instead need select **File -> New -> Project from Version Control**. This will open up a dialog similar to the image below. If Git is not installed properly, refer to the previous section to configure Git.

You will need to copy the project's URL from GitHub and paste it in the URL field. To get this address, go to the remote repository and click the **Code** button and make sure to select **HTTPS** to get the correct URL to clone. 
![GitHub remote repository HTTPS address](./images/URLRemoteRepo.png)
You will also need to enter the directory where you want to clone the project into. Once you have completed this select the **Clone** button in IntelliJ IDEA and if everything is correct, the project will be cloned from the remote repository to your hard drive into the directory you specified.
![Clone repository into IntelliJ IDEA](./images/CloneRepoScreen.png).

If a dialog pops up asking if you trust this project, choose to trust it. IDEA should now download the project files and open the project.
![Trust Project IntelliJ IDEA](./images/TrustProject.png).

### Cloning a project IntelliJ IDEA Start screen

You can select **Clone Repository** from the IntelliJ IDEA Welcome Screen. If you click **Clone Repository** the same dialog screen will appear as before and you will still need to enter the URL of the project you want to clone, as well as select the destination directory on your hard drive. Once this is completed and you click **Clone** the project will load into IntelliJ IDEA.
![Clone repository into IntelliJ IDEA](./images/RepoCloned.png).

# Running the project

If all goes well, you should just be able to navigate to **src -> intro -> Introduction** to open up the main source file for the project. From there, click one of the green arrows (either the one next to the class definition or the one next to the main method) and click Run 'Introduction.main()' to run the program, which should show 'Welcome to CAB302' in ASCII art. If the green arrows are not present, look at the top of the source file window - there may be a message there saying that the JDK is not set up. Clicking that message should allow you to select **Amazon Corretto 21** and resolve that problem.
![Run Project in IntelliJ IDEA](./images/RunProject.png).
![Run Project Executed in IntelliJ IDEA](./images/ProjectExecuted.png).