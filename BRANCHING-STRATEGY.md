# Branching strategy.

## I have used Trunk based branching strategy in the whole assignment.
- I used trunk based branching strategy because it consists of short lived feature or target branches which gets merged after each small and frequent update.
- Trunk based branching strategy results in faster development as there are fewer commits since the developers merge their feature or target branches daily, leading to fewer and less complex merge commits.
- Trunk based branching strategy also helps in Continous integration, which means the latest code generally is present in the main branch fully tested and ready to be deployed.

## Branch diagram

![Branch diagram](screenshots/Branch%20diagram.png)

## When to branch, From where, How to name branch?
- When to branch? One should branch whenever there's a chance of breaking the existing workflow. For example :- 
    1. Fixing a bug.
    2. Documenting the project.
    3. Working on a new feature.

- From where? It depends, but generally the main consists of the production ready code so it makes sense to work on the stable version to work upon though in some teams there exists a development branch where developers contribute their code and if the code is up to the mark it gets merged in the main branch. So to answer this question it depends on the team's workflow.

- How to name branches? A good branch name is very important for everyone in the team to understand what a specific branch does in the repository so it makes sense to format it with category/description. For example :-
    1. feature/add-sidebar
    2. hotfix/recovery
    3. feature/add-navigation

## When to rebase vs when to merge?
- One should rebase when they want clean linear history but very carefully as it rewrites history, so one should never rebase on a shared public branch or a branch on which multiple developers are working on. As it can break everyone's history resulting in tons of merge conflict.
- Merge generally compares the tip of two branches and tries finding a common ancestor to merge the two tips of the branch also called as the 3 way merge. Merge is generally used whilst working on a remote or shared respository on which multiple developers are contributing.