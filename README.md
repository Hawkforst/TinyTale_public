# TinyTale public repository
<img width="1408" height="768" alt="obrazek" src="https://github.com/user-attachments/assets/a3f8b598-a5b2-4fc1-bf81-ab73f4cb6899" />

The purpose of this repository is to be a public overview of the TinyTale project. We're safeguarding our code in a private repository so this is mainly to outline and explain the high-level direction and state of the project.
# What is it?
TinyTale is an AI-powered story-based Dungeon & Dragons style game with handcrafted stories, play alone or with others, only using your voice and listening to the narrator.

## What customer problem do we solve?
People love Dungeon & Dragons style storytelling experience (its popularity boosted by media like Stranger Things,..) and people love playing around with genAI. 
But you need friends to play with, someone to design the story for the group, and time to come together, which can be overwhelming.

There's also a huge market for games where you don't need to watch the screen all the time. People can play while doing garden work, when their eyes are tired or even with their grandparents. The only interface is the narrator's (generated) voice and user's own voice (or just write the text as an optional feature)
## How do we solve this problem?
We've designed and now are developing a deterministic framework (with Dungeon & Dragons style rolls). There's an underlying world with set rules and scenes that the player interacts with. On top of this backbone, we're using an AI powered narrator (an LLM) with Text to Speech capability. This combination of deterministic rules and LLM narration freedom gives the user both the feeling of freedom and immersion (LLM narrator reacts to whatever the player comes up with) but prevents AI slop (LLM narrator is constantly reminded of the world's contraint in prompts, major decision and events are code-based, not LLM based)

This creates an immersive D&D style experience that can be played solo, with your friends, or with your grandmother (the very natural flow of the game makes it easier to bridge even big age gaps).

(Note: For now our experiments run on a laptop but we're aiming to eventually move the game on smartphones (by either moving the computationally heavy part on a cloud or through optimization, e.g. TTS model distillation). )

# How it works?
Our moto is "Complexity from simple concepts". This is a pattern that dominates many engineering fields. Neural network, for example, are very simple concepts if you look into the lowest level, yet these simple parts interacting together create complex behavior. In a similar way, we are designing TinyTale to use several simple concepts which interact together (and with the player, via the narrator) to create an immersive experience that gives off the impression of a real world with its own rules, characters and struggles (that the player can interact with).
<!-- <img width="1236" height="1148" alt="obrazek" src="https://github.com/user-attachments/assets/0a9ced64-7dbc-4b43-b75f-2aa4a5ec0cf1" /> -->
<img width="1024" height="730" alt="01" src="https://github.com/user-attachments/assets/6d8a1f99-69ab-4d5f-8177-4ad1e8a82fb7" />

# Example of story flow visualization
The story is largely linear, for now. This is to ensure we get all the aspects of the technical implementation right. As the framework matures and becomes consistent, coherent and robust, we will move forward with much more non-linear stories, where multiple branches intertwine together. We're, however, ultimately aiming for complex stories with meaningful choices.
<img width="1712" height="1023" alt="obrazek" src="https://github.com/user-attachments/assets/bd65c0b7-2b4d-411a-a135-489fe2eb9a2d" />

# High level diagram of TinyTale logic
<img width="1347" height="959" alt="image" src="https://github.com/user-attachments/assets/58d66417-b4d7-4bfb-8324-566a371a49d7" />

# TinyTale rewards creative solutions
<img width="1024" height="730" alt="03" src="https://github.com/user-attachments/assets/6931b9dd-f014-426e-920a-0fbeca3f1a1e" />

# Example gameplay
<div align="center">
  <video src="https://github.com/user-attachments/assets/3c5652dd-7b12-4763-bc4c-709881a94171" 
         alt='video'
         width="80%" 
         autoplay 
         muted 
         loop 
         playsinline>
  </video>
</div>
Our game supports Text-to-Speech, meaning the player(s) can play the game without looking at the screen.
<div align="center">
  <video src="https://github.com/user-attachments/assets/6b7d209d-a20f-440b-bb3e-b93bffae6817" 
         alt='video'
         width="80%" 
         autoplay 
         muted 
         loop 
         playsinline>
  </video>
</div>









