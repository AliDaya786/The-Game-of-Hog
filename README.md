# The-Game-of-Hog

In Hog, two players alternate turns trying to be the first to end a turn with at least 100 total points. 
On each turn, the current player chooses some number of dice to roll, up to 10. 
That player's score for the turn is the sum of the dice outcomes. However, a player who rolls too many dice risks:

Sow Sad --> If any of the dice outcomes is a 1, the current player's score for the turn is 1.

Hefty Hogs --> If the opponent's score is 0 and the player chooses to roll zero dice, the player will get 1 point. However, if the opponent's score is not 0, a player who chooses to roll zero dice will gain points according to the following:
 - The opponent's score will be mapped to a series of functions to be applied to the player's score, starting from the rightmost digit (the one's place) and ending on the leftmost digit.
 - Each digit from 0 to 9 corresponds to a pre-defined function, f0 through f9.
 - The result of this series of calls modulo 30 is the amount of points the player receives for the turn.
