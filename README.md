# Pacificsts of the Caribbean

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
  should one vessel lose all its hull tokens, the ship sinks and the game is lost.

Place 4 **sea** tiles between each ship. This represents the distance between the ships.

The **captains deck** is created by shuffling the **captain cards**. These hold the actions of the ships whose outcome
the players want to avoid.

Every player is handed one **players deck** <!-- I am not happy with this name, maybe we should find a good position on 
military ships that the players have and use this instead of 'player' -->. This is a complete deck with one and only one
card of every player action there is. Then every player randomly takes 2 cards from their deck and gives one to their
left
neighbour and one to their right neighbour. Every player now takes thees cards on their hand. <!-- not sure about 
the wording here --> Players are not allowed to talk about the content of their hand.

The player that most recently did _not_ partake in any war, gets the **first player** token.

## Playing the Game

The game consists of 7 rounds. In each round the following phases are executed in that order:

* **captains phase** The captains' actions that try to sink the other boats are revealed
* **players phase** The players declare their actions in order to prevent that
* **outcome phase** <!-- better name --> The consequences of the actions are deduced
* **preparation phase** <!-- better name --> The next round is prepared

### Captains' Phase

Beginning with the **first player** in clockwise order, every player draws **two** cards from the **captains deck**.
They
place the first card on the **starboard** side of their ship and the second **portside**.
Both cards are open. <!-- I do not know the english opposite of upside down card -->

Exception: a **side** of the ship where there is no **sea** tile left automatically takes the **boarding combat**
captain action. <!-- the boarding combat captain action should be printed on the ship cardboard sheet on the place where captain 
actions are placed -->

The cards' effects will not be evaluated now. This happens in the **outcome phase**.

### Players Phase

Beginning with the **first player** in clockwise order, every player now plays one card from their hand - or does
nothing.
Once played the same card cannot be played again. The card played is placed upside down next to either the **starboard**
or **portside** captains action. The players card will only modify the captains action it is placed next to.

Players are not allowed to comment on what card they played or what card another player should play.

### Outcome Phase

Now the result of all actions are determined. This happens in the following order:

1. crew assignment
2. boarding combat
3. movement actions
4. artillery actions

Note that some player cards contradict the rules here. In such cases the cards overrule the general rules.

#### Crew Assignment

Every player now reveals their player card played and assigns their remaining **crew** tokens to the **starboard**
and **portside** actions: Half to **starboard**, half to **portside**; reminders to **starboard**.

#### Boarding Combat

These actions are executed simultaneously. For each **boarding combat action** the player on this ship rolls as many
dice as
**crew** tokens are assigned to that action. Every **5** and **6** rolled counts as one _success_. Count the number
of _successes_. These are the number of casualties. After every player determined the number of casualties for their
boarding actions, the casualties are removed from the ships on the side of the boarding actions. Remove casualties first
from the side facing the ship with the boarding action and from the other side afterwards.

Should a ship run out of **crew** tokens now, the players lose the game.

#### Movement Actions

Beginning with the **first player** in clockwise order, the **movement actions** of the ships are executed (**starboard
**
before **portside**). For this the player of the ship rolls a number of six sided dice that equals the **crew** tokens
**assigned** to the movement action. Depending on the number of sails the ship has left, different numbers count as
_successes_:

| sails | successes |
|-------|-----------|
| 0     | 7         |
| 1     | 6,7       |
| 2     | 5,6,7     |
| 3     | 4,5,6,7   |
| 4     | 3,4,5,6,7 |

Count the number of _successes_. The ship will now move by a number of **sea** tiles equal to the number of _successes_. 
The direction depends on the exact card: **Attack Movements** will move towards the neighbouring ship on the side the 
card was played on, while **Retread Movements** will move away from the neighbouring ship on the side the 
card was played on.

To execute an **Attack Movement** remove as many **sea** tiles on the side of the ship as _successes_ were rolled. If
more _successes_ were rolled than **sea** tiles exist on this side, remove one **hull** token from the neighbouring ship
on this side for every _success_ over the number of **sea** tiles.

To execute a **Retread Movement** add as many **sea** tiles on the side of the ship as _successes_ were rolled.

#### Artillery Actions

These actions are executed simultaneously.

First, For each **artillery action** check whether it will hit something or not: An **artillery action**
has a **range** and a **spread**. An artillery action hits every ship in the direction of the
action that is more than **range** and less than **range + spread** **fields** away. A **field** is either a **sea**
tile or a **ship**.

If no ship is hit, ignore the action. Otherwise, determine the amount of damage by rolling as many six sided dice as
**crew** tokens are assigned to this action. Every **5** and **6** rolled counts as one _success_. The number of
_successes_ is the damage that **every** ship hit by this **artillery action** takes.

Note: Some Artillery cards have an **attack modifier** (-1 or +1). Add this modifier to every die rolled, when 
determining _successes_ (treat results of 7 or higher as 6).

After the damage for every **artillery action** is calculated it is applied. For every **artillery action** every ship
hit removes as many tokens as damage was calculated by this action. The types of token to remove depend on the
ammunition used by the action:

* chainshot: remove **sails** tokens
* grapeshot: remove **crew** tokens
* solid: remove **hull** tokens
* explosive: remove damage from **sails**, **crew** _and_ **hull** tokens

If a ship damaged loses all its **crew** or **hull** tokens, the players lose the game.

#### Preparation Phase

The number of human casualties (**crew** tokens removed by **artillery** and **boarding actions**) this round are
counted. If it is below the number of players, remove one **sea** tile between every ship. If it is above 2 times the
number of players add one **sea** tile between every ship.

All cards played and tokens removed are out of the game and placed in the game box. The **first player** gives the
**first player** token to his **portside** neighbour.

If this was the last round of the game, the players win with the sum of **crew** tokens left on the ship.

## Cards

### Captain Actions

* Artillery RANGE, SPREAD, AMMUNITION
* Attack Movement
* Retread Movement

### Player Actions

* "The Other Starboard"
    * the captains card changes its direction
    * artillery shoots in the other direction
    * attack movement becomes retread movement and vice versa
* change assignment
    * the crew assigned to this action are assigned to the action on the other side
* demotivate
    * _successes_ will be one number harder
    * i.e. evaluate every die as if it rolled a number **one less** than it did
* There will be Grog
    * _successes_ will be one number easier
    * i.e. evaluate every die as if it rolled a number **one higher** than it did
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
    * It will be evaluated as if there is another movement card on the other side
    * No effect on non-movement cards
* Defect
    * can only be played on boarding-actions
        * instead of producing a casualty, every _success_ of the boarding action will make one **crew** token move
          from this ship to the ship attacked
* Belay that order
    * When this card is revealed, immediately replace the affected **captains card** with the next on the **captains
      deck**. 

  