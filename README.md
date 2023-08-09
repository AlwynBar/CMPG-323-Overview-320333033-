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
