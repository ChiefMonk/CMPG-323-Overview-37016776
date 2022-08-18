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


## Code Example
Let us see an example with X elements in an array and sort it.
```
using System;



## Output
Sorted Array:
```
[ 13 45 55 78 98 ]
```
## Contributors
* [Chipo Hamayobe](https://github.com/ChiefMonk) - Project Lead

## References
### Branching
* [What is the best Git branch strategy?](https://docs.microsoft.com/en-us/learn/paths/intro-to-vc-git/](https://www.gitkraken.com/learn/git/best-practices/git-branch-strategy))
* [Visual Studio version control docs](https://docs.microsoft.com/en-us/visualstudio/version-control/?wt.mc_id=learnredirect_githubvscode_content_cnl_csaapp&view=vs-2022)
* [Build community-driven software projects on GitHub](https://docs.microsoft.com/en-gb/learn/paths/build-community-driven-projects-github/)
### Azure Fundamentals
* [Microsoft Certified: Azure Fundamentals](https://docs.microsoft.com/en-us/certifications/azure-fundamentals/)



