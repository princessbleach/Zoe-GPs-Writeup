# Greedy Piggies Development Log 
Zoe Efstathiou 2423029


<hr style="height:3px; border:none; background-color:#ffb6c1;">

## Overview  

This document outlines my contributions to *Greedy Piggies*.

My work focuses on audio direction, technical implementation, and workflow development, demonstrating both creative design and the application of industry-standard tools within a collaborative production environment.


## My Role  

I worked as Audio Lead, responsible for both the creative direction and technical implementation of sound systems within the project.  

This included:
- Designing the overall audio style and player feedback systems  
- Organising and managing voice actors and musicians  
- Editing and preparing audio assets for integration  
- Implementing voice lines, UI audio, and ambient systems in Unreal Engine  
- Ensuring functionality across both single-player and multiplayer contexts  

Alongside this, I developed workflow tools (including Discord-based systems) and contributed to gameplay systems such as archetypes and voice-driven interactions.



## Structure  

This log is divided into three sections:

1. Audio Direction & Implementation  
2. Archetypes, Voice Lines & Animation Systems  
3. Workflow & Pipeline Tools 







<hr style="height:3px; border:none; background-color:#ffb6c1;">

## Audio Research: Card Game Industry  

During pre-production, audio direction was established collaboratively to ensure a consistent vision across the project.  

As a team, we shared **reference material and curated playlists** based on games such as Liar’s Bar (Treehouse Games, 2023) and Poker Night at the Inventory (Telltale Games, 2010). This helped define the tone, pacing, and overall atmosphere of the game early in development.  

To further align the audio direction, musicians were asked to produce **small demo tracks** based on these references. This allowed for early feedback and iteration, ensuring that the final music would fit the intended style and gameplay context.  This process improved communication between designers and audio contributors, reduced inconsistencies, and established a clear foundation for implementation later in development.

An initial mistake in the audio pre-production process was casting voice actors based on generic portfolio auditions rather than using lines from the game itself. While some actors were well-suited to their roles, others did not match the intended tone or character, resulting in inefficient use of studio time. In future projects, I would ensure that all actors are auditioned using game-specific lines. 



## Audio Production  

#### Voice Lines

We recorded all voice lines over two days in our university studio. The process was highly collaborative, with two designers and two developers present. The designers printed out scripts, ensuring actors had the exact lines at hand. To help actors embody their characters, we displayed concept art on a screen, offering visual inspiration. The sessions ran smoothly, and we successfully captured all required voice content within our planned timeframe. I also outsourced an actor online to play one of the older archetypes as there were no students suitable. I then edited voice lines in Reaper (Cockos Incorporated, 2024), ensuring they met standards needed in game and exported them with understandable naming conventions. 

#### Music, Foley/SFX

For music, foley, and SFX production, I managed a team of four music students, dividing them into groups and assigning each a specific sound category. To support organisation, I created a Trello (Atlassian, 2024) board where designers could upload asset lists. This allowed musicians to easily view, claim, and track required audio assets. Designers were also able to attach reference audio to each task, which helped communicate intent and improved consistency across submissions. At this stage of development, limited visual material was available. 


All sound effects were submitted through a custom Discord bot I developed (discussed later), with the majority of assets completed by week 6. Music production required a longer iteration process, with multiple revisions to better align with the intended tone of the game. I worked with a designer on creating the menu track also.

## Audio Implementation 

For implementation, I chose to use **Sound Cues** rather than MetaSounds, as this allowed for a simpler and more efficient workflow while still achieving the required functionality. All voice lines, foley, and SFX were organised into Sound Cues, making use of **randomiser and modulator nodes** to introduce variation in playback and avoid repetition.  

(*Figure. Sound Cue Example.*)

<iframe src="https://blueprintue.com/render/dv6pn3a7/" scrolling="no" allowfullscreen></iframe>

To create the ambient soundscape for the main level, I developed a system using **target points placed within the environment** to define the origin of each sound. These were referenced within a Blueprint (BP_SoundAmbienceManager), where sounds were triggered at their locations using *Spawn Sound at Location*.  Each ambient sound (e.g. bar noise or chair movement) was linked to a specific target point and Sound Cue. To avoid predictable repetition, I used a **timer system with randomised intervals**, allowing sounds to play naturally over time rather than looping continuously.  Validation checks were also implemented to ensure that target points existed before attempting to play sounds, improving stability and preventing runtime errors.  

<iframe src="https://blueprintue.com/render/unh5na9y/" scrolling="no" allowfullscreen></iframe>

(*Figure. Sound Ambience Manager.*)


#### Audio Settings Menu


blah balh

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

(*For Assad, more on this, in respective repository's README.md*)

<img src="https://raw.githubusercontent.com/princessbleach/Zoe-GPs-Writeup/refs/heads/main/TicketDemo.gif?token=GHSAT0AAAAAADZIUT7HDLVGGVSMVVSMFSRM2OL7ADQ" width="650">

(*Figure. Ticket Bot Demo.*)

## Discord Sound Submission Bot  

I created a custom Discord bot to handle the submission of audio assets from music students. This helps save myself time as I do not have to manually move assets into the project but it also aids musicians who do not know how to use version control. 

The bot allows users to:
- Submit audio files directly through Discord  
- Categorise submissions (e.g. SFX, foley, music)  
- Ensure files were delivered in the correct format  

Submitted files were automatically organised into the project directory, allowing for faster integration into Unreal Engine and reducing manual file handling.  


(*For Assad, more on this in respective repository's README.md*)

<img src="https://raw.githubusercontent.com/princessbleach/Zoe-GPs-Writeup/refs/heads/main/SoundUploadDemonstration.gif?token=GHSAT0AAAAAADZIUT7HEH7DNA2Z65YYFO3I2OL7BIQ" width="650">

(*Figure. Audio Upload Bot Demo.*)

## Audio Team Discord Server  

Alongside this, I developed a Discord server to manage communication with myself, designers and musicians.  

The server provided:
- Clear submission guidelines and instructions  
- Dedicated channels for different types of contributors  
- A structured environment for feedback and updates  
  
.

<img src="https://raw.githubusercontent.com/princessbleach/Zoe-GPs-Writeup/refs/heads/main/AudioTeamServer.png?token=GHSAT0AAAAAADZIUT7HNHXZQUTJO7CWGNXE2OL6RSQ" width="500">

(*Figure. Audio Standards in Audio Team Server.*)

## Public Facing Discord Server

In addition to internal tools, I created a public-facing Discord server to support player engagement and external communication.  

The server features:

- Role selection for region and pronouns using pre-existing bot
- Optional roles for receiving social media updates  
- Clearly defined rules and a dedicated welcome and information area  
- The use of webhooks to deliver announcements and updates efficiently  
  

This provided a central space for players to interact with the project, stay informed, and engage with the development process.  
<p align="center">
 <img src="https://raw.githubusercontent.com/princessbleach/Zoe-GPs-Writeup/refs/heads/main/PublicServerRoles.png?token=GHSAT0AAAAAADZIUT7G2U2GW2VUO3XMRM2O2OL6JPA" width="25%">
 <img src="https://raw.githubusercontent.com/princessbleach/Zoe-GPs-Writeup/refs/heads/main/PublicServerRules.png?token=GHSAT0AAAAAADZIUT7H2ZAX75VJORHJLCIE2OL6J2Q" width="35%">
 <img src="https://raw.githubusercontent.com/princessbleach/Zoe-GPs-Writeup/refs/heads/main/PublicServerWelcome.png?token=GHSAT0AAAAAADZIUT7G77K55KU33ES2RTP42OL6NWA" width="35%">

 (*Figure . Webhook Messages in Public Server.*)

<hr style="height:3px; border:none; background-color:#ffb6c1;">








## Bibliography

**GAMES**

Treehouse Games (2023) *Liar’s Bar*.  

Telltale Games (2010) *Poker Night at the Inventory*.  


**SOFTWARE**

Cockos Incorporated (2024) *REAPER*. Available at: https://www.reaper.fm/ 

Atlassian (2024) *Trello*. Available at: https://trello.com/ 

GitHub (2026) *GitHub*. Available at: https://github.com/ 

**AI**

AI assistance (ChatGPT, OpenAI) was used to support structuring and refinement of this document. All technical decisions are my own.
