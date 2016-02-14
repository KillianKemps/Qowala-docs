# Contribute

To keep consistency in the quality of our work, we have set up the following workflow for developing new features on Qowala.

All development and Merge request must be done on this Gitlab: [https://git.framasoft.org/KillianKemps/Qowala-live](https://git.framasoft.org/KillianKemps/Qowala-live "https://git.framasoft.org/KillianKemps/Qowala-live")

## Request for a feature

### For internal collaborators
1. Create a User Story (US) which address one user's need
2. Create tasks in the US for each technical part
3. Put the US in a sprint

### For external collaborators
1. Open a Bug or a Enhancement issue with a clear description.
2. If the issue is an Enhancement and is approved by the internal collaborators, it will be later on integrated in a sprint to be developed.

If you want to develop the feature yourself, just do a Merge Request on the Gitlab repository with a detailed explanation.

## Feature development

1. During the feature development, you have to open a Merge Request on the Gitlab repository with a `[WIP]` prefix while it is still Work In Progress (it will avoid it to be merged accidentally).
2. Once the feature development finished and that all unit tests passes, you can remove the `WIP` prefix from the Merge Request name. 
Then ensure the Merge Request contains the following:
    - ~~In the title: the name of the Taiga's task `TG-XX` and the `#ready-for-test` status~~. (Removed from the process because some issues were encountered when pushing several times commits)
    - You assigned yourself to the Merge Request
    - A clear description of the feature
    - A link to Taiga's related task
    - A checkbox helping to understand the steps if the feature is quiet complex
    - A Warning concerning the feature effects if needed

3. Let the internal collaborators know that the feature is finished so they can review your Merge Request
4. Once you get the approval from at least one developer, you can merge the feature
5. Taiga will be automatically updated and the development server too.
6. Another internal collaborator has then to test the feature on the development server to check if everything is allright and if the specifications are reality-proof
7. Once the collaborator has verified the feature online, he has to update to feature status on Taiga to `#done`
8. Once all features of a sprint has been finished, the develop branch is then merged into the master branch and the new release is done