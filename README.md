# Blackjack
//Pseudo-code and documentation goes here

Team Members: Elizabeth Arias, Joseph Murray, Jason Ibrahim

1. What problems are you solving in this project?

A. The purpose of this program is to simulate a game of Blackjack using one deck of 52 cards, and calculate the probability of player advantage. It should update the probability of player advantage with every card drawn.


2. What solutions are you implementing in the project? 

A. Based on what the player draws the suggestion of whether to hit or stand is given and additionally they are given the probability of that the card the need to reach 21 can come up considering what has already been drawn by both the dealer and player.


3. Provide explanation of calculations and algorithm implementation.

A. The program makes calculations in the program based on the value that it assigns to each card. The program creates a matrix of 13 ranks and 4 suits to automatically enumerate all 52 cards in the deck. There are 4 versions of each rank, and a function determines the value of the rank. The gameplay process is a sequence of algorithms, for example, the card drawing loop that checks when the player or dealer busts every time a card is drawn and added to the score sum.


4. What is the program objectives? Explain how your program is interacting with the user and it's purpose.

A. The purpose of this program is to simulate a game of Blackjack for the user and provide the probability that the player will win based on the likelihood of drawing a satisfactory card. At the visual level, the program will display two of the users cards and one of the dealers cards. The user will be prompted to "hit" or "stay" and be given a probability of advantage. With each "hit", the player advantage will update to give the user the opportunity to use their judgment when making their next decision.


5. How is discrete structures implemented in the C++ program?

A. The forumula for proability is integrated into the program in order to calculate the probability.


6. What are the limitations of the program?

A. The program does not simulate games with more than 2 participants. [IN IT'S CURRENT STATE: (6/4/2019 7:19PM) ] The program does not provide probability calculations for player advantage.


7. Provide recommendation on improving the limitations of the program.

A. If the program only provides probability calculation, it should also provide the chances of busting on the next draw and winning, or getting a score 21 on the next draw. This offer even more advantage for the player to make decisions when drawing.





Pseudocode

    Shuffle deck
        for all values between 0 and 3 and...
        for all values j between 1 and 12...
            enumerate all 52 cards in the lattice
                generate random number
                rearrange elements in the range of mainDeck

    Calculate Points
        Assign value to each rank
        Pointer-to-card function
            remove pointed-to card from array

    Game Process
        Deal first cards of the round
            Display player cards
            Display dealer card and hidden face-down card
            get points for the player
                if player score is equal to 21...
                    win, restart sequence
                if player score is less than 21...
                    input H to "hit"
                        pointer-to-card function
                            if player score is more than 21...
                                lose, restart sequence
                    input S to "Stay"
                        end player turn
            get points for the dealer
                while dealer score is equal to or less than 16...
                    pointer-to-card function
                        if dealer score is greater than 21...
                            player win, restart sequence
                        if dealer score is equal to or greater than player score
                            player lose restart sequence
