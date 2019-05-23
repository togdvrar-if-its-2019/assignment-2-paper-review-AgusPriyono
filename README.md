# assignment-2-paper-review-AgusPriyono

Player-Adaptive Spelunky Level Generation

- David Stammer (Hochschule Mannheim) david.stammer@googlemail.com 
- Tobias G¨unther (Cooperative State University Baden-Wuertemberg) tobias.guenther@dhbw-mannheim.de
- Mike Preuss (WWU M¨unster, Germany) mike.preuss@wi.uni-muenster.de

## STRUCTURE
- ABSTRACT
- INTRODUCTION
- RELATED PCG AND DDA WORKS
- SPELUNKY
- PLAYER SURVEY CONCERNING DDA
- DIFFICULTY ESTIMATION AND PLAYING STYLE In
- CONTROLLED LEVEL GENERATION
- USER STUDY 
- CONCLUSION
- REFERENCES


## Abstract
- PCG has been applied to many games today, so it helps level designers to be creative
- Generate level by adjusting the level of difficulty by applying the rule for its adaptive
- The approach is Experience-Driven PCG approach, where generating from the level depends on the experience of the user
- Based on surveys, most people appreciate adaptation, the more important thing is an easy game to play at any time


## Intro
- One of the many studies on AI in games, relates to almost all topics about AI in games, and is increasingly being applied to commercial games [1]
- Spelunky games currently have implemented auto generation, but it does not depend on player performance, and can be frustrating
- Choose the right level and according to the style of the player
- Baghdati [2] makes PCG for spunun generating levels use GA with the Search-based PCG (SBPCG) paradigm [3], but without using DDA (Dynamic Difficulty Adjustment)
- The application of simple adaptation is based on manual rule adjustments, so the process of generating levels is faster
- Using the initial survey, regarding DDA


## PCG and DDA
- DDA is part of the game changed to fit the player, especially the level of difficulty
- Spronck et al. [5] and Hunicke [6] explored different ways to match the Game AI performance with the players’ abilities, different content preferences
- Drachen et al. [7] have detected four different player types in Tomb Raider Underworld with different main goals
- DDA or rather generation of player-adjusted content can be realized via PCG, The commercial example is AI of the game Left 4 Dead, By emotional intensity according to damage dealt and received, then change distrbution of enemy, but the level structure is not changed
- Jennings- Teats et al. [8] realized in their Polymorph system
- Shaker et al. [9] even implement personalized online level generation for a Mario- style platformer
- Lopes et al. [10] use experience-driven PCG for DDA in a relatively simple mobile game
- Shaker et al. [11] employ experience-driven PCG in order to generate content that matches a detailed player model 


## Spelunky
- Spelunky is a rogue-like adventure 2D platformer where player run in the caves and search the exit point to go out
- Spelunker can use weapons to fight enemies (spiders, snakes etc.), bombs to break through walls and ropes to climb up
- Created by David Yu, first released as open source freeware (based on Game Maker) 2008 for Windows, and an updated version with much better graphics and different platforms released at 2012. As it was necessary to make code changes in order to change the way levels are generated, this work is based on the 2008 version
- Starts with a 4 rows 4 columns room layout
- One room in the top row is randomly chosen as entry point, and one room in the bottom row as exit point
- The solution path between these is also randomly determined
- For each room, a matching room template is selected, depending on its connections to neighboring rows and columns
- Then, the obstacles are distributed in each room
- The templates already contain wildcards that mark the places where these can be placed
- In a last step, enemies and treasures are added according to predefined probabilities that take environmental factors into account


## PLAYER SURVEY CONCERNING DDA 
- To get a general idea of what gamers expect of a difficulty adjustment (without a concrete relation to any game)
- A preliminary player survey using oral face-to-face interviews at the VEGA Camp 20146, an international conference on visual effects, games, animation, and mobile media in Stuttgart, Germany, on December 4 and 5, 2014
- All of the 12 participants can be considered as relatively young (between 19 and 25 years), experienced gamers, and one third of them are women
- Presented 10 scenarios to them and asked them to rate these on a scale from 1 to 5
- ”When the player has been killed 2 times by the end boss, the end boss is reduced to 50% of its strength”
- ”When the player has been killed several times due to falling down, the distance to the ground is reduced”
- ”If the player has solved one level without getting damage, the next level will contain more enemies”
- ”When the player has solved all riddles of a level, the number and difficulty of riddles is increased in the next level”
- 

Terrain
- Component for games, simulations, or movies (outdoor environtment)
- Fully automatic or semi-automatic method

Voxel Representation
- Can create rich object like caves and overhangs

PCG
- PCG is a procedural system to create object like texture, geometry, or animation.
- Need for eficient in process, effort, and time (cost effect)
- Help designer to design

Voxel-based approach 
- The presented method expands the concept of shape grammars to a volumetric space

Research 
- Introduce voxel-based approach for generating overhangs and caves
- Create ruleset implemented to voxel
- Create surface using surface net algorithm
- present timings and memory usage from our results for the generation of the voxel data using different rulesets plus the performance statistics of our GPU surface extraction algorithm.
- Collaboration with Sony Interactive Entertainment Euro Research and Development
- Using Phyreengine
- Supported by Nvidia (Titan GPU)


