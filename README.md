# TrickPaperScissors

PlayingCards.io implementation of the game.

*Trick taking game with changing trump suits determined by lead suit. Must follow if possible, score points by winning tricks and change the value of those points by trumping.*

![Anatomy of a card](CardAnatomy.png)

### Rules

- Each trick, the lead suit establishes the trump suit according to **Rock** / **Paper** / **Scissors** rules i.e. **rock** trumps **scissors**, which trumps **paper**, which trumps **rock**. e.g. If **Scissors** leads this hand, **rock** will be trump.

- Winning a trick with a *lead* suit card
  - Player takes the trick and scores a number of points from the stars on the *lowest* card of the *lead* suit in that trick.

- Winning a trick with a *trump* suit card
  - Player may change the *value* of the points of the *trump* suit
  - Alter value by one step between -1 <-> 1 <-> 2
  - At the start of a game, every suit's value begins at 1

- In either case, the winner of a trick leads the next trick.

- When all tricks have been played, calculate each player's total score by multiplying the number of points in each suit by the value of points in that suit.

Highest sum of all three suits wins.
