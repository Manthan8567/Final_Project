# Information System Development

## Project Proposal

> PUBG (Player Unknown Battleground)

-  I chose PUBG (Player Unknown Battleground). Which is a battle royal game with different modes of game. I chose this game because I have played this game many times and I am very familiar with the all aspects of this game. Here, I choose one of its game modes which is called TDM (Team Death Match). 

-  Team Death Match: is a mode in the game where you play with 3 other players (total 4 players including you) with another team with 4 players on a smaller map than the usual Battle Royale Maps. Your team's aim is to get a certain number of kills (mostly 40) in a limited amount of time to win.

-  First, user can join with other 4 players or they can start this mode with the random players. As soon as player joins the team with other three players, every player must be ready to start the match. After starting the match, each team player spawns in their side of spawn area. Where they get certain seconds (30 secs) to choose the weapon, attachments of the weapon, ammo, and frags. User can choose 2 weapons, primary and secondary. As soon as the match starts, the 5 min timer also starts to countdown. Players of both team starts to attack each other. If a player takes the damage from the opponent, the player heals himself automatically within few seconds. If a player kills the opponent his team gets a point and the score bar updates and player can also pickup the loot of the killed player. Once the player dies, they respawn in the spawn area again. After killing the opponent, player’s individual kill count also updates on the screen. Within the time limit of 5 mins, the team who reaches first to the score of 40 wins the match. If both team reaches the time limit of 5 mins, the team with the highest score wins the match and the other team looses the match. If both team scores equal at the end of the time, the match goes to the extra play time of 2 mins and the result of the match is decided with the highest scoring team by winning the match. Even in extra time, if both teams score equally then the match ends in a draw. Also, after finishing the match, the result screen appears where individual can check their kill counts and everything and among the winning team players, the player with the highest kill count gets a tag of MVP (Most Valuable Player) of the match. 


## Flowchart Diagram

>  First, Player joins the lobby with other players. If everyone is ready then the match will be started else, the match can not be started. After starting the match, each team players spawns in the opposite sides of the spawn area. In the spawn area, player can choose their preferred loadouts for the match and then starts to fight. If a player takes a damage and dies, they respawn again in the spawn area and then they can change the loadouts and start to fight again. Else, if they kill the opponent the damaged player gets heal automatically and the score bar updates with the individual kill counts on the player screen. If any team reaches first to the score of 40 then the team wins the match, and the match result shows at the end with the MVP of the match. But if the time is over before any team reaches to the score of 40, then the game goes for overtime of 2 minutes. Within the overtime, if the score of the match is equal at the end, then the match is declared as a draw else, the team with the highest score wins and the result screen with the MVP of the match shows at the end. 

![Flowchart_diagram](https://github.com/Manthan8567/Final_Project_Information_System_Development/assets/124721292/e3513433-6766-4045-9568-1ea635ed29cf)
  

## Class Diagram

>   In the class diagram, the Lobby class has a list of Player objects, a reference to a Map object, the current game mode represented by the GameMode class, field to add or remove players. The Match class has a list of Team objects, a reference to a SpawnArea object where players will spawn in, a score limit for the match, the current time during the match, and methods to start, update, check if the match has started or finished, get the result, MVP, and score limit of the match.
The Team class has a list of Player objects, as well as field to remove or add players in the team, field to get the team score and update score to the match.
The Player class has a reference to a Loadout object, which represents the player's equipment and weapons, as well as their position on the map represented by the Position class. The Player class also has a field for the player's health, number of kills, number of deaths, and methods to spawn in the SpawnArea, get their loadout.


![Class_diagram](https://github.com/Manthan8567/Final_Project_Information_System_Development/assets/124721292/70dd8d9f-a784-4b07-9705-25e85e688ae0) 

## Sequence Diagram

>  In the sequence diagram, we can see that first player sends a request to
   server to start the match then server responds to player that the match is started
   and also responds to Enemy (opponent) that the match is started.
 - The diagram shows sequence of events that occur during the match. We can see
   that in a if-else condition, if player shoots at the enemy then enemy health gets
   decreased and the score bar updtes. Then scorebar resonds server that the
   score is updated and the enemy is dead. Else, the enemy shoots at the player
   then player health gets decreased and the score bar updates. This process takes
   place in a loop from shooting at the opponent to score bar updates and player
   respawn in the match.
 - In another alternative box with if-else condition, if player team score 40 points
   then it asks the server and then server confirms with score bar for player team’s
   score. The score bar replies with yes or no. Else, the same Enemy team asks the
   server for score confirmation. Either team scores 40 points win the game.
 - This whole process also takes place in the alternative box. Where with the
   condiotn is If then the whole match process takes in place. Else, it’s end.

![Sequence_diagram](https://github.com/Manthan8567/Final_Project_Information_System_Development/files/15104266/20230308092725_Final_Project_Sequence_Diagram.pdf) 
