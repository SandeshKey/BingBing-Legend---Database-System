# BingBing-Legend---Database-System
The purpose of this project is to design a database system for the online mobile game 'BingBing Legend'. 


# BingBing-Legend---Database-System
The purpose of this project is to design a database system for the online mobile game 'BingBing Legend'. 

### BUSINESS RULES
1. A distinctive email address and username are required during player registration
2. At least one hero must be owned before any skin purchase
3. Only 5 (no more or less) active players are permitted in a team
4. Heroes must be selected uniquely within a team during the battle
5. Skins and heroes can only be procured with diamonds or battle points

<br>

## ENTITIES 
<br>

### ENTITY: PLAYER
Attributes | Description
-- | --
Player_ID | A distinctive ID is given to each player which distinctly identifies each information stored on that table of that particular player.
Player_name | To make the message dynamic, the player's real name is used while sending the player emails and updates.
Email | Email address of player.
Username | Player’s name in the game.
Global_level | The global level of players viewed publicly.
Diamond Collected | This holds the record for the collection of diamonds by players.
Online_Status | It is the boolean process where true indicates active or online and false indicates inactive or offline.
<br>

### ENTITY:HERO
Attributes | description
-- | --
Hero_ID | A unique primary key indicates each hero and automatically increments.
Hero_name | The names of hero’s like Fanny and Estes,  Clint, Cyclops, Rafaela, Dark Rose, etc.
Hero _Role | Role description of hero’s like Assassin, Fighter, etc.
Hero_Speciality | Specialty description of hero’s like Regen, Charge, etc.
Hero_Price | It is the integer which represents the price of hero’s in diamonds and battle points.
Hero_lvl | Specific played owned their current level of a specific hero.
<br>

### ENTITY:SKIN
Attributes | description
-- | --
Skin_ID | A unique primary key which indicates each skin and automatically increments.
Skin_name | A name of skin is usually one to describe it.
Skin_price | It is the integer which represents the price of skin’s in diamonds and battle points.
  |  

<br>

### ENTITY:GAME-MODE
Attributes | description
-- | --
Game_mode_ID | A unique primary key which indicates each available game mode and automatically increments.
Game_mode type | Classic, Brawl, or human vs AL mode are categorized as specific types of the mode.

<br>

### ENTITY:GAME
Attributes | description
-- | --
Game_ID | A unique primary key which indicates to each that has been played by players and automatically increments.
Game_date | It indicates the date variable in which the game shows the date that has been started.
battle _duration | It is an integer which represents the duration of game in which game can be change it into appropriate form if needed
Game_result | A foreign key which represents the team_ ID of the team that lost or won the game.
Arena | It is the cosmetics and environment of each game mode.

<br>

### ENTITY:TEAM
Attributes | description
-- | --
Team_ID | A unique primary key which indicates each team created and automatically increments.

<br>

### ENTITY:PERSONAL STATISTICS

Attributes | Description
-- | --
Player_ID | It is a foreign key which indicates the Player_ID that is located in the player in which the player has been linked to their statistics.
Most_used_hero | It is a foreign key which indicates the Hero_ID that is located in the hero entity in which the player used the hero most.
pervious_game_result | It is represented by using boolean in which false indicates the player lost the game and true indicates the player one last game they played.
Additional_result | Player description with their profiles.

<br>

### SIMPLIFIED ERD - WITHOUT CARDINALITY

![image](https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/8fa3cf05-2ffe-49f2-aa45-fb768640e2fa)

<br>

### DATABASE SCHEMA

![image](https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/9b5b33e9-ae00-4b2d-b309-7472b321b22a)

<br>

### DATABASE DIAGRAM

<img width="482" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/0306e27e-701b-4a97-95c7-7f06f89186c3">

<br>

## SQL-Data Definition Language SQL-DDL

#### DATABASE CREATION

<img width="214" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/0ea5e406-35d1-457b-a2ce-41c886184cda">

<br>

#### Player Table
<img width="401" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/c1840c53-312c-4a8b-b0f2-127ff001c7ac">

<br>

![image](https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/5ff23d3f-fe08-4a6d-8c6b-b553eed90b9b)

<br>

![image](https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/28c10521-e751-4e74-99e0-65cea3b4cace)

<br>

#### Hero Table
<img width="352" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/e393ef29-cca8-44e2-bfc7-1ed4a89dd166">

<br>

<img width="482" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/063b3da0-088f-4c67-8ddd-53ae0a1e6848">

<br>

<img width="482" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/40b0cc27-74ea-47ba-98df-16f791e62393">

<br>

#### Skin Table
<img width="363" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/cb71fa4e-1099-4387-96fa-a88a5bfb0c91">

<br>

<img width="482" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/bb6d13d1-a1a1-4d5a-ba7e-54ffbeae37e7">

<br>

#### Player-Hero Table
<img width="373" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/cd88f888-6174-4e64-b062-b544adbc34c1">

<br>

![image](https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/05b866f9-3636-450a-82d7-d94f128af665)

<br>

<img width="314" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/da155e97-c9c1-48c2-8718-c7587c041978">

<br>

#### Hero-Skin Table
<img width="355" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/326c0545-d586-432f-a215-081ba25883f9">

<br>

![image](https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/2a92debe-616f-49b3-80e0-d2662c4800fc)

<br>

#### Mode-Chosen Table
<img width="423" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/5dd4b720-cac5-4266-a819-2bc764830268">

<br>

![image](https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/6dfa8bf9-622c-4c87-bd44-419f4336709a)

<br>

#### Game-Mode Table
<img width="328" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/750203ea-7eda-4092-bb37-177963442d32">

<br>

<img width="331" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/bce39891-e085-492f-9b88-74c5833d7b55">

<br>

#### Team Table
<img width="412" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/3f49c885-dfe5-41c6-a9d1-8f4c320d8133">

<br>

<img width="482" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/cc926b75-b433-40e7-8187-4b1ce750ebab">

<br>

<img width="227" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/5bae4129-6e67-4c84-8324-27fc6c2a739a">

<br>

#### Team-Player Table
<img width="370" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/4c20b289-2479-4e64-a24a-6133e667ed08">

<br>

<img width="482" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/d8794fb4-7690-40e2-ab3b-6d1e1056081e">

<br>

#### Game Table
<img width="427" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/f57847c2-7caf-4fb8-bb89-65e8c7678973">

<br>

![image](https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/52017681-a38d-43a7-b3b7-20750139b864)

<br>

#### Personal Statistics Table
<img width="376" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/fb410794-b42d-495d-98e1-b993c78469b5">

<br>
<img width="482" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/bf2f8358-4486-433b-b8a9-e943b99f2e47">

<br>
<img width="440" alt="image" src="https://github.com/SandeshKey/BingBing-Legend---Database-System/assets/98152515/d37408d0-3114-4a6e-a715-077fa363f613">

<br>


## ### Project Information

[BingBing Database Docs.pdf](https://github.com/SandeshKey/BingBing-Legend---Database-System/files/13163444/BingBing.Database.Docs.pdf)



### Project Documentation

[BingBing Database Docs.pdf](https://github.com/SandeshKey/BingBing-Legend---Database-System/files/13163444/BingBing.Database.Docs.pdf)

<br>

### For Database File, and Keynote/PowerPoint Presentation, Visit **[My Portfolio Website](https://sandeshsubedi7.com.np/)**
