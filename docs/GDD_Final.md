# Game Design Document (Final)
Graveyard
Thomas Deolall

Game: https://legit-studios.itch.io/graveyard

## Finished Mechanics:
- [x] Hex-grid movement system
- [x] Enemies attack players (Add injury cards to their deck)
- [x] Players attack enemies
- [x] Basic card draw functionality
- [x] Enemies spawn from gravestones
- [ ] Items, spells. and gear logic
- [ ] Hand-off items between players
- [ ] Shop system

## Changelog:
Ignoring mechanics cut due to time constraints:
 - Added double attack cards
Tanks were very difficult to take down, and there were very few ways to damage an enemy more than once in a turn (certain spells, shuriken item). Additionally, it was extremely difficult to purchase higher rarity items within the game. Double attack cards would provide a reliable way to deal multiple attacks in a turn and double as a stronger currency within the slot of one card to provide more buying power during the shop phase.
- Added chance for no enemy to spawn on a tile
Having a constant 6 enemies every turn made the game very overwhelming very quickly. This mechanic added a small layer of balance and tweaking for the game, and made it feel more varied.
- Added ability to hand off cards between players
This change was added for several reasons. It added another layer of interaction between players in an area where the game was already lacking. Before this change, there were very few ways of assisting your allies directly. This allowed allowed some deck manipulation, the ability for one player to buy a item/equipment and then hand it off to another player in a future turn, and allowed players to "pool their money together" to try to make one big purchase.
- Added/tweaked many items to remove cards from your deck
Deck fixing is an important mechanic in all roguelike deckbuilders, and this game originally lacked it entirely. By implementing ways to thin your deck, it further supported the dynamic of smaller decks being able to draw more favorable cards faster, while larger decks were more resistant to injury cards.

# Below is my original treatment

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
- Archer: low HP, high damage. Special ability: extra range
- Tank: med HP, med damage. Special ability: can only take 1 damage per attack
- Healer: high HP, low damage. Special ability: at end of turn, heals all adjacent non-healer enemies

# What can a player do each turn?
Move: Move one tile over (unless affected by other spell/equipment item)
Attack: Either by casting a spell or using their melee weapon
Item: Use an item. Perhaps some items (such as scrolls) are in replacement for your attack.
Spell: Cast a spell. Spell is on cooldown, must roll its listed in number to get it off cooldown

# How does a player get knock out/die?
Ideas:
- When they pull a full hand of injury cards?? Smaller decks are more risky, as they are more susceptible to injuries
