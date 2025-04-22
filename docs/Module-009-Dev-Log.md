<!-- Markdown Docs: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax -->
## Name: Thomas Deolall
### Module: 9

<!-- Repeat the below as needed-->
### Date: [04/21/2025]

#### Goals for this Module
<!-- Example Template (include the brackets to make a checklist, fill them in as appropriate
- [ ] Goal 1
- [ ] Goal 2
- [ ] Goal 3
-->
- [ ] Grid movement **(IN PROGRESS)**
- [ ] Card deck logic (shuffling, draw starting hand, etc.)
- [ ] Card functionality
- [ ] Enemy logic (Spawning, attacking, getting hit)

#### Progress
- **What I accomplished**:
  - Summarize completed tasks or progress made.
  - I worked on the basis of movement for the players in my game, though it's not fully functional just yet.
  
- **Challenges faced**:
  - Describe blockers, bugs, or issues encountered.
  - N/A

- **Solutions**:
  - Detail how you addressed challenges or your thought process.
   N/A

#### Learnings
- Key insights, techniques, or concepts explored.
- The Red Blob Games article made implementing the movement much easier, as it provided functions and equations for essentially any sort of calculation I'd need for the grid. It was also quite easy to expand upon to record things specific to my game.

#### Free Thinking
- Brainstorm or reflect on design ideas, architecture patterns, or potential improvements.
- I'm planning to have each player use a regular controller to control rather than the suggested pass-and-play solution in class. I feel that it'll vastly improve my game, as it isn't turn-based between players, and the ability to make choices inbetween your teammates' choices freely is an essential part of my game. I think a good visual design choice is that, whenever a player is hovered over a grid, each player's cursor points to a different vertex of the hexagon. For example, player 1 could point to the top vertex, player 2 can point to the (bottom) right vertex, and player 3 can point to the (bottom) left vertex. This way, multiple players can easily hover over the same hexagon without having to code other visual features for overlap.

#### Next Steps
- Tasks or experiments to focus on during the next session.
- I'd like to finish up my movement system, then look into outlining an entity-component system for the players and enemies on the board.
