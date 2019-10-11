#Project1: Concept

##Jiahao Song, Hao Yuan, Chen Gu

####What game are you going to build?

We are going to build a classic Reversi game. 
Reversi is a strategy board game for two players, played on an 8×8 uncheckered 
board. There are sixty-four identical game pieces called disks (often spelled 
"discs"), which are light on one side and dark on the other. Players take turns
 placing disks on the board with their assigned color facing up. During a play,
 any disks of the opponent's color that are in a straight line and bounded by
 the disk just placed and another disk of the current player's color are 
 turned over to the current player's color. The object of the game is to have
 the majority of disks turned to display your color when the last playable 
 empty square is filled. 
 [Click here for WiKi](https://en.wikipedia.org/wiki/Reversi)

####Is the game well specified (e.g. Reversi) or will it require some game work
 (e.g. a monster battle game)?*
The game is well specified. Here are the rules:
####Basic rules
Each reversi piece has a black side and a white side. On your turn, you place 
one piece on the board with your color facing up. You must place the piece so 
that an opponent's piece, or a row of opponent's pieces, is flanked by your 
pieces. All of the opponent's pieces between your pieces are then turned over
to become your color. 
####Aim of the game
The object of the game is to own more pieces than your opponent when the game 
is over. The game is over when neither player has a move. Usually, this means 
the board is full. 
####Start of the game
The game is started in the position shown below on a reversi board consisting
 of 64 squares in an 8x8 grid. 
####Playing the game
A move consists of placing one piece on an empty square.	
####Capture 
You can capture vertical, horizontal, and diagonal rows of pieces. Also, you 
can capture more than one row at once. 
####Time control
A clock is used to limit the length of a game. These clocks count the time
that each player separately takes for making his own moves. The rules are very 
simple, if you run out of time, you lose the game, and thus must budget your 
time. 
####End of the game
The game ends when: 
One player wins, by making his color dominant on the board;
The players agree to finish the game (as a resignation, or a draw).
[reversi](http://www.flyordie.com/games/help/reversi/en/games_rules_reversi.html)

####Is there any game functionality that you’d like to include but may need to
 cut if you run out of time?*
All of the above criterias should be implemented to make this game work. 
Besides that, we also need to create a chat-room next to our chess board to 
allow observers and players communicate with each other by sending and 
receiving messages. Our app must support multiple “game tables” where players
can meet and play, and should support separate games being played at multiple 
tables at the same time. Some additional features that we might add into the
game but may need to cut are: 
####Create a leader-board to keep track of players with most win games.
Players who win a game will receive some game currency to purchase “skins” 
for their chess-piece or board.
#### What challenges do you expect to encounter?
With more than 2 users jump into our web page and channels, we might encounter 
some concurrency problems where users cannot send and receive messages 
properly. Also, the observers may not able to see the moves and updates 
occurring on the board. Player A can challenge many other players at the same
time, but only the first player who accepts the challenge will start a game 
with Player A. Other challenge requests should be nullified or be queued when
Player A gets into a game.
