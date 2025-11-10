# HW3A Solution - Git and Version Control
## Part 1: Repository Cloning
I successfully cloned the class repository from `https://github.com/olearydj/INSY6500` to
`~/insy6500/class_repo`.

### Key Commands Used
- `git clone <url>` - Create local copy of remote repository
- `git log` - View commit history
- `git remote -v` - Check remote repository connections
- `git status` - Check what git sees
- `git add` - to send files to the staging area (ready to commit)
- `git commit -m` - To commit the files and add a commit message 

## Part 2: Portfolio Repository Creation
I created my personal course repository with:
- Professional README.md describing the project
- Proper .gitignore to exclude unnecessary files
- Organized directory structure for homework, projects, and notes
### Understanding Git Workflow
The three-stage workflow:
1. Working Directory: Where I edit files
2. Staging Area: Where I prepare commits with `git add`
3. Repository: Where commits are permanently stored with `git commit`

## Part 3: GitHub Publishing
Successfully published repository to GitHub:
- Used `git remote add origin` to connect local repo to GitHub
- Used `git push -u origin main` to upload commits
- Verified all files and commits are visible on GitHub
### The Remote Connection
My local repository is now connected to GitHub:
- `git remote -v` shows the remote URL
- `git push` will send my commits to GitHub
- `git pull` will get updates from GitHub (if changes are made on GitHub)
### Details
Complete this section with details from your setup:
- Repository URL: https://github.com/ggilarteaga/py4eda-work
- Output of `git remote -v`:
origin  https://github.com/ggilarteaga/py4eda-work.git (fetch)
origin  https://github.com/ggilarteaga/py4eda-work.git (push)

- The output of `git log --oneline`:
5bf7621 (HEAD -> main, origin/main) Add hw3a solution document
d426c6d Initial commit: Add README and .gitignore

##Questions
###Reflections

####Question 1: Git Workflow Benefits:
a) Before this assignment the way I tipically managed different versions of my work was by adding at the end of the file name the version/revision (ex: _V2). If the work was collaborative I would add at the end of the document a table with the version/revision, date and author to keep track of changes.
Git greatly facilitates the version control efforts since all this information (and additional information) is available in a more accessible and organized way. It allows simultaous work when working on a collaborative file.
By using Git I don't need to rename the latests verions of the files, which would sometimes lead to confusions about which is the actual latest version of a document. I is also very useful to maintain up to date the files shared with others by using "git pull". Running this command everytime I access a repo would help me ensure I work with the latest version of the documents, homework, assignments. Therefore any corrections made since the last time I opened it would be visible.

b) When I was working in Spain as a Product Engineer we had multiple problems trying to have all product documentation and company files up to date for everyone. The reason behind most of the problems was that people would work on the documents locally and then upload the modified version to the common/shared directory. But if someone had previously modified that same document, all previous changes would be lost. 
Additionally, unless the version control table was properly filled out by the people working on the document it would be hard to track changes and recognize authors in case of doubt.
Using Git would have solved these problems since any changes (even minor changes) could have been easily and rapidly updated and tracked by everyone in the organization. This would have saved extra amount of work and would have prevented the loss of information.

####Question 2: Repository Organization:
a) It is important to keep this two repositories separated because each of them serves a different purpse. class_repo is managed by the instructor, and its content should not be modified by the students since they could introduce errors and therefore affect the rest of the students. The material on that repositpry should be only accessible to read.
On the other hand, my_repo is the personal repository in which studetns develope their own work. For that reason they should be able to modify the content of the repository, and push it to GitHub (so that the instructor can access it and evaluate it). 
If you tried to put everything in one repository you probably wouldn't be able to push any changes as we don't have permission from the instructor to modify his repository (class_repo). However, if he gave us access to modify teh repo, it would be a mess since every student would be modifying the exact same files.

b) For my future course work or projects I would create a repository for each class (or professional project) that I have. If I had a group project for a class I would create a repository for that project inside the repository of the class and give permission to the people on the group to modify that repository. However, if the project was an individual assignment I would also create an additional repository inside the class repository (if needed), but I wouldn't give editor permissions. 
For reference materials I would clonate the repos that I need as a reference and pull from them every time I need to work with them.
 

####Question 4: Commit Messages and History
a) The second commit message is definitely more useful since it provides valuable information about the changes that have been made. Commit messages must be meaningful, otherwise the commit message is useless since it doesn't reflect the updates. 
I might need to find this commit again in the future if I want to review hw3 before the next exam, or if on a future class I'm required to use git and I need to review this assignments.
b) From my own experience anything that takes 60 minutes of work or more deserves a commit (as a general rule of thumb). However, any major change than affects significantly any future work must be commited as soon as possible. 



###Graduate Questions

####Question 1
a) I think it was valuable to commit the README and .gitignore separately from the hw3a-solution because those two initial files are part of the initial set up of the repository, while the homework was actual "work". 
If I had committed everything at once I would have lost either information about the initial commit used to set up the basics of the repository, or information about the first added work (hw3a).

b) I would commit the updates on the readme (I don't understand what you mean with write code to load data. I am assuming is not part of a file or document, just code on the terminal. So I wouldn't commit that), I would probably wait till I finish the homework to commit the changes, since homework assignments are generally not very long and not collaborative so there might be little value in conmitting very frequently.
I would not commit the typo correction since its a minor thing. Stagning helps me make the decision since I don't need to commit all changes at once and I can wait until changes on parts of my work are relevant enough.

c) Git status helps me make decisions about what to stage and commit by letting me know what information is currently being tracked, what is staged and need to be commited and what is already commited. This help me visualize what is already "safe".
I would use it before I start working with my projects/assignments and when I'm done.

####Question 2
a) A distributed control system is a type of control system in which every user has a local copy  (clone) of the repository. In contrast, Google Drive or Dropbox just have a common copy on the cloud shared by all the users.

b) This architecture is valuable for developers since they can work on their local repository (which may be a preferred option) even without internet access and then synchronize the changes made by them and merge them with those made by others. This enables developerts to work simultaneously on the same files withouth being disrupted by others working on the same part of a file.

c) Git clone creates a local copy of someone's repository, you can git pull from the origin of that repository to update any changes made by the owner of the repository, but you can't push changes made by you on the clone repository towards the original unless you have permission. However you can use git push to synchronize github with your repositories to update changes.
The reason I can pull from class_repo but I can't push to it is that the repository is public and I can therefore get the latest version by pulling, but I can't push because I haven't been authorized by the owner (the instructor) to make changes.
Since my_repo is my personal repository (I am the owner) I can do both.


####Question 3
a) When deciding what to commit I must consider the quality of the work and the meaningfullness towards the progress of the projects that I'm working on at the moment. I like to demonstrate that I work and revise my work by showing continuous progression and improvements on my work. I believe this is more valuable to me and to others who are reviewing my work. Products are never perfect or finished, there is always room for improvement.

b) A README file for a portfolio repository should include information about the formation and general working line of the author. A README for an open-source project should have specific and valuable information regarding that project that facilitates the understanding of the repository.

c) Builing this portfolio during my course work is going to help me greatly to start adding content to it and polish detalis se that when I start my job search I will already have a well developed, well structured and full of content portfolio. I must adopt habits to maintain the portfolio clean and well organized as well as structured and standardized.


b) 


