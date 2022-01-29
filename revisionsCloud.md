[Home](README.md)>[Topic Notes](topicNotes.md)

# Revisions and the Cloud

## Week 01 Day 03

Today we learned about Git, GitHub, and how they work together as valuable tools of a coder.

Git is a DVCS (distributed version control system).
This lets multiple developers work on the same code, at the same time, and be able to track through different revisions or snapshots (commits) in time of that code.
You can view, apply, and remove changes that are made this way, and it allows a team to keep all files within one repository.
Basically, this makes collaboration possible!
Commits represent successive versions of a file, with the HEAD being the most recent.

GitHub is ***not*** Git.
What it is, is your code, in the cloud.
This makes GitHub an excellent way to share code and projects with others.
Also, it provides an online backup for code storage, since most work is done locally.
GitHub can also be used to manage a team's work.
Especially helpful when your team may be comprised of people from around the world.

When we want our changes to go from our local machines (git) to GitHub, we **ACP**.
This stands for Add, Commit, and Push.
Amanda used some great analogies to explain this idea.
One example was that of a polaroid camera.
Add is like when you frame your subject. 
*What do you want in your photo*?
Commit is pushing the button down to take the photo.
Push is when the photo is printed.
A literal snapshot!
That being said, one major difference between this act in coding and taking a photo with a polaroid is that you can add, commit, add, commit, many times without choosing to Push (or print our photo).

What we had to do today was to clone our reading-notes repository from GitHub down to our local machines.
Once we did that, we were able to write code using VSC for our reading-notes repository and ACP as appropriate to make sure that our changes were reflected in GitHub and on our live page.

Here are some commands that I used:

- mkdir (to create the file code102 for the repository to live)
- git clone (to actually clone the repository to my local machine)
- git status
- code . (to open the repository in VSC)
- git add . (to add the changes saved for the repository in VSC)
- git commit -m "caption here" (to commit)
- git push origin main (to push to GitHub)

That's all for now on this topic. More to come later!
