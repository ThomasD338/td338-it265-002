## Concepts from other games I like:
- Decked Out, "stumble" cards: This was a game made in Minecraft on the Hermitcraft SMP server, basically it was a dungeon delver and players would have a deck of their own selected cards to aid them as they search for artifacts in the dungeon. After a certain interval of time, a random card would be drawn and its effect would be played. Additionally, stumble cards would slowly fill the player's deck as time went on. When these cards were drawn, they had a detrimental effect to the player. Stumble cards would also be added to the player's deck by other cards' effects, usually balanced by a very potent positive effect as a tradeoff.
- Dominion, Victory Point cards: The goal of Dominion is to have the most victory points at the end of the game. However, the cards that gave you victory points have no effect and cannot be played, essentially being a dead draw for the player. 
Summary: Dead/bad draws that are more detrimental to the player are cool

## OLD Concept
~~Cooperative board game, 3 players. Gameboard is an 8x4 square board. Enemies randomly spawn in at the top of the board and move downward, randomly selecting between one of three possible move options (ex.: moving left one column then down, just moving straight down, or moving right one column then down). Cast AoE spells to damage each enemy before the reach the end of the gameboard. 3 players cooperate to try and stop the monster force.~~
Issues found during quick playtesting:
- Rolling to see if an enemy spawns, then rolling to see how each one moves is very tedious and very roll-heavy.
- Enemies tend to bias towards the side columns instead of the center
- Many edge cases when an enemy tries to move to an occupied tile or if two enemies are trying to move to the same tile simultaneously.
- Felt very "all or nothing", no health system in place, so even just one enemy slipping by would be game over

# New Concept:
- Enemies mostly stay in place, avoids issue with movement in previous iteration
- Players are interactable figures on the gameboard
- Hexagonal grid allows for more interesting spell shapes and gives players access to more adjacent tiles with melee attacks
- Players can have one melee weapon, one equipped item, one spell, and an extra slot of their choice

# Deck Mechanic:
Several different card types:
- Attack: Lets player attack with their primary weapon
- Spell: Lets player cast a spell

# Spell Cooldowns
- After casting, flip card over to indicate that it is on cooldown. Flip it back over at the end of your next turn.
- At the end of each of your turns, 1 in 2(? 3? 4?) chance that the spell is back on cooldown.

# Item ideas
Most, if not all, item cards are one use and don't go back into a player's deck.
- Lucky clover: All probabilities are guaranteed during your turn.
- Scrolls: Cast the spell listed on the scroll

# Enemy types
- 

# What can a player do each turn?
Move: Move one tile over (unless affected by other spell/equipment item)
Attack: Either by casting a spell or using their melee weapon
Item: Use an item. Perhaps some items (such as scrolls) are in replacement for your attack.

# How does a player get knock out/die?
Ideas:
- When they pull a full hand of injury cards?? Smaller decks are more risky, as they are more susceptible to injuries
- 
