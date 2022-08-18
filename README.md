# CMPG 323 Project Overview
<img src="https://github.com/ChiefMonk/CMPG-323-Overview-37016776/blob/main/nwu_logo.jpg" width="100" /> 

The overview document explains the overall project structure for the semester, and the general branching strategy for each project repository and also serves as a general guide to everything about this semester's projects for CMPG 323.

## Project Structure
For the work to be done this semester, a single <a href="https://github.com/users/ChiefMonk/projects/5">Kanban project</a> is created to outline and plan for all the work to be done. The scheduled work will be done over 8 Sprints, each lasting 10 working days (2 calendar weeks). At the beginning of every sprint, mostly on the first day, a sprint planning session is convened to categorise and itemise what will be done and allocate appropriate resources and time to each issue. 

However, to properly manage the project and meet the various sprint deadlines, the work is further planned and divided weekly. This also helps to negate any time challenges that could be encountered over the 2-week fixed time period.
 
## Branching Strategy
The main idea behind any branching strategy is to isolate the work into different types of branches. There are lots of ways of structuring the braches to meet various organisational and strategic needs. However, for my project, only the following resource branches will be developed:
* <strong>main</strong> : will serve as the master branch with the most current working, relatively non-buggy code.
* <strong>develop</strong> : will serve as the development branch code that will be merged into the <strong>main</strong> branch once properly tested. Any new work must be done on the <strong>develop</strong> 
* <strong>release</strong> : Once a release is required for a particular environment (e.g. prod), a <strong>release</strong> branch will be created off the <strong>main</strong> branch and appropriately numbered and tagged.
* <strong>hotfix</strong> : If an urgent bug has been discovered in a particular release or <strong>main</strong> branch, a <strong>hotfix</strong> branch will be created off that branch and the effective fix applied. Once applied, the code will then be merged back via pull-requests into the applicable branch, and where necessary also into the <strong>develop</strong> branch.

## .gitignore File
In general, Git sees every file in your working copy as one of three things:
* tracked - a file which has been previously staged or committed;
* untracked - a file which has not been staged or committed; or
* ignored - a file which Git has been explicitly told to ignore.
* 
Ignored files are usually build artifacts and machine generated files that can be derived from your repository source or should otherwise not be committed. Some common examples are:
* dependency caches, such as the contents of /node_modules or /packages
* compiled code, such as .o, .pyc, and .class files
* build output directories, such as /bin, /out, or /target
* files generated at runtime, such as .log, .lock, or .tmp
* hidden system files, such as .DS_Store or Thumbs.db
* personal IDE config files, such as .idea/workspace.xml


## Contributors
* <a href="https://github.com/ChiefMonk">[Chipo Hamayobe]</a>(https://github.com/ChiefMonk) - Project Lead

## References
### Branching
* [What is the best Git branch strategy?](https://docs.microsoft.com/en-us/learn/paths/intro-to-vc-git/](https://www.gitkraken.com/learn/git/best-practices/git-branch-strategy))
### .gitignore
* [Git .gitignore File]([https://docs.microsoft.com/en-us/certifications/azure-fundamentals/](https://www.atlassian.com/git/tutorials/saving-changes/gitignore)](https://www.atlassian.com/git/tutorials/saving-changes/gitignore))



