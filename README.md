# Option/Settings System - Roblox Portfolio Project







##  Overview

A complete, dynamic daily quest system for Roblox games featuring real-time progress tracking, smooth UI animations, and persistent player data across sessions.






## Features


- Daily Quest Rotation - Automatically refreshes 2 random quests every 24 hours

- Real-Time Progress Tracking - Live updates for walk distance, jump count, stand time, and play duration

- Smooth Progress Bars - Tween-based animated bars that visually represent completion percentage

- Quest Completion Rewards - Automatic cash rewards upon quest completion

- Persistent Progress - Player quest data saves between sessions via DataStore

- 24-Hour Cooldown - Visual countdown timer for next quest refresh

- Clean UI Feedback - Completed quests display "COMPLETED!" overlay with visual confirmation

- Hover & Click Effects - Consistent button animations with sound feedback across all interactive elements



## Architecture



- **Client-Side**: LocalScripts handling UI updates, progress bars, and real-time quest tracking


- **Server-Side**: Scripts managing quest logic, data persistence, and security validation



- **Networking**: RemoteEvents for secure client-server quest claim communication



- **Data Persistence**: DataStore integration for saving player cash and quest progress







## Installation



1\. Clone this repository.



2\. Open the `.rbxl` file in Roblox Studio (demo file available in Releases).



3\. Import the DailyQuestGui "ScreenGui" into StarterGui.



4\. Configure quest pool and daily quest count in the server script



5\. Run the game and access settings via the DailyQuestsButton.





## Project Structure

Workspace\\StarterGui/

DailyQuestsGui/

├── DailyQuestsClient (LocalScript)    # UI updates and progress tracking

├── OpenQuestsButton (ImageButton)     # Toggles quest menu visibility

├── QuestsFrame/                      # Main quest container

│   ├── RefreshTime (TextLabel)      # 24h countdown timer

│   ├── QuestsScroller/             # Scrollable quest list

│   │   └── QuestLabel (Frame)      # Template for individual quest displays

│   └── [Dynamic Quest Labels]      # Generated quest entries

└── Sounds/
    ├── ClickSound (Sound)          # Button click feedback
    └── HoverSound (Sound)          # Button hover feedback

ServerScriptService/
└── QuestSystems/
    └── DailyQuestsServer (Script)  # Server logic and DataStore management



## Demo



[[Demo Game link for demonstrating the system](https://www.roblox.com/games/132226618571993/Project-Portfolio)]







## Tech Stack







**Platform & Language**



- Roblox Studio



- Lua 5.1 (Roblox-flavored)







**Core Services**



- TweenService (Smooth UI animations)



- DataStoreService (Player progress persistence)



- PlayersService (Character tracking)



- RunService (Real-time progress updates)







**UI/UX Features**



- Responsive hover scaling (1.01x)



- Tactile click feedback (2px depression)



- Smooth slide toggles with color transitions



- Proper ZIndex layering



- Screen-relative positioning





**Additional Expertise**



- Client-Server security models



- Optimized DataStore usage patterns



- Efficient networking strategies







## License



This portfolio project is licensed under the MIT License.







**Note:** This is a demonstration project for portfolio purposes. The code is provided to showcase development skills.







# Author



[I03I] - Portfolio Projects



- Demo Video: \[Coming Soon]

- Portfolio Contact: trafonbusiness.com

