# Notes From POSSE 6/17/2016

## Action/Operation cards

- stage: Play to move any number of change cards in your working tree to the stage.

- commit: Play to move all changes in the stage to the local repository.

- push: Play to move all commits in the developer's local repository to the remote repository. When played, all other developers must draw a number of trouble cards equal to the minimum of the number of change cards in their local repository and the number of change cards pushed to the repository. Place these face down in your local area. You cannot push if another developer has pushed changes sense your last push.

- pull: Play to update your local repository with changes from the remote repository (do not move any other cards). Turn over any trouble cards. Now you may begin resolving trouble cards by playing a change cards. Each time you play a change card to resolve a trouble card, discard both the change card and the trouble card.

- clone
- fork (github)
- pull request (github)
- fetch
- rebase
- squash

- branch


## Trouble/Risk cards
- conflict/merge fail
- new changes
- errors
    - CI
    - Style
    - Compile
    - Test
- Poor implementation
- Poor design
- license violation
- Introduce dependency
- Ugly commit history
- Got lucky (no problem/blank)
- Speling Eror


## Artifact cards
- change: Represents a change to the source code. Each developer can only play changes in his/her local machine. Change comes in different colors (representing different types of changes) and color doesn't matter if you're not using staging
- issues: Each has a size indicating the number of changes that must be commited to complete the issue.
- branch


## Areas/piles/etc.
- Issue tracker - pile/pool of issue cards in the middle
- Local machine
    - Working tree - area immediately in front of developer
    - Stage - area just above working tree
    - Repository - area just above stage
- Remote repository - area in the middle
- Threat pile - where the trouble cards go


## Moves
- If you do not have an incomplete issue in your local area, draw an issue and put it face up in your local area
- You may do any and all of the following
    - Play at most one change card (change is effort)
    - Play any number of operation cards
    - Discard any number of cards
- Draw enough cards to refill your hand to X cards
- Your turn is over and play moves to the next developer widdershins (counter-clockwise)



## Extensions

- Simulating debugging
    - Everytime you play a change card (other than to remove an existing trouble card), draw a trouble card for every existing trouble card you have, plus one.
    - Play a test card to reveal one trouble card.

- Motivating staging
    - The stage can only contain changes of the same color.

- Motivating branches
    - If you draw an emergency issue, you must immediately play it (and draw another). You must complet this emergency issue before you can complete the issue you are currently working on. An emergency issue may interrupt another emergency issue. You must complete emergency issues in the reverse order that you received them.
    - You cannot commit partial implementations to the master branch. You have two choices:
        - If you have been working on the master branch, you may
            - Undo all the commits on the branch that have not been pushed (discard all changes in local machine)
            - Create a new branch to hold your current effort, stash or commit your current changes, move master back to were it was before you started your current effort, then create a new branch off of master for your new effort
        - If you have been working on a branch other than master, stash or commit your uncommitted changes, create a new branch off of master, work on your new branch.
