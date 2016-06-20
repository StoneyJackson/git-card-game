# Rules: Basic

## Players

2-4 players

## Equipment

- Cards: see card-list.md
- Stale tokens: (any small object like a coin will do)

## Setup

1. Create a shuffled Risk card pile
2. Create a shuffled Issue card pile
3. Create a shuffled Action pile from the rest of the cards.
4. Each player draws 5 cards from the Action pile into his/her hand. Do not show them to the other players.

## Definitions

A player's local repository is the area immediately in front of that player.

## Order of Play

1. Agree on a number of points to play to. 10 points is good.
2. Play begins to the player counter-clockwise of the person who shuffled the Action pile.
3. On your turn:
  2. If you do not have an active Issue pile, create one by placing an Issue card face up in front of you.
  3. Play cards
    - You may play no more than one Change card per turn.
    - You may play as many Operation cards as you like, as long as they are legal plays.
    - You may discard as many cards as you like.
  4. Replenish your hand by drawing from the Action pile until you have 5 cards again.

## Goal

The goal is to be the first player to 10 points by completing Issues. Each Issue has a size value. When you complete an Issue, you earn points equal to that Issue's size. To complete issues you need to Push a number of Changes equal to the size of the Issue. You can only Push changes that have been Committed, and you can only Push when you have Committed enough Changes to complete Issue.

## Making a Change

To make a Change, play a Change card by laying it face up on top of your active Issue pile slightly staggered so that you can see all of the underlying cards. If your repository has a stale token, each time you play a Change card, draw a Risk card and place it face down without looking at it next to your active Issue pile.

### Committing Changes

To Commit Changes, play a Commit card by laying it face up next to your Change cards. A Commit card Commits all Changes since the last Commit card you played.

### Pushing Changes

You cannot push an uncommitted Change. You cannot push if you have unresolved Risk cards. You cannot push unless the active Issue pile has Change cards equal to the size of the Issue.

To Push Committed Changes, play a Push card by laying face up next to your active Issue pile. Place a stale token on each other player's local repository, and deal face down to each other player a number of Risk cards equal to the number of Change cards you are pushing or the number of Change cards in his/her local repository, whichever is less. They cannot look at these Risk cards, and place them face down next to their active Issue pile. The Pushing player places the completed Issue card face down in front of himself/herself to indicate that the Issue is complete, and discards the other cards in the now complete Issue's pile.

### Stale Tokens and Risk Cards

To remove a stale token from your local repository, you must update your local repository using a Pull operation. To play a Pull card, place it face up on your active Issue pile, remove the stale token, and flip over any Risk cards.

Any Risk cards in your local repository must be resolved before you can play a Push card. Risk cards must be face up before you can try to resolve them. To resolve a Risk card, follow the directions on that card and then discard it.

Some Risk cards require you to play a Change card to fix. Change cards played this way are played face down on your active Issue stack and behave exactly like other Change cards except that they do not count towards the Issue size.
