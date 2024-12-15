![alt text](./images/AdobeStock_902503425.jpeg "Agile Software Development")
# Introduction to CAB302

This exercise is to familiarise yourself with cloning projects from a remote Git repository. Most of the CAB302 practicals be delivered this way, requiring you to clone the repository containing the practical to your local machine. So it is essential to understand how to clone a remote repository. All of the practical material will be hosted on GitHub so it is worth creating your own personal account on GitHub - we would recommend to use your QUT email address.

There are two detailed guides that have been provided on the CAB302 Canvas site **(Activity 0.1 & Activity 0.2)**. We expect that you will have completed both these activites in advance of Week 1 CAB302 Lecture and Practicals. You will need to complete these activities prior to cloning this repository. If you have not yet done these please complete both activities before attempting to clone this repository.
1. **Activity 0.1** - How to setup the Integrated Development Environment (IDE) required for CAB302
2. **Activity 0.2** - Testing the IDE setup and configuration is correct

There are a number of ways to clone a remote repository, however, for the moment we will be using IntelliJ IDEA. If you prefer to use Git Bash (Bourne Again Shell) and are familiar with the command line utility, then you can certainly go down that path. Most students will probably prefer to let IntelliJ IDEA do all the heavy lifting when starting out working with source/version control. 

## Clone Repository Options
First you will need to start IntelliJ IDEA. When you start IntelliJ IDEA and if you had previously been working on a project that has not been closed, that same project will automatically load when re-starting IntelliJ IDEA. To get access to the controls to clone a remote respository you will need to close the current project. Once the project is closed the Welcome Screen will appear, similiar to the image in figure 1.

![IntelliJ IDEA Clone Repository](./images/cloneRepo1.png)
Figure 1 - IntelliJ IDEA Clone Repository 

The other option is to save any changes to the current project then select **File --> New --> Project from Version Control** (see figure 2)

![IntelliJ IDEA Clone Repository](./images/FileCloneFromVC.png)
Figure 2 - IntelliJ IDEA Clone Repository File Menu

However, if this is your first time launching IntelliJ IDEA, you will be greeted by the IntelliJ IDEA launcher, which will look something like the following in figure 3. Click **Clone Repository**  
![IntelliJ IDEA launcher screenshot](./images/intellij1.png)
Figure 3 - IntelliJ IDEA Clone Repository Welcome Screen/Launcher

### Problems cloning due to GIT

When cloning a repository if you receive an error message stating that Git is not installed, then you need to install Git before attempting to clone the repository again. If you have already completed **Activity 0.1 & Activity 0.2** then you should have already confirmed that Git is installed. If you've installed Git and it still gives you this message, you will need to configure IntelliJ IDEA to explicitly define the Git executable location. The details on how to do this in in **Activity 0.1**. In most cases the problem is due to the incorrect installation order of the IntelliJ IDEA, GIT, and Amazon Corretto Version 21. If you cannot rectify the problem, the best solution is to completely uninstall IntelliJ IDEA, uninstall Git, and most importantly reboot your computer. The follow the installation order of: 
1. Install Git **first**
2. Install IntelliJ IDEA **after** Git has been installed completely.
**NOTE: The is no need to uninstall Amazon Corretto. However, Git MUST be installed before IntelliJ IDEA so the latter will be able to automatically locate Git.**

Follow the instructions in **Activity 0.1** on Canvas as there are detailed instructions and screen-shots to assist the correct installation procedure.

### Clone Repository Dialogue Screen

Regardless of how you are going to clone the repository the same dialogue screen will appear as in figure 4. You will need to get the URL of the repository you want to clone and set the directory where the cloned repository is to be stored on your hard drive. When cloning a repository you will need to select a new directory otherwise an error message will appear that states `"The directory already exists and is not empty"`. It is a good idea to keep your repositories ordered in a consistent way such as by Week Number or Practical Number so you can locate the repositories on your hard drive easily.

![GitHub remote repository HTTPS address](./images/RepositoryURLDialogue.png)
Figure 4 - IntelliJ IDEA Clone Repository Dialogue Screen

You will need to copy the URL of the repository you want to clone from GitHub and paste it in the URL field. To get this address, go to the remote repository and click the **Code** button and make sure to select **HTTPS** to get the correct URL address. 
**Note: You can use SSH however you will need to configure SSH keys (public & private) and load the public key into your GitHub account.** 
This is not in the scope of this exercise however it is not difficult to configure SSH keys and there are many sites that document the process. You will find instructions for Windows, MacOS and Linux, however for the time being we recommend to keep it simple and use the **HTTPS URL Address**.

![GitHub remote repository HTTPS address](./images/RepoURLCopy.png)
You will also need to enter the directory where you want to clone the project into. Once you have completed this select the **Clone** button in IntelliJ IDEA and if everything is correct, the project will be cloned from the remote repository to your hard drive into the directory you specified.

![Clone repository into IntelliJ IDEA](./images/CloneRepoScreen.png).

If a dialog pops up asking if you trust this project, choose to trust it. IDEA should now download the project files and open the project.
![Trust Project IntelliJ IDEA](./images/TrustProject.png).


# Running the project

If all goes well, you should just be able to navigate to **src -> intro -> Introduction** to open up the main source file for the project. From there, click one of the green arrows (either the one next to the class definition or the one next to the main method) and click Run 'Introduction.main()' to run the program, which should show 'Welcome to CAB302' in ASCII art. If the green arrows are not present, look at the top of the source file window - there may be a message there saying that the JDK is not set up. Clicking that message should allow you to select **Amazon Corretto 21** and resolve that problem.
![Run Project in IntelliJ IDEA](./images/RunProject.png).
![Run Project Executed in IntelliJ IDEA](./images/ProjectExecuted.png).
