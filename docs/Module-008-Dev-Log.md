<!-- Markdown Docs: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax -->
## Name: Thomas Deolall
### Module: 8

<!-- Repeat the below as needed-->
### Date: [04/14/2025]

#### Goals for this Module
<!-- Example Template (include the brackets to make a checklist, fill them in as appropriate
- [ ] Goal 1
- [ ] Goal 2
- [ ] Goal 3
-->

  [x] Create Godot project
  [ ] Grid movement
  [ ] Card deck logic (shuffling, draw starting hand, etc.)
  [ ] Card functionality
  [ ] Enemy logic (Spawning, attacking, getting hit)
  

#### Progress
- **What I accomplished**:
  - Summarize completed tasks or progress made.
  - I made the Godot project and designed the board game in Godot.
  - I did a lot more reading into the "Red Blob Games" article on hex-based grids.
- **Challenges faced**:
  - Describe blockers, bugs, or issues encountered.
  -  N/A
- **Solutions**:
  - Detail how you addressed challenges or your thought process.
  - N/A

#### Learnings
- Key insights, techniques, or concepts explored.
- The logic for hex-based grids isn't as daunting of a task as I thought. The axial coordinate system does a very good job representing the grid and is used to easily calculate functions like neighboring tiles, distances, etc.

#### Free Thinking
- Brainstorm or reflect on design ideas, architecture patterns, or potential improvements.
- The Red Blob Games article has quite a lot of different functions and coordinate systems detailed, a lot of which I won't be needing for my game. I think I'm going to work entirely with axial/cubical coordinates and primarily use the getting neighbors function, and utilize a little bit of the pathfinding portion for checking if a hex is reachable by a player.
<!--Your entry here or N/A if not applicable for this entry-->
<!--

- Example prompts:
  - "What if the player interactions were asynchronous instead of real-time?"
  - "How could ECS improve performance in this system?"
  - "Does my current design support scalability? How can it improve?"
  
-->

#### Next Steps
- Tasks or experiments to focus on during the next session.
- As recommended by the lecture slides, I want to have an outline of my grid-based movement done first before touching any other mechanics of the game.
