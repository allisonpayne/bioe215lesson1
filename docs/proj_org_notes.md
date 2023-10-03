# How to set up a project

## 1. Create an RStudio project

Create a new project. The directory name is the name of the project.
Make sure that "Create a git repository" is checked.

*Note: Stick to letters and numbers, and avoid special characters.*

## 2. Create a git repository

usethis::usegit() usethis::git_default_branch_rename()
usethis::use_github()

## 3. Set up folder structure

Good folders to include in the root folder: -data -paper (for the
manuscript) -figs -output (models, processed datasets, etc.) -R (R
scripts defining functions) -reports (quarto documents) -docs (rendered
versions of the quarto docs) -scratch (early prototypes, random stuff)

Scripts should live in your root folder unless things get really
complicated.

If you don't want to share your data, call
usethis::use_git_ignore("data/\*").

## 4. Activate GitHub pages

Create "index.md" in your docs folder. This is your readme!

Go to your Github repo, click on settings, code & automation, and choose
pages. source should say "deploy from a branch" branch should say "main"
directory should say "/docs" Save!

Go back to git. Commit and push index.md and Github will render the
site.
