# final-project
Counting cards agent with 6 decks 
https://colab.research.google.com/drive/1MbT2ln7QBO0N3AsNhddE87qLLu1TL9gM#scrollTo=CqBtm6_y_Pq9
Counting cards agent with 1 deck
https://colab.research.google.com/drive/1dHE0CGwupAzzlp2CguiImIGcFxTHkeVh#scrollTo=CqBtm6_y_Pq9


Blackjack is a game that is you vs the dealer. Everyone playing including the dealer is dealt two cards.
The game revolves around the sum of your cards. You can either decide to hit to add another card, or
to stand and stop recieving more cards. If your card total goes over 21 you bust and lose. If you card total is
less than 22 by also less than the dealers you still lose. You go first and hit as many times as necessary then
the dealer goes. The Dealer will always hit when the sum of their cards is less than 17. You make your bet 
before the cards are dealt. If you win you double your money if you lose the money is taken from you.
The game is played with a deck or multiple decks of cards. Kings, queens, jacks are worth 10, 
and aces are worth 1 or 11 depending on the sum of your cards.

Blackjack has the best odds of any casino game at 49% but that still means you will most likely lose
money over time. In 1962 Edward Thorp wrote “Beat the Dealer” which describe a stategy of counting cards that 
popularized the idea to the american public. Since the gambit has been referenced in pop culture like the movie
"Rain Man" or "21". The idea is that every time a card is dealt we keep track of it using a count to better
understand what cards are still left in the deck. If a low card (2-6) is dealt the count is increased by one.
If a 7-9 is dealt the count does not change. If an ace or 10 is dealt the count is decreased by one. This is
important because keeping track of the count can increase your earnings at the blackjack table. Theory says
that the higher the count the more you bet. A higher count means more 10’s and 1’s are left in the deck.
This increases your odds of getting a natural blackjack (being dealt an ace and a 10 that recives 
1.5 * the payout) or high card total. This is also important becasue the dealer must hit when anywhere less than 17
The dealer has to hit 12-16 (stiff hands) and when the count is high there is a good chance they bust.

I created an agent using Keras-rl that plays blackjack and counts cards. This agent's oberservation space
consists of the count of the cards before the the cards are dealt and the length of the deck. The agents action space
consisted of a range from 5 to 500 which were possible bets for the agent that would be used as the reward.
This agent played the exact same game as the dealer only hitting when it's card total was less than 17 but
learned to bet in effective ways and make money.


