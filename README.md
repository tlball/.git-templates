# git-templates
A listing of git templates to use globally or in individual git projects.

## Setup

### Individually
To use these scripts individually, clone this project, and copy any desired file to the same relative path within your project's `.git` directory

### Globally
Note: If using these templates gloablly, all scripts will be used for any project that is cloned or initialized.

`$ git config --global init.templatedir '<PATH/TO/THIS/PROJECT/CLONE>'`

This tells git to copy everything in this project to your per-project .git/ directory when you run `git init` or `git clone`.

## Current Scripts
### Hooks
[prepare-commit-msg](hooks/prepare-commit-msg)
* Extracts Story ID number from start of branch name, and writes it to the start of the commit message, using bracket notation.

An example:

For branch `1539685-cool-feature`, a commit message will start with 

```
[#1539685]
 Please enter the commit message for your changes. Lines starting
 with '#' will be ignored, and an empty message aborts the commit.
 On branch 1539685-cool-feature
 Changes to be committed:
.
.
.
```
