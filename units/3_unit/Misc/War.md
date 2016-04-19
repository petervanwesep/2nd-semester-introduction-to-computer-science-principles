##War

Today we will begin implementing a version of the card game [War](http://www.pagat.com/war/war.html).

Here is your starter [code](https://gist.githubusercontent.com/petervanwesep/89737f79bc638c7539d954e03f9cb80f/raw/deed1de02df5112a53fe9a7b7056547109b32446/war.py).

For simplicity, Jacks will be represented as 11, Queens will be represented as 12, Kings will be represented as 13, and Aces will be represented as 14

We will not be paying attention to suits.

##Part 1: play_game(), compare_scores(), player_turn()

You will be implementing three new functions. Their contracts are included in the starter code.

The `play_game()` function has already been partially implemented. It uses a "game loop", similar to what was in Zork. On each turn, your program will choose a card for each player, compare their values and increment each player's score appropriately.

If a player draws a larger card, they should get one point. For the first part, if the two cards are equal, your code should give one point to each player.

##Part 2: Closer to War

Add a new function `war()`. This function will take both players' names and the deck as an argument. It returns the name of the player who wins this war, or the empty string ("") if nobody wins.

To decide the winner, the function will draw 3 cards for each player. The value of the third card will decide the winner. The player whose name is returned by this function gets 4 points instead of the usual 1. If the cards are equal again, neither player will receive any points.

Note: This function should only be called if the players' cards are equal. If the cards are not equal, `compare_scores` should be called as usual.

##Part 3: Full Metal Jacket

Implement the actual game of "War" as specified [here](http://www.pagat.com/war/war.html).

Some notes:

* Each player should have their own pile of cards, which are dealt from the shuffled deck, and they should also have their own discard pile.
* During a war, as long as players continue to play the same card, the war should continue. The winner takes all cards that were played and adds them to their discard pile.
* Once a player goes through their deck, their discard pile should be reshuffled and reused as their deck.
* You should revise the code in `player_turn` so that instead of printing 11, 12, 13, 14 it prints "Jack", "Queen", "King" and "Ace" respectively.
* The winner is the player who wins all of the cards.