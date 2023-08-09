# Projects_CMPG_323
# Repositories that will be used and added :   
Cmpg 323 Overview 32033303
# Diagram:
# ![Diagram](https://github.com/AlwynBar/CMPG-323-Overview-320333033-/assets/80039379/5842a83f-03bc-4008-8f68-748aced6a929)
# Branching strategy:  
GitFlow is a branching model and workflow for version control using the Git version control system. It was popularized by Vincent Driessen in 2010 and provides a structured approach for managing and organizing the development of software projects, especially larger and more complex ones. The GitFlow workflow defines specific branches and their purposes, helping to maintain a clear separation of concerns and facilitating collaboration among developers.

Here's an overview of the main branches and concepts within the GitFlow workflow:

Main Branches:  
master: This branch represents the stable and production-ready state of the project. Code in the master branch is expected to be of high quality and free from critical bugs.
develop: This branch serves as the integration branch for ongoing development work. It is where features, bug fixes, and other changes are combined before being tested and eventually merged into the master branch.

Supporting Branches:
feature branches: These branches are created for developing new features or enhancements. Each feature is developed in its own isolated branch. Once the feature is complete, it can be merged into the develop branch.
release branches: When the development work on the develop branch has reached a stable point and is ready for release, a release branch is created. This branch allows for final testing, bug fixing, and preparation for deployment. Once everything is ready, the release branch is merged into both the master and develop branches, and a version tag is usually applied.
hotfix branches: In case critical bugs or issues are discovered in the master branch, a hotfix branch is created. Hotfix branches allow for quick bug fixes to be applied and tested. Once the hotfix is ready, it's merged into both the master and develop branches.

Workflow Steps:
The typical workflow in GitFlow involves the following steps:
Create a feature branch: Developers create feature branches from the develop branch to work on specific features or changes.
Develop and test: Developers work on their features, making commits and testing their changes in isolation.
Merge to develop: Once a feature is complete and tested, it's merged into the develop branch.
Create release branch: When the develop branch is stable and ready for release, a release branch is created from it.
Test and finalize: The release branch undergoes testing, bug fixing, and final preparations.
Merge to master and develop: After thorough testing, the release branch is merged into both the master and develop branches. A version tag is often added to mark the release.
Hotfix branches: If critical issues are found in the master branch, hotfix branches are created, fixed, and merged back into both master and develop.

The GitFlow workflow promotes a structured and organized approach to development, making it easier to manage releases, coordinate teamwork, and maintain a stable production environment. However, it can be relatively complex, especially for smaller projects, and there are alternative branching models and workflows that might be better suited to certain development scenarios.
# The use of .gitignore:
A .gitignore file is a powerful tool in the realm of version control using Git. It serves as a configuration file that specifies which files and directories should be ignored by Git, meaning they won't be tracked or included in the repository. This is particularly useful for excluding files that are either generated automatically, contain sensitive information, or are not relevant to the version control process. Here's why the .gitignore file is important within each project:

Exclude Unnecessary Files: Many projects generate files that are not essential for collaboration or distribution. Examples include compiled binaries, log files, temporary files, and cached data. By adding these patterns to the .gitignore file, you prevent them from cluttering the repository and potentially causing conflicts or increasing its size unnecessarily.

Protect Sensitive Information: It's common for projects to include configuration files containing sensitive data like passwords, API keys, and tokens. Ignoring these files with .gitignore ensures that such sensitive information isn't accidentally exposed in the repository's history or to unauthorized users.

Avoid Platform-Specific Files: Some development environments generate platform-specific files that might not be relevant to all contributors. These files can include IDE settings, build artifacts, and editor-specific configuration files. Using .gitignore can prevent cross-platform issues and make the project more accessible to different developers.

Enhance Clarity: Ignoring unnecessary files helps maintain a clean and focused version history. When you're browsing the history or changes of a project, you'll be able to focus on meaningful changes and avoid distractions from irrelevant files.

Facilitate Collaboration: When working in a team, the .gitignore file ensures that everyone is on the same page regarding which files are considered disposable or irrelevant to the project. This minimizes confusion and potential conflicts.

Speed up Git Operations: Excluding large or unnecessary files from being tracked by Git can significantly speed up operations like cloning, pushing, pulling, and branching, as Git doesn't waste time processing irrelevant data.
