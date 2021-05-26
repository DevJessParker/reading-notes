# HELP! Repo to ACP Detailed Process Guide

This week is going to push us all outside our comfort zones. That's okay! Take a look at what we've done today. Could we have done this yesterday? Probably not. \I know *I* couldn't!

Learning is uncomfortable and we're all going to make mistakes. That's okay, too.

Here is my step-by-step guide to:

- Creating a Repo on GitHub
- Setting up your Repo
- Finding your location on your computer
- Git cloning your repo down to your local computer
- Opening your file in VS Code
- Editing your file
- Saving Changes
- Performing an ACP
- Returning to your live website

## Creating a Repo on GitHub

To create a New Repo on GitHub, perform the following steps:

1. Log in to [GitHub](https://www.github.com/)

2. In the upper right hand corner, click on your photo. You can also click on the dropdown arrow.

3. Select **My Repositories**

4. On the new page, click the green button that says "NEW"

### Pay very close attention to these next steps. Go slowly, as it can be a bit tricky. Think of a Repository as a giant master bucket that holds all the pages for a certain project. That is why you will have a reading-notes repository **AND** a repository for your html website. Those are *two different projects*. However, your notes for each class are all "Reading Notes," so they apply to the same bucket, which is your reading-notes repository.

5. Name your new repository. Do **NOT** use capital letters. Do **NOT** use spaces.

6. Add a short description of your repository.

7. Make sure your repository is marked **PUBLIC**

8. Click **"Add a README.md file"**

9. Click **"Create Repository"

### Congrats! You now have a brand new bucket where you can store all the GitHub pages relating to this particular project. Now, let's **SET UP YOUR NEW REPOSITORY.** Pay very close attention here, as you need to closely follow these steps.

10. You should be on the dashboard home for that repository. Click on the **SETTINGS** gear in the toolbar.

11. On the lefthand side, scroll down until you see the vertical tab marked **PAGES.** Click this tab now.

### We need to now deploy the repository so it can have a live URL home. 

12. Under **SOURCE**, click the **BRANCH** dropdown and select **MAIN**

13. Click the button marked **SAVE**

14. You should now have a message providing you a link to your live website.

15. Highlight and copy/paste that link.
    - For MAC users, the shortcut to copy/paste is **COMMAND C**
    - For Windows users, the shortcut to copy/paste is **CTRL C**

16. On the upper left side of your screen, you will see a **breadcrumb** that lists your UserName/name-of-your-repository. This may be blue in color. Specifically click on the name of your repository, as this will take you back to that repository's dashboard home.

17. On the right hand side, in the **ABOUT** section, click on the gear symbol.

18. Under **WEBSITE** paste your link.

19. Click **SAVE CHANGES**

### Now that our repository has been created in GitHub, and we have assigned it a URL, we will **NOW STOP EDITING THE REPOSITORY IN GITHUB**. Moving forward, we will be editing this repository using our coding tools on our computer.

### However, right now our Repository only exists on GitHub. We need a way to create a connection between GitHub and our local editing tools \(Our Terminal/Ubuntu and VS Code\)

20. On your Repository's home dashboard screen, click the green **CODE** button.

21. You will see a popup labeled **CLONE** that shows a URL link. Copy and paste this link.

### Be sure you grab the link under the **CODE** button. You will need this link shortly.


## Let's Get Moving!

Now we're ready to create a connection between GitHub and the editing tools on our local computer. To make sure we're ready to go, let's do a couple steps first.

22. Open your Terminal.

### Before we start throwing files around all willy nilly in our Terminal, let's make sure we know *where* those files are going. But first, where are *we* in our Terminal? It may help to think of this as if you are a character in a video game filled with rooms. Before you can complete your mission in a certain room \(or folder, in our case\) we need to know:

Question | Video Game Example Question
------------ | ------------
Where are we currently editing in our code? | Which room are we in?
How do we get to our target location from our current location? | How do we change rooms?

23. When setting up the folders on our computer, we used our Terminal to create **paths**. Paths are the hallways and directions that lead us to the rooms.

24. If you did **NOT** set up folders using the mkdir command, I recommend you stop here and contact a TA or the instructor. They can help explain how to set up your folder pathways using your Terminal.

25. You should have set up the following folders and sub-folders, in this order:
- Projects
    - Codefellows
        - code102

### Now, let's find out which room you're currently in.

26. On the command line in your terminal, type **pwd**

27. PWD stands for Print Working Directory. This is how you ask your Terminal, "Hey, where am I right now?"

28. You may get an **output** or response that looks something like this: /mnt/c/Users/thepa/projects/codefellows/code102/

### With this output, we know we are in projects > codefellows > code102
### The further left you go in the list, the higher the main folder. The further right you go in the list, the more you're getting deeper into sub-folders. For this example, code102 is a room that exists **inside** the codefellows room. The codefellows room exists **inside** the larger room that is the projects folder. Folders work like nesting dolls. What matters **MOST** to us right now is ***which folder is listed at the far right***.

29. Remember that repository I made? I want to place it inside the **code102** room. That means I have to be ***standing in the room to place it***. According to my output, I'm standing inside the **code102** room right now, so I'm exactly where I need to be! If you are also standing in your **code102** room, move on to ***STEP 31***

### If your **pwd** command produces a different output \(or a different "room" than code102\) please feel free to stop here and ask for help. Or, if you're adventurous, I have some tips to help get you to the right spot.

### To move around inside our Terminal, we need to type the **cd**. This is easy to remember because it stands for **Change Directory**.

### In most cases, we also need to tell our Terminal *where* we want to go. But how do we do that? What command do we use to "move" around?

## cd location

Now, you are not actually typing the word "location" here. It's just an example. You will be typing the name of the destination/folder/directory of the "room" you want to visit.

## But Jess, how do I know what to type?

Great question! There are two types of **paths**

## Relative Paths
> Typing a relative path name here will travel you to a location related to where you currently are. For instance, let's say you are standing inside a folder named "Months of the Year." Inside the folder, we have separate sub-folders each named after, you guessed it, the months of the year. It would be set up something like this:

- Months of the Year
 - January
 - February
 - March
 - April
 - May
 - June
 - Ect. You get the idea

So, if we're standing *inside* the main/parent folder called "Months of the Year" we can travel to a sub-room \(or sub-directory, sub-folder\) using the following:

### cd May

This tells our computer **CHANGE DIRECTORY** to the **MAY** room connected to my current location.

## Absolute Paths
> Absolute paths are a bit different. They spell out an exact location, no matter which room we're standing in. Rather than a door between connected rooms, it works more like a wormhole to wherever you need to go. Absolute paths typically feature forward slashes or **/**

These paths are exact directions given as the location relates to your root directory, or the highest level directory in your current heirarchy.

## Let's go back to our Terminal. How do we get to the directory we need, which is **code102** ? *NOTE: If you were already standing in **code102** when we checked earlier, skip to **STEP 31***.

30. If you type in the command **pwd** and you see code102 somewhere in the output, you have a few options. For example.

 - I have typed **pwd** and this was my output:
    - /mnt/c/Users/thepa/projects/codefellows/code102/reading-notes

    I can see from this output that I am one room too far because I am currently standing in the "reading-notes" room. I need to travel back to the "code102" room, which is one room *back* in my directory.

        - I can do one of two things:

            - I can copy/paste the absolute path, but ommit the "reading-notes" room. It would look something like this:
                - /mnt/c/Users/thepa/projects/codefellows/code102/
            
            - I can type the shortcut **cd ..** which tells my terminal to **CHANGE DIRECTORY** back **..** one parent folder or "room".

### If these options do not work, please contact a TA or instructor for help. To view the files or folders contained inside your location, type **ls** which tells your Terminal to **LIST** the contents of your current location. If we use our video game metaphor, this command shows you *what is in the room with you as you stand there*.


## GIT CLONE YOURURLHERE

31. Success! You've hit this step because you've found room/directory/path **code102**

32. Now, when we use the command **git clone yoururlhere** your Terminal automatically knows to create a folder *inside* **code102**

33. Let's do it! Type **git clone yoururlhere** into your command line. Remember that link you copied from your GitHub repository? You will paste that in place of the text "yoururlhere." For me, it looks like this:

>git clone https://github.com/DevJessParker/reading-notes.git

34. You should get an output that looks similar to this:

>Cloning into 'reading-notes'...
remote: Enumerating objects: 171, done.
remote: Counting objects: 100% (171/171), done.
remote: Compressing objects: 100% (167/167), done.
remote: Total 171 (delta 76), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (171/171), 42.04 KiB | 341.00 KiB/s, done.
Resolving deltas: 100% (76/76), done.

### Great! Now, the most important thing to remember at this step is that our goal is to edit our reading-notes files in VS code. But to edit a room right now, we have to be standing inside it. And, as we know, we are currently standing inside **code102** because we have *created* a new folder but ***we have not moved into it yet.***

## Let's Move - Pt. 2!

Before we send our file to edit in VS Code, we need to make sure we send the *right* file. How do we do that?

35. We need to move into the reading-notes directory. Do you remember how to do that? What is the command we need to use to signal our Terminal to change directories?

36. That's right! Type in 
    
**cd reading-notes**

> We can use a *relative* path here because **reading-notes** is a room connected to**code102**. We are telling our Terminal to **CHANGE DIRECTORY** to **READING-NOTES** because we need to be standing inside the directory we want to send to VS Code.

37. Ready to code? Let's tell our Terminal we want to open our current location in VS Code by using the following command:

**code .**

38. This should open a VS Code window with the contents of your reading-notes repository. On the left, your separate GitHub pages will be shown in a vertical list.

39. Select the page or file you want to edit. Make your Markdown changes.

40. Be sure to **save**. You can either set up auto-save or you can use the save shortcut.

    - For MAC users, the shortcut is COMMAND S
    - For Windows users, the shortcut is CTRL S

## ACP STEPS

41. You've reached the point where you're done editing your files in VS Code. Now it's time to start the ACP process, which will sync or **"push"** your changes back to GitHub so they can go live.

42. First, let's open our Terminal and make sure we know where we are. Type the command you learned earlier that asks the question, "Hey Terminal! Where am I?"

**HINT: Print Working Directory**

43. We need to make sure we are standing in the folder we need to sync or "push" back to GitHub. For this example, we need to be standing in the **reading-notes** directory. Revisit the steps above regarding navigating through the directory \(where we learned how to change "rooms"\)

44. Now that you're standing in the **reading-room** directory, let's start the ACP Process.

## Remember that ACP stands for:
    - ADD
    - COMMIT
    - PUSH

## Here are the git commands you will be using listed in the order they are performed.

Command | Action or Output
------------ | ------------
**git status** | Asks your Terminal to show all modified files that have **NOT** been synced to the original source of your repository.
**git add filename** | This transfers a specific file to your "Waiting to Sync" queue. You are signaling to your Terminal that you intend to "push" this modified file back up to GitHub.
**git add .** | This is a shortcut that does the same action as above, but instead of sending a specific file to your "Waiting to Sync" queue, it sends ***all files with modifications located in your current directory*** to your queue. Don't know which files have modifications? They should be listed in red on your Terminal as the output of your previous command **git status**
**git status** | This is repeated here to verify that your files have been added to your "Waiting to Sync" queue. You should see an output that lists "Changes to be committed:" along with the files you selected when using the **git add filename** command. Depending on your system, those file names could now be shown in green instead of red.
**git commit -m "Your modification notes here."** | Gives a brief description of *what* was changed and/or *why* it was changed. Keep it short and simple for now.
**git push origin main** | This is the final signal in the process. It will "push" your queue of selected **git add** files back up to GitHub so your changes can go live.

## OTHER NOTES

### Adding a new page into your Repository.

1. Now that you've downloaded your GitHub Repository into your local system, do **NOT** edit any of your content within GitHub itself. We will do all our edits using our Terminal, VS Code, and the ACP steps I just described above. Editing in GitHub can cause content conflicts, and we want to make sure you aren't having to redo any of these steps.

2. If you need a new page in your Repository \(for instance, if you need to add a new page for a new Reading Notes assignment\), you do **NOT** add it using GitHub. You add it using the following steps:

     - Open your Terminal and enter the command used to ask, "Hey Terminal. Where am I right now?"
     - Navigate to the directory for your Repository. For the example above, you will be navigating to the **reading-notes** folder. If you have been working with your reading-notes file in VS Code, you may already be standing in the **reading-notes** "room" and would therefore *not* need to move. If not, use some creative thinking to navigate yourself to the **reading-notes** directory. You may need to revisit the section above about Navigation and absolute versus relative paths.
     - Okay! If you're at this step, it means you're standing in **reading-notes** and are ready to add your new page.

## Commands for Creation

Command | Action
------------ | ------------
mkdir | Make Directory \(Makes a folder\)
touch | Creates a specified file

3. It's time to create that file! **Remember:** We are creating a file within a *parent* directory. In this case, **reading-notes** will become our parent directory. Our new file will go *inside* our **reading-notes** directory.

4. Consult the list above. What command would we use to create a file? That's right! For the following example, let's say I want to create a file/page called "ACP for Beginners"

5. I do **NOT** want spaces in my file name. These can cause issues and unnecessary confusion in my directory as I move around. So, I will use the following command:

     >**touch acpforbeginners.md**

6. Notice the **.md** at the end? That is because I need this particular file to be a ***Markdown*** file. If I needed an HTML file, I would use the following command:

    > **touch acpforbeginners.html**

## How can I tell if I have this new file?

7. Great question! Do you remember the command we learned earlier that asked the question, "Hey Terminal. What else is in the room where I'm currently standing?" That command is:

>**ls**

8. This should show you a **LIST** of all files and sub-folders contained inside your current location. You should now see your newly created file listed in the results. If not, grab a TA and do some troubleshooting! It's all part of the learning process.

9. Now, I want to edit my new file. What do I type to signal that I now want to open my current location in VS Code? Scroll up to find the answer. 

>HINT: I'm ready to **code .**

10. Now remember, you're still "standing" in **reading-notes**. You *created* your new file but did not *move* to it. So, when you type the command listed above, it will open your **reading-notes** file in VS Code. Since **reading-notes** is the folder of our entire Repository, you should see all your pages listed in the vertical tabs on the left hand side.

## POTENTIAL ISSUES AND TIPS

> If you created a .html file, you'll want to open up a live server preview. This will allow you to preview how your html changes will look on a deployed or live website. To open up the live server preview in VS Code, follow the steps below:

    - Right click your .html file. Select the **Open with live server** option.
    - If you do *not* see this option, don't worry! Click on the toolbar icon that looks like a grid with a square breaking off. You will find this on the far left side. When you hover over this icon, you'll notice it is called **Extensions**.
    - Search for liveserver. You should see an option toward the top of the results labeled "Ritwick Dey." Install that extension.
    - *Voila!* You should now be able to right click your html file and select **Open with Live Server**.

> If you aren't seeing your pages, make sure you are accessing the correct Repository file. We now have *two* Repositories, one for our **Reading Notes** and one for **our upcoming website/wireframing project using HTML**. If you need to open one or the other, use your Terminal to navigate to your desired location, then use the **code .** command to open that location in VS Code. There is an option to access your Terminal directly in VS Code \(available by clicking on **Terminal** in your top tool bar\) but I personally find that having my Terminal open in its own window helps me keep them separate in my mind.

## DON'T FORGET!

 - If you created a file using the **touch filename** command above, you did so on your *local device*. Your changes will need to be "pushed" back up to GitHub so that new information can sync to your GitHub Repository. This is how your changes and GitHub pages will go live on your website.

 - Not sure how to "push" your changes back up to GitHub? Revisit the **ACP STEPS** section above.

 # GO FORTH AND CODE GREAT THINGS! I'M PROUD OF US!









