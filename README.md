# card-die-game
 The program allows the user to choose between playing a card game or a die game.

 If they choose a card game, it first initializes the card game by creating 52 cards in a standard deck of cards and shuffles the cards by choosing two random cards and swapping them using a random number generator 100 times and then printing out the new shuffled card list. It then plays the main card game, by making the user to select two cards from the shuffled cards at random, saving these selections and displaying the chosen cards and the remaining cards in the deck. It then displays if they won if one of the cards is an Ace, else they lost.

 If they choose a die game, it first initializes the die game, plays the main die game by letting the user roll the die twice and generating a random number between 1 and 6 using a random generator on each turn, saving and displaying the numbers chosen. It then declares if the user won the die game if any of the numbers, they rolled was a 1, else, they lost.

Run Test.java to play the game.

Output:
![Screenshot 2023-08-11 at 4 24 15 PM](https://github.com/cedgark/card-die-game/assets/114522674/20ff8e4a-42de-4ed3-9975-ed416a6058ea)

The classes have been identified -

Input: Take in and store the game choice as user’s input.

RandomInterface: Defines an interface to get the next random number LinearCongruentialGenerator: Generate a random number between 0 and 1. 

GameFactory: Creates objects without exposing the instantiation logic to the client. 

Game: Refers to the newly created objects through a common interface.

CardGame: Play the card game for the user.

DieGame: Play the die game for the user.

Test: Run all the above classes in the correct order.

To maximize cohesion and minimize coupling each class does one thing only and its methods relate to that class (following the specific responsibility principle). And the classes are designed to have as little dependency as possible by depending on the interface rather than the implementation.
