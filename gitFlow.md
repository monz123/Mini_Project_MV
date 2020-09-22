### Git Flow
#### Definition
GitFlow is a stretching model for Git, made by Vincent Driessen. 
It has pulled in a great deal of consideration since it is very appropriate to cooperation and scaling the advancement group.
#### Key Benefits
#####Parallel Development
#####Collaboration
#####Release Staging Area
#####Support for Emergency Fixes

#### How It Works:
New development (new features, non-emergency bug fixes) are built in feature branches:

![GitWorking Img1](images/Picture17.png)

Feature branches are branched off of the develop branch, and finished features and fixes are merged back into the develop branch when they’re ready for release.

![GitWorking Img2](images/Picture18.png)

A release branch is created off of develop, when it is time to make a release.

![GitWorking Img3](images/Picture19.png)

The code in the delivery branch is conveyed onto an appropriate test condition, tried, and any issues are fixed legitimately in the delivery branch. This send - > test - > fix - > redeploy - > retest cycle proceeds until you're upbeat that the delivery is adequate to release to clients.
When the release is finished, the release branch is merged into master and into develop too, to make sure that any changes made in the release branch aren’t accidentally lost by new development.

![GitWorking Img4](images/Picture20.png)

The master branch tracks released code only. The only commits to master are merges from release branches and hotfix branches.
Hotfix branches are used to create emergency fixes:

![GitWorking Img5](images/Picture21.png)

They are spread straightforwardly from a tagged release in the master branch, and when completed are converged over into both master and create to ensure that the hotfix isn't incidentally lost when the following customary release happens.

[**Back to Home Page** :houses: ](/README.md)