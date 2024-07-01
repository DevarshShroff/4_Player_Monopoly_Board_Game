#4-Player Monopoly Board-Game

I have created this game of Monopoly for those who wish to enjoy the game virtually.
The rules of the game are easy,direct and at each steps of the game, the system enables the player to enjoy the game with its smooth functioning. It provides functions like **pausing** the game and **continuing** at a later point in time, allowing the users to play at their convenience.

##The Game has the following elements:

**Player info:** Choosing number of players and corresponding token names.
    
**Dice Double:** Gives random values for a dice roll.

**Property:** Checks the Board-info and player-info dictionaries and performs transactions like buying, paying rent and increasing rents etc. 

**Community**/**Chance:** Checks chance cards and performs the action of deducting and depositing money to the corresponding player.

**Tax:** Gets called when the player lands on income tax and deducts $200 (fixed rate).

**Go:** Gets called when a player crosses Go and deposits $200 into the player’s account.

**Parking:** Gets called when a player lands on parking and greets the player with a message of a free and a safe stay. 

## How it Works 
The Main Loop *irritates* through all the player's *key* from the **player info dictionary**. A random *dice output* for each player and adds it to their *position* and shows the choices that the player can make according to type of place they have landed on. Before making *purchases*, the *UDFs* check for *availability of funds* and shows status to the player, in order for the player to make the decisions. The Game continues until one player remains while the other lose due to bankruptcy. All the *game constriatns* are applied through **if-else statements**, **dictionaries** and *game actions* are operated **through the UDFs**.   

## How player data is stored and used 
**ASCII** files for are created for every player playing storing important variables like *positions*, *balance*, *places owned* and *number of hotels made at evey house owned*. All this **attributes** are saved after every round of the game, when resuming the game at a later point this files are used to **populate** the *player info* and *board info dictionaries* resuming the game where the players left it.

 

