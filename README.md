# CS11A-Final-Project
some kind of card game java program

Data structures:
  SLN: singly linked node; it holds some data and a pointer to the next node
  SLL: singly linked list, composed of unlimited number of SLNs, connected by pointers
  (A SLL forms a directional list - you can only traverse it in one direction (head to tail). It's different from arrays in that you don't
   have to specify the size of it at initialization, and this is the case in this game, since the number of cards players have is always 
   changing. However, a downside of it is that you can't access its element by indexing, i.e. you have to traverse every single element
   before to reach the desired element, which could hurt the running time. But since the max number of cards is 52, this shouldn't matter
   that much.)
   
Game structures: 
  Card: it has a value and a suit, and can be printed nicely
  PlayerGF: player for playing go fish only; enables the player to make certain moves (receive a card, ask for a value, etc) needed for 
            playing the game; also it stores what cards and books the player currently has, the number of cards, etc
  GoFish: where most stuff like game flow happens; holds info about the game (who the players are, what are the cards in the pool, etc)
   
For printing only:
  CardSuitsValues: it only holds some numbers for printing the suit symbols and some strings for suit names. 
  
Console: very very simple driver class, think of it as the main method in a java class; allows the user to play the game multiple times
