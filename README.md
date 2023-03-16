# Pacifists of the Caribbean

A cooperative board game, where you try to omit as many human loss as you can in a 17th century naval battle. The game
can be played with 3-8 players.
<!-- we should find a good maximum number of players. Playtesting!! -->

## Set Up

Each player is on a different ship which is placed in front of him. The ship has tokens for **sails**, **crew** and
**hull**. Each ship starts with **4 sails**, **8 crew** and **6 hull**.

As the ships take damage in the course of the game, tokens will be removed from the ship.

* **sails** represent the integrity of the vessels sails. Loosing them will make movement actions less effective.
* **crew** tokens represent the persons working on the ship. It is the goal of this game to lose as few as possible of
  them.
  Also, all actions of the vessel will be less effective the fewer **crew** it has.
* **hull** tokens represent the integrity of the vessels body. Loosing them will have no effect at first. However,
  should one vessel lose all its hull tokens, the ship sinks and all players lose the game.

Place 4 **sea** tiles between each ship. This represents the distance between the ships.

The **captains deck** is created by shuffling the **captain cards**. These hold the actions of the ships whose outcome
the players want to avoid.

The **players deck** os created by shuffling the **players cards**. These cards hold the actions the players may 
execute to undermine the captains actions. Every player gets 3 **players cards** in their hand. Players are not allowed 
to talk about the content of their hand.

<!-- 
The player that most recently did _not_ partake in any war, gets the **first player** token.
-->

## Playing the Game

The game consists of 7 rounds. In each round the following phases are executed in that order:

* **captains phase** The captains' actions that try to sink the other boats are revealed
* **players phase** The players declare their actions in order to prevent that
* **resolution phase** The consequences of the actions are deduced
* **cleanup phase** <!-- better name --> The next round is prepared

### Captains' Phase

Deal **two** cards from the **captains deck** to each player. Place the first card on the **starboard** side of 
their ship and the second **portside**. Both cards are face up. 

Exception: a **side** of the ship where there is no **sea** tile left automatically takes the **boarding combat**
captain action. Do not draw a card in this case. 
<!-- the boarding combat captain action should be printed on the ship cardboard sheet on the place where captain 
actions are placed -->

The cards' effects will not be evaluated now. This happens in the **resolution phase**.

### Players Phase

Now the players may take their turns. There is no specific order to this, however the turns are taken one after the 
other, not simultaneously. For your first games it is advised to determine one start player and then take turns in 
clockwise order.  

When taking a turn a player chooses one of 3 options:

  1. Play no card, draw 2 cards
  2. Play 1 card, draw 1 card
  3. Play 2 cards, draw no card

When playing cards players place the card upside down next to either the **starboard** or **portside** captains action. 
The players card will (in most cases) only affect the captains action it is placed next to.

Cards are drawn after cards are played. The cards drawn can earliest be played next round.

Players are not allowed to comment on what card they played or what card another player should play.

### Resolution Phase

Now the result of all actions are determined. This happens in the following order:

1. crew assignment
2. movement actions
3. boarding combat
4. artillery actions

Note that some player cards contradict the rules here. In such cases the cards overrule the general rules.

#### Crew Assignment

Every player now reveals their player card played and assigns their remaining **crew** tokens to the **starboard**
and **portside** actions: Half to **starboard**, half to **portside**; reminders to **starboard**.

#### Movement Actions

Resolve **Retread Movements** first, then **Attack Movements**. Resolve different **Retread Movements** in an arbitrary 
order, as well as **Attack Movements**.

For each movement action, first determine the movement distance. It is the minimum of crew assigned to the action and
 one plus **sails** tokens the vessel has left. This is the number of **sea** tiles the ship moves.

Example: a movement action has assigned 8 crew and all 4 of its sails left. The distance is min(8, 1 + 4) = 5. The 
movement action will move the vessel by 5 tiles. 

The direction depends on the exact card: **Attack Movements** will move towards the neighbouring ship on the side the 
card was played on, while **Retread Movements** will move away from the neighbouring ship on the side the 
card was played on.

To execute an **Attack Movement** _remove_ as many **sea** tiles on the side of the ship as the movements **distance**. If
this is more than **sea** tiles exist on this side, ramming occurs (see below).

To execute a **Retread Movement** add as many **sea** tiles on the side of the ship as the movements **distance**.

##### Ramming

Whenever a movement distance is higher than the **sea** tiles present, ramming occurs. The vessels between which the 
movement occurred take damage to their hull. For every point movement **distance** over the number of **sea** tiles 
available _before_ executing the movement the players of the affected ships roll one die each. The ships take one **hull** 
damage for every **4**, **5** and **6** rolled by their player. If one of the ships ran out of **hull** tokens the players
lose the game.

#### Boarding Combat

These actions are executed simultaneously. For each **boarding combat action** the player on this ship rolls as many
dice as
**crew** tokens are assigned to that action. Every **4**, **5** and **6** rolled counts as one _success_. Count the number
of _successes_. These are the number of casualties. After every player determined the number of casualties for their
boarding actions, the casualties are removed from the ships on the side of the boarding actions. Remove casualties first
from the side facing the attacking ship and from the other side afterwards.

Should a ship run out of **crew** tokens now, the players lose the game.


#### Artillery Actions

These actions are executed simultaneously.

First, for each **artillery action** check whether it will hit something or not: An **artillery action**
has a **range** and a **spread**. An artillery action hits every ship in the direction of the
action that is more than **range** and less than **range + spread** **fields** away. A **field** is either a **sea**
tile or a **ship**.

If no ship is hit, ignore the action. Otherwise, determine the amount of damage by rolling as many six sided dice as
**crew** tokens are assigned to this action. Every **4**, **5** and **6** rolled counts as one _success_. The number of
_successes_ is the damage that **every** ship hit by this **artillery action** takes.

Note: Some Artillery cards have an **attack modifier** (-1 or +1). Add this modifier to the number of dies rolled.

After the damage for every **artillery action** is calculated it is applied. For every **artillery action** every ship
hit removes as many tokens as damage was calculated by this action. The types of token to remove depend on the
ammunition used by the action:

* chainshot: remove **sails** tokens
* grapeshot: remove **crew** tokens
* solid: remove **hull** tokens
* explosive: remove damage from **sails**, **crew** _and_ **hull** tokens

If a ship damaged loses all its **crew** or **hull** tokens, the players lose the game. 
Excessive chainshot damage that exceeds the ships **sails** tokens has no effect.

#### Cleanup Phase

The number of human casualties (**crew** tokens removed by **artillery** and **boarding actions**) this round are
counted. If it is below the number of players, remove one **sea** tile between every ship. If it is above 2 times the
number of players add one **sea** tile between every ship.

All cards played and tokens removed are out of the game and placed in the game box. 

If this was the last round of the game, the players win with the sum of **crew** tokens left on the ship.

## Cards

### Captain Actions

* Artillery RANGE, SPREAD, AMMUNITION
* Attack Movement
* Retreat Movement

### Player Actions

* "The Other Starboard"
    * the captains card changes its direction
    * It is executed as if it was played on the other side
      * The crew used is from its original side
* "This is not your Post"
    * the crew assigned to this action are assigned to the action on the other side
* demotivate
    * Evaluate action as if there is one less **crew** token assigned
* There will be Grog
    * Evaluate action as if there is one more **crew** token assigned
* further
    * The range of the artillery card is increased by 3
    * no effect on non-artillery actions
* nearer
    * The range of the artillery card is decreased by 3
    * no effect on non-artillery actions
* There is Grog
    * The crew assigned to this action is halved (rounding down)
* Both sides
    * The effect of the movement card is applied to both sides of the ship
    * No effect on non-movement cards
* Defect
    * can only be played on boarding-actions
        * instead of producing a casualty, every _success_ of the boarding action will make one **crew** token move
          from this ship to the ship attacked
* "Belay that order"
    * When this card is revealed, immediately replace the affected **captains card** with the next on the **captains
      deck**.
* "Arm the Mariners"
    * Remove the affected **captains card**
    * Instead, a boarding combat action is executed
    * This boarding combat is executed as if one more **crew** token was assigned


