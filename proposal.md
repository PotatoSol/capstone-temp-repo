Simple game that based on Pokemon Mystery Dungeon and Final Fantasy 12

Control a party of 1-6 pokemon (might be defaulted to 4 to start with)

Each pokemon, including wild/enemy pokemon, has a list of "tactics" that dictate how they fight

Tactics (Gambits from Final Fantasy 12) are a user defined list of commands that activate under a specific condition

 * Example: 
 1) {IF} Enemy is < 10% HP {THEN} use item(PokeBall)
 2) {IF} Enemy is targetable {THEN} use move(Tackle)

The way this works is that when a pokemon with this tactic list is available to receive a command, it will first check to see if an enemy nearby is 
  under 10% hp, and if they are, then a pokeball will be thrown at that enemy.  (There will be an implicit check to see if the enemy is an elligable target
  for a pokeball, like in the games - an example of a non-eligable target is the pokemon owned by an enemy trainer, while an eligable target is a wild pokemon)

  THEN if the first condition does not get met, it will check the second condition - If there is an enemy that is targetable, then the move "Tackle" will be 
  used on it.  

  If the entire tactics list is exhausted and none of the commands are fulfilled, then there will be a cooldown period before running through the list again. 

---

In regards to the map and the gameplay, I will be referencing a RNG map algorithm.  I haven't decided on the particular one I will use, but I have done
research into roguelikes in the past, and will use a similar algorithm to the map making algorithms used in those games - there are many free ones online
that I can directly reference.  Wild pokemon will be randomly generated, and if I have time, I will implement trainers and gyms and others.  

Assets for Pokemon Mystery Dungeon are freely available online for use. I will likely just be using assets from these games exclusively. 

-- 

MVP for this project is simply the ability for a user to start the game, be assigned a team (either hard coded or randomly generated) and begin combat. 
The game is intended to be run fairly hands-off (an idle incremental game).  I'll probably code a few pokemon to start, ideally I would get 100s of pokemon
coded, but will likely settle for less than 10 to begin with.  A few moves will also be coded at first, but not many.  Pokeballs are unlikely to be added at
first, but are the first stretch goal I have.  

====================================================================

Name of Student: Michael Sol

Name of Project: PokemonTactics {NAME TBD}

Project's Purpose or Goal: Fun video game that can be played with minimal player interaction

List the absolute minimum features the project requires to meet this purpose or goal: Working game with minimal features

What tools, frameworks, libraries, APIs, modules and/or other resources (whatever is specific to your track, and your language) will you use to create this MVP? List them all here. Be specific.

 * Unity
 * C#
 * Pokemon Mystery Dungeon Assets
 * Roguelike RNG Map generation algorithm (stretch)

If you finish developing the minimum viable product (MVP) with time to spare, what will you work on next? Describe these features here: Be specific.
 
 * Additional Pokemon
 * Additional Moves
 * Item Usage
 * Trainer battles
 * Gym Battles
 * Random Events
 * Further Pokemon Attributes (initial attributes will likely just be name, type, moveset, level, and stats - further attributes tbd)
 * Mobile Development****

What additional tools, frameworks, libraries, APIs, or other resources will these additional features require?
 
 * Unsure, but Mobile Development will definitely require more research into android development, a field I have no clue about

Is there anything else you'd like your instructor to know?

 * I plan on researching this further this weekend, and working on beginning this project.  I may end up bailing and just making a website. 
