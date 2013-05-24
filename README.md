#Foosball app
###Insert amazing tagline!

Being the nerds that we are, it was time to have a digital scoreboard to accompany our physical [table football](http://en.wikipedia.org/wiki/Table_football).

##Requirements
###Overall prerequisites
####Logistics
- Foosball table
- 4 players
- 2 teams
- 1..4 mobile devices
- 2 player positions per team (attacking & defending)
####Envisioned architecture
- 1 Gamelist (a.k.a. server)
- 0..* Lobbies (a.k.a. channels)
- 0..* Matches (a.k.a. "Lobby" being played)
###Version 1.0 "Base API with consonle output to mimic app":
####Prerequisites/Scope
- Static list of players i.e. no login feature
- Make it work for 2 mobile devices first (no syncing yet)
- Ruleset: first team to 11 goals. Should win with a margin of +2 goals. (i.e. 12 - 14 could be a valid score)

####Requirements
- There should be a Gamelist where matches are shown. Perhaps with an option to only show available matches
- If you're in the Gamelist, you should be able to create a Lobby. You will become the Host.
- If you're in the Gamelist and you see an available Lobby, you can join this Lobby.
- In a Lobby you can switch Team and Position
- When a Lobby is full, the Host can start the Match.
- When a Match is started, Players can keep score for themselves.
- When the "Ruleset" is met, the Match is over and the Scores will be given.

##Roadmap
- One server with public API
- Support 1 or multiple (4 max) mobile devices (keep them in sync too)
- Tournaments
- Statistics (per tournament, per team, per player)
- Graphics
