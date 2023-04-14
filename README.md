# TrickPaperScissors

PlayingCards.io implementation of the game.

*Trick taking game with changing trump suits determined by lead suit. Must follow if possible, else able to trump.*

### Rules

- Lead suit establishes trump suit according to **Rock** / **Paper** / **Scissors** rules i.e. **rock** trumps **scissors**, which trumps **paper**, which trumps **rock**. e.g. If **Scissors** is lead this hand, **rock** will be trump.

- Winning a trick with a *lead* suit card
  - Player takes the trick and scores a number of points equal to the lowest card of the *lead* suit in that trick.

- Winning a trick with a *trump* suit card
  - Player may change the __value__ of the points of the *trump* suit
  - Move one step between -1 <-> 1 <-> 2
  - At the start of a game, every suit's value begins at 1

- The winner of a trick leads the next trick.

- When all tricks are played, total score is number of points in each suit multiplied by their value.

Highest total wins.
