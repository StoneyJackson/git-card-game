# Super Basic Rules

The goal of this variant is to illustrate the relationship between push and pull operations and their impact on a shared project.

## Goal

Cooperatively complete all issues in the fewest number of rounds.

## Cards

To play this variant, you need only the following cards.

- Push
- Pull
- Change
- Error
- No Error
- Issue

## Setup

- Each player draws 5 action cards into their hand.
- Each player draws 1 issue card and plays it face up in front of themselves. This represents a feature branch in their local repository.

## Play

Each turn a player can play one change card and as many non-change action cards as they want. To end their turn, they replenish their hand to 5 cards by drawing more action cads.

The goal is to complete issues. Each issue has a size. That's the number of change cards that must be played on the issue before you can push it and complete that issue.

Once you have played enough change cards on an issue (equal to the size of the issue) you may push it to the team's shared repository, completing that issue. When you push an issue, all other players must place a stale token on their local repository if they don't already have one, and draw a number of risk cards equal to the number of changes in the issue you just pushed or the number of changes in their local repository, which ever is smaller. They place them face down above their issue pile.

If you have a stale token on your local repository, that means there are changes in the shared repository that are not in your local repository. Which means that you can't be sure if your changes are compatible with those in the shared repository. To remove the stale token, you need to play a pull card to pull those changes into your local repository. When you play a pull card, remove the stale token and flip over the risk cards on top of your issue pile. Now you can get busy addressing each risk one at a time.

Note, you cannot push an issue that has a stale token or unresolved risks.

Risk cards are either "Error" or "No Error". "No Error" cards are resolved simply by discarding them to the risk discard pile (you got lucky). "Error" cards are resolved by playing a change card. Remember, you can only play one change card per turn, and playing a change card to fix an error counts toward that quota. When you play a change card to resolve an error, discard both cards.

## Variations

You may want to try varying the following and observe their impact on play:

- Varying the number and sizes of issues.
- Vary the ratio between Error and No Error cards to change the chance that changes will conflict.
- Reduce the number of pull cards to force folks to develop on stale local repositories.
- Reduce the number of change cards to model the idea that some changes are harder to make than others.
- Try playing adversarially. Each issue is worth a number of points equal to its size. The goal is to complete the most number of points. See what strategies emerge which might suggest things you should avoid when developing in a team.
