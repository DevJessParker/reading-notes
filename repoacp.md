# HELP! Repo to ACP Detailed Process Guide

This week is going to push us all outside our comfort zones. That's okay! Take a look at what we've done today. Could we have done this yesterday? Probably not. I know *I* couldn't do this before!

Learning is uncomfortable and we're all going to make mistakes. That's okay, too.

Here is my step-by-step guide to:

- Creating a Repo on GitHub
- Setting up your Repo
- Finding your location within your Terminal 
- Git cloning your repo down to your local system via your Terminal
- Opening your Repository files in VS Code
- Editing your file
- Saving Changes
- Performing an ACP
- Viewing your changes on your live website
- Troubleshooting and Tips

## Creating a Repo on GitHub

To create a New Repo on GitHub, perform the following steps:

1. Log in to [GitHub](https://www.github.com/)

2. In the upper right hand corner, click on your photo. You can also click on the dropdown arrow beside the photo avatar circle.

3. Select **My Repositories**

4. You'll be taken to a new page that lists all your current Repositories. Click the green button that says "NEW"

>Pay very close attention to these next steps. Go slowly, as it can be a bit tricky. Think of a Repository as a giant master closet that holds all the pages for a certain project. That is why you will have a **reading-notes** repository **AND** a repository for your html website \(which you will name yourself depending on your topic\). Those are *two different projects* and each needs its own Repository. However, your reading notes for each class are all part of the "Reading Notes" project, so exist inside the **reading-notes** Repository.

### Now, let's set up a new example Repository. For the following example, I'm going to pretend we are setting up our **reading-notes** Repository for the first time. You do **NOT** need to repeat this setup if you already have your **reading-notes** Repository built in GitHub. However, if you need to build a new Repository, or need help building one for your upcoming HTML project, these steps will be the same. Just substitute your own Repository name for **reading-notes**. It will still be located in the **code102** folder, which we will learn about below.

5. Name your new repository. Do **NOT** use capital letters. Do **NOT** use spaces. Dashes ( - ) and Underscores ( _ ) are okay.

6. Add a short **description** of your repository.

7. Make sure your repository is marked **PUBLIC**

8. Click **"Add a README.md file"**

9. Click **"Create Repository"**

### Congrats! You now have a brand new closet where you can store all the GitHub pages relating to this particular project. Now, let's **SET UP YOUR NEW REPOSITORY** with a few more steps. Pay very close attention here, as you need to closely follow these directions.

## Our goal right now is to deploy the repository so it can have a live URL homepage. 

10. You should be on the dashboard home for your new repository. Click on the **SETTINGS** gear in the toolbar.

11. On the lefthand side, scroll down the vertical tab list until you see the tab marked **PAGES.** Click this tab now.

12. Under **SOURCE**, click the **BRANCH** dropdown and select **MAIN**

13. Click the button marked **SAVE**

14. You should now have a message providing you a link to your live website.

15. Highlight and copy that link.
    - For MAC users, the shortcut to copy is **COMMAND C**
    - For Windows users, the shortcut to copy is **CTRL C**

16. On the upper left side of your screen, you will see a **breadcrumb** that lists your UserName/name-of-your-repository. This may be blue in color. Specifically click on the **name of your repository**, as this will take you back to that repository's dashboard home.

17. On the dashboard home page, on the right hand side, in the **ABOUT** section, click on the gear symbol.

18. Under **WEBSITE** paste your previously copied link.
    - For MAC users, the shortcut to paste is **COMMAND V**
    - For Windows users, the shortcut to copy is **CTRL V**

19. Click **SAVE CHANGES**

### Now that our repository has been created in GitHub, and we have assigned it a URL, we will **NOW STOP EDITING THE REPOSITORY IN GITHUB**. Moving forward, we will be editing this repository using our coding tools on our local system.

### However, right now our Repository only exists on GitHub. We need a way to create a connection between GitHub and our local system editing tools \(Our Terminal/Ubuntu and VS Code\)

20. While you're still in GitHub, on your Repository's home dashboard screen, click the green **CODE** button.

21. You will see a popup labeled **CLONE** that shows a URL link. Copy this link.

>### Be sure you grab the link under the **CODE** button. You will need this link shortly.


## Let's Get Moving!

Now we're ready to create a connection between GitHub and the editing tools on our local computer. To make sure we're ready to go, let's do a couple steps first.

22. Open your Terminal.

### Before we start throwing files around all willy nilly in our Terminal, let's make sure we know *where* those files are going. But first, where are *we* in our Terminal? It may help to think of this as if you are a character in a video game filled with rooms. Before you can complete your mission in a certain room \(or folder, in our case\) we need to know:

Question | Video Game Example Question
------------ | ------------
Where are we currently located in our directory? | Which room are we in?
How do we get to our target location from our current location? | How do we change rooms?

## Let's get back to business.

23. When setting up the folders on our computer, we used our Terminal to create **paths**. Paths are the hallways and directions that lead us to the rooms. The folders we created as a class were named **projects**, **codefellows**, and **code102**
----------------

24. *If you did **NOT** set up folders using the mkdir command earlier in the class, or if you can't remember these steps, I recommend you stop here and contact a TA or the instructor. They can help explain how to set up your folder pathways using your Terminal.*
-----------------

25. You should have set up the following folders and sub-folders, in this order:
- projects
    - codefellows
        - code102

Remember: Folders are like nesting dolls. **code102** exists *inside* its parent folder, which is **codefellows**. The folder labeled **codefellows** exists *inside* the parent folder named **projects**.

### Now, let's find out which "room" or directory you're currently in.

26. On the command line in your terminal, type 
> **pwd**

27. PWD stands for Print Working Directory. This is how you ask your Terminal, "Hey, where am I right now?"

28. Hopefully you get an **output** or response that looks something like this: 
> /mnt/c/Users/thepa/projects/codefellows/code102/

### With this output, we know we are in
> projects > codefellows > code102

- *The further left you go in the list, the higher the main folder. The further right you go in the list, the more you're getting deeper into sub-folders. For this example, **code102** is a room that exists *inside* the **codefellows** room. The codefellows room exists inside the larger room that is the **projects** folder. What matters **MOST** to us right now is ***which folder or sub-folder is listed at the far right***, which tells us our current location.*

29. Remember that new repository we made in the previous steps? I want to place it inside the **code102** folder location \(or "room" if we use our video game metaphor\). That means I have to be ***standing in the folder to place the Repository there***. According to my output in my Terminal, I'm standing inside the **code102** room right now, so I'm exactly where I need to be! If you are also standing in your **code102** room, move on to ***STEP 31***

> *If your **pwd** command produces a different output \(or shows you are in a different "room" than code102\) please feel free to stop here and ask for help. Or, if you're adventurous, I have some tips to help get you to the right spot.*

 - So, you've discovered you're not in the correct location. How do we get there? To move around inside our Terminal, we need to type the **cd** command. This is easy to remember because it stands for **Change Directory**.

 - In most cases, we also need to follow our **cd** command with a space and the destination we want to go. This is how we tell our Terminal *where* we want to go. But how do we type that command?

> ### cd locationname

 - Now, you are not actually typing the word "locationname" here. It's just an example. You will be typing the name of the destination/folder/directory of the "room" you want to visit. This is called a *path*. 

## But Jess, how do I know what to type?

Great question! There are two types of **paths**.

## 1. Relative Paths
> Typing a relative path name after **cd**  will travel you to a location related to *where you currently are.* For instance, let's say you are located inside a folder named "Months of the Year." Inside the folder, we have separate sub-folders each named after, you guessed it, the months of the year. It would be set up something like this:

- Months of the Year \(Parent Folder\)
    - January \(Sub Folder\)
    - February \(Sub Folder\)
    - March \(Sub Folder\)
    - April \(Sub Folder\)
    - May \(Sub Folder\)
    - June \(Sub Folder\)
    - Ect. You get the idea.

So, if we're standing *inside* the main/parent folder called "Months of the Year" we can travel to a sub-folder \(or sub-directory, "sub-room" in terms of our video game example\) using the following:

> ### cd May

This tells our computer **CHANGE DIRECTORY** to the **MAY** path connected to my current location.

## 2. Absolute Paths
> Absolute paths are a bit different. They spell out an exact location, no matter which room we're standing in. Rather than a door between connected rooms, it works more like a wormhole to wherever you need to go in your entire directory. Absolute paths typically feature forward slashes or the **/** symbol.

 - These paths are exact directions given in relation to your root directory, or the highest level directory in your current heirarchy.

## Let's go back to our Terminal.

- How do we get to the directory or folder we need, which is **code102**? *NOTE: If you were already standing in **code102** when we checked earlier, skip to **STEP 31***. Remember, the reason we want to travel to **code102** is because we want to place our Repository there.

30. If you type in the command **pwd** and you see **code102** somewhere in the output, you have a few options.

    - For example, I have typed **pwd** and this was my output:
> - /mnt/c/Users/thepa/projects/codefellows/code102/example-folder

- I can see from this output that I am one "room" too far because I am currently located in the "example-folder". \(**NOTE: example-folder is a dummy name I created for this demo. It is not a real folder you should have.\)** I need to travel back to the **code102** room, which is one room *back* in my directory.

        - I can do one of two things:

## Option 1

            - I can copy/paste the absolute path, but ommit the "example-folder/". It would look something like this:
> - /mnt/c/Users/thepa/projects/codefellows/code102/
            
            - Notice I no longer have the "example-folder/" following the "code102/" on my path.

## Option 2
            
            - I can type the following shortcut
 > **cd ..** 
 
            - This tells my terminal to CHANGE DIRECTORY back ONE parent folder, or "room" if we use the language from our video game metaphor.

### *If these options do not work, please contact a TA or instructor for help. To view the files or folders contained inside your location, type **ls** which tells your Terminal to **LIST** the contents of your current location. If we use our video game metaphor, this command shows you *what is in the room with you as you stand there*.*


## GIT CLONE YOURURLHERE

31. Success! You've reached this step because you've found yourself standing in the "room"/directory/path/folder named **code102**. This is where we will place our Repository using the **git clone yoururlhere** command.

32. Now, when we use the command **git clone yoururlhere** your Terminal automatically knows to create a folder *inside* **code102** to group all the information it is about to import from GitHub. The folder will be named after the title you assigned to your Repository in GitHub when you created and set up the Repository. For the rest of this demo, we are proceeding as if we are going to **git clone** our **reading-notes** Repository. If you have already done this process and have the **reading-notes** Repository available to edit in VS Code on your computer, don't repeat this guide using that particular Repository. This is just an example that you can use with any *new* Repository you create.

    - *If you haven't been able to **git clone** your **reading-notes** Repository to your local computer yet, I hope the following info helps!*

33. Let's do it! In our example, we're moving forward to **git clone** our **reading-notes** Repository and place it within our **code102** folder. In your Terminal, type **git clone yoururlhere** into your command line. Remember that *second* link you copied from your GitHub repository located under the green **CODE** button? You will paste that in place of the text "yoururlhere." For me, it looks like this:

> git clone https://github.com/DevJessParker/reading-notes.git

34. You should get an output that looks similar to this:

>Cloning into 'reading-notes'...
remote: Enumerating objects: 171, done.
remote: Counting objects: 100% (171/171), done.
remote: Compressing objects: 100% (167/167), done.
remote: Total 171 (delta 76), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (171/171), 42.04 KiB | 341.00 KiB/s, done.
Resolving deltas: 100% (76/76), done.

#### Great! Now, the most important thing to remember at this step is that our goal is to edit our **reading-notes** Repository files in VS code. But to edit our Repository files, we have to be standing inside the Repository we've just created. And, as we know, we are currently standing inside **code102** because even though we have just *created* a new folder **reading-notes** folder and placed it into the **code102** "room" ***we did not moved into the **reading-notes** folder.** We are still standing in the **code102** room.*

## Let's Move - Pt. 2!

Before we send our file or files to edit in VS Code, we need to make sure we send the *right* file or files. How do we do that?

35. We need to move into the **reading-notes** folder, since that is the location containing all the files we want to edit. Do you remember how to move within your Terminal? What is the command we need to use to signal our Terminal to **Change Directories?**

36. That's right! Type in 
    
**cd reading-notes**

> We can use a *relative* path here because **reading-notes** is a "room" connected to our current location in **code102**. We are telling our Terminal to **CHANGE DIRECTORY** to **READING-NOTES** because we want to travel to the **reading-notes** folder located *inside* our current location.

Remember: For this demo, we want to be standing inside the folder containing the Repository files we want to edit \( in this case the folder named **reading-notes**\) before we send the folder and its contents to VS Code for editing.

37. Ready to edit your project files? Let's tell our Terminal we want to open our current location \(the **reading-notes** folder\) into our editing program, VS Code, by using the following command:

> **code .**

38. This command should open a VS Code window with the contents of your **reading-notes** repository, since we were standing in the **reading-notes** folder when we issued the command. On the left in your VS Code window, any Repository pages you previously created using the GitHub creation tools will be show in a vertical list.

>Remember - We are no longer adding pages or editing our Repositories in GitHub. We are now doing these tasks using our Terminal, VS Code, and the ACP Steps. If you need to add a page or file to your Repository, you will need to use your Terminal and use commands to manually create the file. Then, you'll follow the ACP steps to make that page go live on GitHub.

## Let's get back to VS Code

39. Select the page or file you want to edit from the left side list in the VS Code window. Here, you can make make your intended Markdown changes for any file.

    - Take note of the icon featuring overlapping pages located in the far left toolbar. If you have a blue number showing here, you have unsaved changes.
    - To see a real-time preview of your edits in a Markdown or **.md** file, click the icon in the upper toolbar that looks like an open book laying beneath a magnifying glass. This will open up a preview to the right of your text editing window.

40. Be sure to **save** each file or page as you go. You can either set up auto-save or you can use the save shortcut.

    - For MAC users, the shortcut is COMMAND S
    - For Windows users, the shortcut is CTRL S

## ACP STEPS

41. You've reached the point where you're done editing your files in VS Code and you're ready to send those changes back to GitHub so you can see them live on your browser. Now it's time to start the ACP process, which will sync or **"push"** your changes back to GitHub so they can go live.

42. First, let's open our Terminal and make sure we know where we are, just in case we don't remember moving or we've had to enter any additional commands since starting this Help Guide. Type the command you learned earlier that asks the question, "Hey Terminal! Where am I?"

**HINT: Print Working Directory**

43. We need to make sure we are standing in the folder containing the modified files we intend to sync or "push" back to GitHub. For this example, we need to be standing in the **reading-notes** directory, because we've been editing many of the files located *inside* the **reading-notes** folder, such as your individual page files. Revisit the steps above regarding navigating through the directory \(where we learned how to change "rooms"\)

44. Now that you're standing in the **reading-room** folder, let's start the ACP Process.

## Remember that ACP stands for:
    - ADD
    - COMMIT
    - PUSH

## Here are the git commands you will be using, listed in the order they are performed.

Command | Action or Output
------------ | ------------
**git status** | Asks your Terminal to show all modified files that have **NOT** been synced to the original source of your repository. These may show in red.
**git add filename** | This transfers a specific file to your "Waiting to Sync" queue. You are signaling to your Terminal that you intend to "push" this modified file back up to GitHub.
**git add .** | This is a shortcut that does the same action as above, but instead of sending a specific file to your "Waiting to Sync" queue, it sends ***all files with unsynced modifications located in your current directory*** to your queue. Don't know which files have modifications? They should be listed in red a few lines up as the output of your previous command **git status**
**git status** | This command is repeated here to verify that your files have been added to your "Waiting to Sync" queue. You should see an output that lists "Changes to be committed:" along with the file names you selected when using the **git add filename** command. Depending on your system, those file names could now be shown in green instead of red.
**git commit -m "Your modification notes here."** | Use the quotation area to give a brief description of *what* was changed and/or *why* it was changed. Keep it short and simple for now. This acts as your "Save As" point.
**git push origin main** | This is the final signal in ACP the process. It will "push" your queue of selected **git add** files back up to GitHub so your changes can go live.

## OTHER NOTES

### Adding a new page into your Repository.

1. Now that you've downloaded your GitHub Repository into your local system, do **NOT** edit any of your content within GitHub itself. We will do all our edits using our Terminal, VS Code, and the ACP steps I just described above. Editing in GitHub can cause content conflicts, and we want to make sure you aren't having to redo any of these steps.

2. If you need a new page in your Repository \(for instance, if you need to add a new page for additional Reading Notes assignments throughout the week\), you do **NOT** add it using your GitHub dashboard. You add it using the following steps:

     - Open your Terminal and enter the command used to ask, "Hey Terminal. Where am I right now?"
     - Navigate to the directory for your Repository, or the location you need the file to go. For the example above, you will be navigating to the **reading-notes** folder since we are adding a page to that project. If you have been working with your **reading-notes** file in VS Code, you may already be standing in the **reading-notes** "room"/ folder and would therefore *not* need to move.
     - If you are no longer located in **reading-notes**, use some creative thinking to navigate yourself to the **reading-notes** folder. You may need to revisit the section above about Navigation and **absolute** versus **relative** paths.
     - Okay! If you're at this step, it means you're standing in the **reading-notes** folder and are ready to add your new page.

## Commands for Creation

Command | Action
------------ | ------------
mkdir | Make Directory \(Makes a folder\)
touch | Creates a specified file

3. It's time to create that file! **Remember:** We are creating a file within a *parent* directory. In this case, **reading-notes** will become our parent directory. Our new file will go *inside* our **reading-notes** folder.

4. Consult the list above. What command would we use to create a file? That's right! For the following example, let's say I want to create a file/page called "ACP for Beginners"

5. I do **NOT** want spaces in my file name. These can cause issues and unnecessary confusion in my directory as I move around using the **cd** command we learned earlier. So, I will name my file without spaces and use the following command:

     >**touch acpforbeginners.md**

6. Notice the **.md** at the end? That is because I need this particular file to be a ***Markdown*** file. If I needed an HTML file, I would use the following command:

    > **touch acpforbeginners.html**

## How can I tell if I have this new file?

7. Great question! Do you remember the command we learned earlier that asked the question, "Hey Terminal. What else is in the "room" or folder where I'm currently standing?" That command is:

>**ls**

8. This should show you a **LIST** of all files and sub-folders contained inside your current location. You should now see your newly created file listed in the results. If not, grab a TA and do some troubleshooting! It's all part of the learning process.

9. Let's say, I want to edit my new file. What do I type to signal that I now want to open my current location in VS Code? Scroll up to find the answer. 

>HINT: I'm ready to **code .**

10. Now remember, you're still "standing" in **reading-notes**. You *created* your new file but did not *move* to it. So, when you type the command listed above, it will open your **reading-notes** folder in VS Code. Since **reading-notes** is the folder of our entire Repository, you should see all your pages and files listed on the left side. Opening the entire **reading-notes** Repository folder in VS Code is great because you can make and track changes easily across all your pages in the entire project, since they will all be listed in easy-to-click tabs on the left in your VS Code window.

## POTENTIAL ISSUES AND TIPS

> If you created a .html file, you'll want to open up a live server preview. This will allow you to preview how your html file will look on a deployed or live website. To open up the live server preview in VS Code, follow the steps below:

    - Right click your .html file. Select the "Open with live server" option.
    - If you do NOT see this option, don't worry! Click on the toolbar icon that looks like a grid with a square breaking off. You will find this on the far left side. When you hover over this icon, you'll notice it is called "Extensions."
    - Search for liveserver. You should see an option toward the top of the results labeled "Ritwick Dey." Install that extension.
    - Return to the html file you want to edit by clicking on it in the list.
    - Voila! You should now be able to right click your html file and select "Open with Live Server."

> TIP:

If you aren't seeing your pages, make sure you are viewing files in the correct Repository. We now have *two* Repositories, one for our **reading-notes** and one for **our upcoming website/wireframing project using HTML that you will name yourself**. If you need to open one or the other in VS Code, use your Terminal to navigate to your target Repository folder, then use the **code .** command to open that location in the VS Code editor.

There is an option to access your Terminal directly in VS Code \(available by clicking on **Terminal** in your top tool bar located in the VS Code window\) but I personally find that having my Terminal open in its own window, separate from VS Code, helps me keep them separate in my mind. I think it's probably personal preference right now.

## DON'T FORGET!

 - If you created a file using the **touch filename** command above, you did so on your *local system*, meaning your new file doesn't exist outside your computer. Your changes will need to be "pushed" back up to GitHub so that new file and any changes can sync to your GitHub Repository. This is how your changes and GitHub pages will go live on your website. The page will NOT show up on GitHub until you complete the ACP process and "push" your changes up using the **git push origin main** command.

 - Not sure how to "push" your changes back up to GitHub? Revisit the **ACP STEPS** section above.

 # GO FORTH AND CODE GREAT THINGS! I'M PROUD OF US!









