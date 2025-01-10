#### Databases

teams
- team_id
  - SERIAL
  - PRIMARY KEY
- name
  - VARCHAR 20
  - UNIQUE
  - NOT NULL

games
- game_id
  - SERIAL
  - PRIMARY KEY
- year
  - INT
  - NOT NULL
- round
  - VARCHAR 20
  - NOT NULL
- winner_id
  - INT
  - NOT NULL
  - FOREIGN KEY - teams.team_id
- opponent_id
  - INT
  - NOT NULL
  - FOREIGN KEY - teams.team_id
- winner_goals
  - INT
  - NOT NULL
- opponent_goals
  - INT
  - NOT NULL
