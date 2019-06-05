# Blackjack
//Pseudo-code and documentation goes here

Team Members: Elizabeth Arias, Joseph Murray, Jason Ibrahim


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
