<h1 align="middle">SCP: Containment Failure</h1>

<p align="middle">
  <a href="https://www.roblox.com/games/16752950836/Mailbox-Misery">
    <img src="https://img.shields.io/badge/Play_on_Roblox-red?style=for-the-badge&logo=roblox&logoColor=white">
  </a>
</p>
<br>
<br>

**0 visits — Advanced horror game**  
**Role:** Main scripting developer

<p align="left">
SCP: Containment Failure was planned to be a SCP: Containment Breach remake on Roblox, featuring procedural map generation and interactive SCPs (most of which are NPCs). The game has been postponed multiple times, but several advanced scripts and systems have already been developed in preparation for its release.
</p>

---

<h2 align="left">Work-showcase</h2>

https://github.com/user-attachments/assets/bd31d3bb-942f-4f1a-8287-14ee5bed9bde

> The video showcases a procedurally generated map layout with fully random room generation. The system automatically checks for invalid placements and includes required sections for rooms that must appear in every layout.

<p align="left">
  <a href="https://pastebin.com/0H51pu9U" target="_blank">
    <img src="https://img.shields.io/badge/Luau-View_Code_Snippet-royalblue?style=for-the-badge&logo=luau&logoColor=white">
  </a>
</p>
<br>

https://github.com/user-attachments/assets/9727c308-5c2a-4692-8d46-2e210ff62e8f


> The video showcases one of the NPCs: SCP-096. According to the lore, SCP-096 is a tall, pale humanoid that becomes extremely aggressive toward anyone who sees its face. In the demonstration, you can see the NPC calculating a dynamic path to the player, proving that even monsters appreciate efficient routing.
> NOTE: Some scripts and UIs are outdated and acted as placeholders, for example the proximity prompt or the blinking UI on the left. These were just placeholders during the early phase of development. The AI itself has not changed in any noticeable way since then.

<p align="left">
  <a href="https://pastebin.com/GT5Qd0WC" target="_blank">
    <img src="https://img.shields.io/badge/Luau-View_Code_Snippet-royalblue?style=for-the-badge&logo=luau&logoColor=white">
  </a>
</p>

---

<h2 align="left">Biggest dificulty & What I learned</h2>
<p align="left">
The hardest part of this project was making the procedural map generation system. I had never done anything like this before, so I had to figure it out from scratch.

At first, I tried to make it work like the game DOORS, where rooms generate in a straight line. But I quickly realized that wouldn't work for what I needed. I wanted branching paths and multiple routes, not just one long hallway.

After scrapping that idea, I looked into how SCP: Containment Breach made its levels. I couldn't find much about how their code worked, but I found an online map generator that showed how their rooms were laid out. I spent a lot of time generating different maps on that site, looking for patterns and trying to understand how it all worked.

After studying it, I noticed the maps followed a pattern that went horizontal, then vertical, then horizontal again. I came up with my own approach based on what I saw:
The system starts by creating a horizontal row of rooms across the level. Then it picks a few random rooms from that row and creates vertical connections (like stairs or elevators) going up to the next floor. This pattern keeps repeating for each floor, making a snake-like path through the whole level.
This creates natural branching paths while keeping everything connected. I also added some extra features: if one side generates short, the other side generates longer to keep things balanced. Room counts use weighted random chances so there's variety but nothing too extreme. The system also uses raycasting to check that doors line up properly between rooms before placing them.
This went from being something I had no idea how to do, to one of the coolest systems I've built. It taught me a lot about procedural generation and working with grids and coordinates.

Additionally, I created a few NPCs for the game that needed to open doors, and I wanted Roblox’s PathfindingService to be able to ignore the doors and path through them. This experience helped me learn how pathfinding links and modifiers work.
</p>



<br>
<br>
<p align="middle">
  <a href="https://github.com/QluxpEL#-scp-containment-failure">
    <img src="https://img.shields.io/badge/GitHub-return_to_main_page-181717?style=for-the-badge&logo=github">
  </a>
</p>
