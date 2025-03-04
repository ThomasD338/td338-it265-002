<!-- Markdown Docs: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax -->
## Name: Thomas Deolall
### Module: 5

<!-- Repeat the below as needed-->
### Date: [03/03/2025]

#### Goals for this Module
<!-- Example Template (include the brackets to make a checklist, fill them in as appropriate
- [ ] Goal 1
- [ ] Goal 2
- [ ] Goal 3
-->
- [ ] Submit game design treatment
- [x] Brainstorm board game idea
- [x] Create and edit the living game design treatment document

#### Progress
- **What I accomplished**:
  - Summarize completed tasks or progress made.
  - This week I made pretty substantial progress towards brainstorming my board game concept. I landed on a 3-player, cooperative board game where players are able to coordinate their attacks to take out all of the enemies on the hexagonal grid map. Each player has their own deck of cards that they draw from and dictate what they can do each turn. As they get hit and take damage, they add "injury cards" to their deck, which will bloat their deck and hinder their ability to pull the cards they want.
  - I created [a new page](https://thomasd338.github.io/td338-it265-002/GameDesignTreatment) to record things about my game.
  - I wrote out details for some of the spells, items, equipment, and weapons for my game and transferred them to some index cards.
  - I tried "playtesting" my game solo to get a feel for how the game plays. The dynamic I really like about it is that there aren't any conventional "turns" between the players. Player 1 can attack, then player 2 can cast a spell, and then player 1 can move or use an item after the spell. Mixing and matching when each player goes could make for some awesome coordinated plays!
    
- **Challenges faced**:
  - Describe blockers, bugs, or issues encountered.
  - Problem 1: In the first iteration of my game, which took place on a long, square grid that enemies would move down, I had a very difficult time making the enemies' movement down the board interesting. My solution at the time was to have the player roll a die, and that roll would determine how the enemies would move. This had several problems. If the one roll would determine all of the enemies' movements, they'd all move in the same direction (if the roll said to move left, no enemies would be on the rightmost column. Boring!). If one roll decided just one enemies' movements, you would likely have to roll 10+ times just to move the enemies. I landed somewhere in the middle, where one roll decided the movement for one of the three types of enemies, so you would only have to roll 3 times. Still, these rolls were also on top of rolling to randomly spawn in enemies, so the enemy-phase was simply not fun at all for the player to manage. On top of this, when enemies would move in different directions, sometimes they would try to land on an occupied square, or two enemies would attempt to move to the same square simultaneously. Rolling an moving every enemy piece was already a lot for the player to do, but to then have to deal with following the rules on how to resolve these edge cases made me realize that there was a pretty significant flaw with the whole "enemy movement" system.
      -TL;DR: Old version of game had the chore of rolling a bunch to move all the enemies, on top of having a bunch of edge cases.
  - Problem 2: How would enemies spawn onto the board?  I could randomly select an open tile, but how would one convert a die roll into a random hex tile on a board that constantly changes which tiles are valid and invalid every turn? I could reserve a select few tiles for enemies to spawn, but then the enemies would always be grouped up in the same spot!
  
- **Solutions**:
  - Detail how you addressed challenges or your thought process.
  - Problem 1: The old version didn't have any actual player tokens on the game board; they simply just casted spells and attacks wherever the felt like. Putting the players down as actual game pieces made it so that the enemies didn't have to move, the players would! It also solved a lot of smaller issues, such as implementing the injury cards mechanic that I liked from other games as well as giving players a bit more to do than just throw a bunch of spells down on the board. Now players' spells/attacks can actually harm their allies.
  - Problem 2: I made these two "obelisks" that sit on the vertices of the hex tiles (where the settlements sit in Catan). At the beginning of the enemy's turn, enemies would spawn only on the three tiles that the obelisk is touching. Then the obelisk would move a random amount of spaces, orbiting around the central hexes on the map. If a player is on one of these three hexes when an enemy is supposed to spawn, they relocate their piece to a safe tile, drawing one injury card for each tile they must move. This solution spreads out the enemy spawns while giving the players a reactable way to respond to where the enemies will spawn next round.

#### Learnings
- Key insights, techniques, or concepts explored.
- Board games are a lot more susceptible to "chores" than video games. Any sort of randomness that would usually be handled by a function call in game code is now a drawn card, coin flip, or die roll from the player. It's why Balatro would NEVER work as a physical card game. Calculating every hand that you play when their scores can literally exceed the integer limit would not be fun.

#### Free Thinking
- Brainstorm or reflect on design ideas, architecture patterns, or potential improvements.
- Going forward, I need to figure out a few things for my game. How do the players win? How do they lose? I don't have a system for them to draw new cards either. There are still a lot of very large holes in my game, but from the minimal amount of playtesting I've done I at least know that the core gameplay is enjoyable.
<!--Your entry here or N/A if not applicable for this entry-->
<!--

- Example prompts:
  - "What if the player interactions were asynchronous instead of real-time?"
  - "How could ECS improve performance in this system?"
  - "Does my current design support scalability? How can it improve?"
  
-->

#### Next Steps
- Tasks or experiments to focus on during the next session.
-  <!--Your entry here or N/A if not applicable for this entry-->
