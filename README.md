# Greedy Piggies Development Log 
Zoe Efstathiou 2423029


<hr style="height:3px; border:none; background-color:#ffb6c1;">

## Overview  

This document outlines my contributions to *Greedy Piggies*.

My work focuses on audio direction, archetype implementation, and workflow development, demonstrating both creative design and the application of industry-standard tools within a collaborative production environment.

## Contents

Audio
- [Audio Research](#audio-research-card-game-industry)  
- [Audio Production](#audio-production)  
- [Audio Implementation](#audio-implementation)  
- [Audio Settings Menu](#audio-settings-menu) 

Workflow + Pipeline Tools
- [Discord Ticket Bot](#discord-ticket-bot)  
- [Discord Sound Bot](#discord-sound-submission-bot)  
- [Audio Team Discord Server](#audio-team-discord-server)
- [Public Discord Server](#public-facing-discord-server)

Archetypes
- [Archetype and Voice Line Systems](#archetype-and-voice-line-systems)  
- [Narrator System](#narrator-voice-lines)  


For access to **Tools and Production** task repositories, see [RepositoryLinks.md](https://github.com/princessbleach/Zoe-GPs-Writeup/blob/main/RepositoryLinks.md)

<hr style="height:3px; border:none; background-color:#ffb6c1;">

## Audio Research: Card Game Industry  

During pre-production, audio direction was established collaboratively to ensure a consistent vision across the project.  

As a team, we shared **reference material and curated playlists**. This helped define the tone, pacing, and overall atmosphere of the game early in development. Originally, we steered towards the electronic music genre, centering a more sinister tone. Reference songs included: LuthorCorp - John Murphy, Bunsen Burner - CUTS. 

[Video Click Here: Superman Soundtrack Reference](https://youtu.be/d8ovNewe2As?si=on4Ltl-abxf0Pu_s)

![Superman](https://th.bing.com/th?&id=OVP.qzV6M8Oblqu_PLAh4itNUwHgFo&w=321&h=180&c=7&pid=2.1&rs=1)

[Video Click Here: Ex Machina Soundtrack Reference](https://youtu.be/4OmwjCX08l8?si=iKznTfV6hFSjGZPs)

![Bunsen](https://th.bing.com/th/id/OVP.hrRYkmqpwdCM7CaIQ6cZZgEsDh?w=243&h=136&c=7&rs=1&qlt=70&o=7&dpr=1.1&pid=2.1&rm=3)

(*Figure and . Initial Music References*.)


To further align the audio direction, musicians were asked to produce **small demo tracks** based on these references. This allowed for early feedback and iteration, ensuring that the final music would fit the intended style and game play context.  This process improved communication between designers and audio contributors, reduced inconsistencies, and established a clear foundation for implementation later in development.

 However, after further thought from the designers, we pivoted to a more lighthearted jazz vibe. We took inspiration based on games such as Liar’s Bar (Treehouse Games, 2023) and Poker Night at the Inventory (Telltale Games, 2010).  



[Video Click Here: Poker Night Reference](https://youtu.be/zbnhXCbP-jU?si=ZA4UwPBuxWlPC1G9) 

[![Poker Night Reference](https://i.ytimg.com/vi/zbnhXCbP-jU/hqdefault.jpg?sqp=-oaymwFBCNACELwBSFryq4qpAzMIARUAAIhCGAHYAQHiAQoIGBACGAY4AUAB8AEB-AH-CYAC0AWKAgwIABABGD4gZSgcMA8=&rs=AOn4CLCvsP2lz7OPgtoS8JNmnAeh3oU79g)]

(*Figure. Poker Night Music Reference.*)

In addition, we provided voice acting references to guide performance. For example, the narrator character was inspired by the “Old Money” style delivery found in Deadlock (Valve, 2024), helping to establish a clear tone and personality for voice performances.


[Video Click Here: Old Money Reference](https://youtu.be/jaaR9vMQGTg?si=jL76GBk_HUIwVV4i)


![ArchMother](https://th.bing.com/th/id/OIP.44HUgNawE30GiGhmNDvYrwHaFj?w=222&h=180&c=7&r=0&o=7&dpr=1.1&pid=1.7&rm=3)


(*Figure. Old Money Reference*)


An initial mistake in the audio pre-production process was casting voice actors based on generic portfolio auditions rather than using lines from the game itself. While some actors were well-suited to their roles, others did not match the intended tone or character, resulting in inefficient use of studio time. In future projects, I would ensure that all actors are auditioned using game-specific lines. 


Before recording foley sounds, we mainly drew inspiration from the UNO mobile game (Mattel163, 2019). These sounds were easily replicable and perfect for our style of card game. This reference also allowed us to spot any missing card sounds in our asset list, such as table card slides etc.


[Video Click Here: Card Sound Reference](https://youtu.be/z7AQ8vK9t64?si=akBoHI7FVHnE0Lxy)

![UNO](https://i.ytimg.com/an_webp/z7AQ8vK9t64/mqdefault_6s.webp?du=3000&sqp=CIzv_c4G&rs=AOn4CLCgX47SqmGbnxEDDdlLtMZFldwMTA)

(*Figure. Card Reference.*)

## Audio Production  

#### Voice Lines

We recorded all voice lines over two days in one of the uni studios. The process was highly collaborative, with two designers and two developers present. The designers printed out scripts, ensuring actors had the exact lines at hand. To help actors embody their characters, we displayed concept art on a screen, offering visual inspiration. The sessions ran smoothly, and we successfully captured all required voice content within our planned timeframe. I also out-sourced an actor online to play one of the older archetypes as there were no students suitable. I then edited voice lines in Reaper (Cockos Incorporated, 2024), ensuring they met standards needed in game and exported them with understandable naming conventions. 

<p align="center">
 <img src="https://github.com/princessbleach/Zoe-GPs-Writeup/blob/main/Images/Actor.jpeg?raw=true" width="20%">
 <img src="https://github.com/princessbleach/Zoe-GPs-Writeup/blob/main/Images/RecordingInspo.jpeg?raw=true" width="21%">

(*Figures . Voice Actors in Studio With Reference Material On Screen*)



#### Music, Foley/SFX

For music, foley, and SFX production, I managed a team of four music students, dividing them into groups and assigning each a specific sound category. To support organisation, I created a Trello (Atlassian, 2024) board where designers could upload asset lists. This allowed musicians to easily view, claim, and track required audio assets. Designers were also able to attach reference audio to each task, which helped communicate intent and improved consistency across submissions. At this stage of development, limited visual material was available. 

<p align="center">
<img src="https://raw.githubusercontent.com/princessbleach/Zoe-GPs-Writeup/refs/heads/main/Images/Trello.png" width="400">

(*Figure . Trello Board.*)

I attended the initial foley recording session to support the creation of core sounds. Real playing cards and additional props were used to produce authentic audio.  Reference material from UNO was used to guide the style of card interaction sounds.

<p align="center">
<img src="https://github.com/princessbleach/Zoe-GPs-Writeup/blob/main/Images/Foley.jpeg?raw=true" width="300">

(*Figure . Foley Artist Making Card Sounds.*)

All sound effects were submitted through a custom Discord bot I developed (discussed later), with the majority of assets completed by week 6. Music production required a longer iteration process, with multiple revisions to better align with the intended tone of the game. I worked with a designer on creating the menu track also.

## Audio Implementation 

For implementation, I chose to use **Sound Cues** rather than MetaSounds, as this allowed for a simpler and more efficient workflow while still achieving the required functionality. All voice lines, foley, and SFX were organised into Sound Cues, making use of **randomiser and modulator nodes** to introduce variation in playback and avoid repetition.  


<iframe src="https://blueprintue.com/render/dv6pn3a7/" scrolling="no" allowfullscreen></iframe>

(*Figure. Sound Cue Example.*)

To create the ambient soundscape for the main level, I developed a system using **target points placed within the environment** to define the origin of each sound. These were referenced within a Blueprint (BP_SoundAmbienceManager), where sounds were triggered at their locations using *Spawn Sound at Location*.  Each ambient sound (e.g. bar noise or chair movement) was linked to a specific target point and Sound Cue. To avoid predictable repetition, I used a **timer system with randomised intervals**, allowing sounds to play naturally over time rather than looping continuously.  Validation checks were also implemented to ensure that target points existed before attempting to play sounds, improving stability and preventing runtime errors.  

<iframe src="https://blueprintue.com/render/unh5na9y/" scrolling="no" allowfullscreen></iframe>

(*Figure. Sound Ambience Manager.*)

I also asked a designer to use Unreal's inbuilt subtitle system and write subtitles for each voice line sound wave. 

## Audio Settings Menu

I implemented an audio settings system to allow players to control different sound categories within the game. This was structured using **Sound Classes**, a **Sound Mix**, and a **Save Game system** to ensure settings persisted between sessions.  

Separate Sound Classes were created for key categories (e.g. music, SFX, dialogue, ambience), allowing each to be adjusted independently. A Sound Mix (*SCM_SoundSettings*) was used to apply real-time volume changes through Sound Class overrides.  A UI widget (*WBP_SoundOptions*) provided sliders for each category. These values were passed into Blueprint logic, where they were applied to the corresponding Sound Classes using volume multipliers.  

To persist settings, a **Save Game object (SG_SoundSettings)** was used. On game start, the system checks for an existing save file:
- If found, saved values are loaded and applied  
- If not, a new save is created with default values  

Whenever a slider is adjusted, the updated values are applied immediately and written back to the Save Game object.This system ensures consistent audio control for the player, while demonstrating the integration of UI, audio systems, and data persistence within Unreal Engine.

<iframe src="https://blueprintue.com/render/h7-aezl5/" scrolling="no" allowfullscreen></iframe>

(*Figure. Sound Settings*)

<hr style="height:3px; border:none; background-color:#ffb6c1;">

## Discord Ticket Bot  

I developed a Discord ticket bot to manage internal team requests and bug reporting using python,. 

The bot allows team members to submit structured tickets through a form-based system, ensuring that all requests included the necessary information (user, branch, description, optional image links). Submitted tickets were then sent to a private review channel, accessible only to designated roles, allowing for organised tracking and prioritisation.  

This system improved communication within the team by:
- Standardising how issues and requests were submitted  
- Reducing clutter in general chat channels  
- Allowing developers to review tasks in a focused environment  

The use of a structured ticketing system helped simulate a more professional production workflow, supporting better task management and accountability within the team.

I then collated the submitted ticket data (with consent) and conducted analysis to identify patterns in team workflow and task distribution. This included examining ticket distribution by category and by course, highlighting trends and areas of high activity. The findings were presented through graphs, allowing for clearer visual communication and more accessible interpretation of the data. Most tickets seemed to center around GitHub (GitHub, 2026) issues. 

(*For Assad, more on this, including source code, in respective repository's README.md*)

<p align="center">
<img src="https://raw.githubusercontent.com/princessbleach/Zoe-GPs-Writeup/refs/heads/main/Images/TicketDemo.gif" width="650">

(*Figure. Ticket Bot Demo.*)

## Discord Sound Submission Bot  

I created a custom Discord bot to handle the submission of audio assets from music students. This helps save myself time as I do not have to manually move assets into the project but it also aids musicians who do not know how to use version control. 

The bot allows users to:
- Submit audio files directly through Discord  
- Categorise submissions (e.g. SFX, foley, music)  
- Ensure files were delivered in the correct format  

Submitted files were automatically organised into the project directory, allowing for faster integration into Unreal Engine and reducing manual file handling.  


(*For Assad, more on this, including source code, in respective repository's README.md*)


<p align="center">
<img src="https://raw.githubusercontent.com/princessbleach/Zoe-GPs-Writeup/refs/heads/main/Images/SoundUploadDemonstration.gif" width="650">

(*Figure. Audio Upload Bot Demo.*)

## Audio Team Discord Server  

Alongside this, I developed a Discord server to manage communication with myself, designers and musicians.  

The server provided:
- Clear submission guidelines and instructions  
- Dedicated channels for different types of contributors  
- A structured environment for feedback and updates  
  
.

<p align="center">
<img src="https://github.com/princessbleach/Zoe-GPs-Writeup/blob/main/Images/AudioTeamServer.png?raw=true" width="400">

(*Figure. Audio Standards in Audio Team Server.*)

## Public Facing Discord Server

In addition to internal tools, I created a public-facing Discord server to support player engagement and external communication. This provided a central space for players to interact with the project, stay informed, and engage with the development process.  

The server features:

- Role selection for region and pronouns using pre-existing bot
- Optional roles for receiving social media updates  
- Clearly defined rules and a dedicated welcome and information area  
- The use of webhooks to deliver announcements and updates efficiently
  

 Webhooks are automated messages sent between applications when a specific event occurs, enabling real-time communication without manual input (GitHub, 2026). I chose to use Webhooks so that I wouldn't have to send messages from my own account. This solves any problems caused if I were to leave the server or detach from the project in the future.


<p align="center">
 <img src="https://github.com/princessbleach/Zoe-GPs-Writeup/blob/main/Images/PublicServerRoles.png?raw=true" width="25%">
 <img src="https://github.com/princessbleach/Zoe-GPs-Writeup/blob/main/Images/PublicServerRules.png?raw=true" width="35%">
 <img src="https://github.com/princessbleach/Zoe-GPs-Writeup/blob/main/Images/PublicServerWelcome.png?raw=true" width="35%">

 (*Figure . Webhook Messages in Public Server.*)

<hr style="height:3px; border:none; background-color:#ffb6c1;">

## Archetype and Voice Line Systems  

I developed an archetype system to define player identity through meshes, animations, and voice lines, using a data-driven approach to ensure scalability and consistency across the project.  

Each archetype was implemented as a **Data Asset**, containing references to skeletal meshes, animation data, and structured voice line sets. This allowed archetypes to be applied dynamically at runtime without modifying Blueprint logic. Voice lines were organised using an **enum (VoiceLineCategory)** and a **struct (VoiceLineEntry)**. The enum defined categories such as win, lose, chuckle, etc. whilst the struct stored associated Sound Cues. These were stored within each archetype’s Data Asset.

<iframe src="https://blueprintue.com/render/kpey9wm3/" scrolling="no" allowfullscreen></iframe>

(*Figure. Lose Reaction Function Example in BP_ArchetypeComponent.*)

This type of system allows for designers to easily swap in animations, meshes etc without having to write Blueprints. They can simply drag into the data assets.

A function-based system within an archetype component was used to retrieve voice lines by category. This function:
- Takes a VoiceLineCategory as input  
- Searches the archetype’s data for a matching entry  
- Returns the appropriate Sound Cue for playback  

To support multiplayer contexts, voice lines were implemented using three playback types:
- **Local (2D)**: Played only for the owning player, used for UI-related or feedback-specific lines e.g shop opening 
- **Global**: Played for all players regardless of position, used for key events such as narrator announcements  
- **Spatial (3D)**: Played at the character’s location using attenuation, allowing other players to hear voice lines relative to distance  

This distinction ensured that audio remained clear within a multiplayer environment. 

<iframe src="https://blueprintue.com/render/yz0s_839/" scrolling="no" allowfullscreen></iframe>

(*Figure. BP_ArchetypeComponent Event Graph.*)

Cooldowns were implemented to prevent voice lines from being triggered repeatedly in quick succession. Each category was given a delay before it could be played again. These cooldowns could be adjusted per line in the Data Asset. This reduced audio overlap and ensured voice lines remained clear and impactful, particularly in multiplayer.


An **Apply Archetype** function was used to initialise each player’s setup, assigning meshes, animation settings, and voice data. Animation montages were triggered alongside voice lines to maintain consistency between audio and visual feedback.  

<iframe src="https://blueprintue.com/render/7ulrrp07/" scrolling="no" allowfullscreen></iframe>

(*Figure. ApplyArchetype Function.*)

##  Narrator Voice Lines

The narrator system was controlled through a dedicated Blueprint (*BP_NarratorManager*), which handled retrieval and playback of narrator voice lines. These lines are sometimes specific to the player archetype: e.g "Nepo-piggy wins the showdown!". Voice line data was stored in structured arrays within a Data Asset, using structs to define each entry. The system used a struct (*ST_GlobalNarratorLine*) containing a global event type and associated Sound Cue.  

The **GetGlobalNarratorLine** function iterates through this array using a *For Each Loop*, comparing the input event type against each struct entry. When a match is found, the corresponding Sound Cue is returned. For archetype-specific narrator lines, the **GetNarratorLine** function performs a similar process, but matches against both the archetype tag and outcome type. A conditional check ensures both values match before returning the correct voice line.  

<iframe src="https://blueprintue.com/render/kyp0e-d_/" scrolling="no" allowfullscreen></iframe>

<iframe src="https://blueprintue.com/render/mpp9bw36/" scrolling="no" allowfullscreen></iframe>

(*Figures. GetGlobalNarratorLine and GetNarratorLine Functions.*)

Playback is handled through replicated multicast events:
- **MC_PlayNarratorLine** is used for archetype-specific outcomes  
- **MC_PlayGlobalNarratorLine** is used for global events  

These events are executed on all clients, ensuring that narrator lines are synchronised across the network. Before playback, an **IsValid check** is used to ensure the retrieved Sound Cue exists. The audio is then played using *Spawn Sound 2D*, ensuring narrator lines are heard clearly by all players regardless of position.  

This system separates data retrieval from playback, using structured data and networked events to create a reliable and scalable global audio system.

## Integration Challenges



An issue arose when integrating the archetype system with the character selection flow. Initially, archetypes were being initialised at the start of the level, before players had made their selection. This resulted in incorrect or default archetypes being applied.  

To resolve this, archetype initialisation was moved to occur only after a player had selected and confirmed their choice. This ensured that the correct Data Asset was applied at the appropriate time.  

Further challenges occurred in multiplayer, where archetype data was not consistently shared between clients. This was resolved by storing the selected archetype in **Player State** and using replication to ensure all players received the correct data. An OnRep function was then used to reapply the archetype on each client when updated.  

This process highlighted the importance of timing and data ownership in multiplayer systems, particularly when integrating UI-driven selection with runtime gameplay logic.


<hr style="height:3px; border:none; background-color:#ffb6c1;">

## Bibliography

**AI DECLARATION**

AI assistance (ChatGPT, OpenAI) was used to support structuring and refinement of this document. 


**GAMES**

Treehouse Games (2023) *Liar’s Bar*.  

Telltale Games (2010) *Poker Night at the Inventory*.  

Valve (2024) *Deadlock*.

Mattel163 (2019) *UNO! Mobile*.

**SOFTWARE**

Cockos Incorporated (2024) *REAPER*. Available at: https://www.reaper.fm/ 

Atlassian (2024) *Trello*. Available at: https://trello.com/ 

GitHub (2026) *GitHub*. Available at: https://github.com/ 

Epic Games (2026) *Unreal Engine*. Available at: https://www.unrealengine.com/


**OTHER**

GitHub (2026) *About webhooks*. Available at: https://docs.github.com/en/webhooks.
