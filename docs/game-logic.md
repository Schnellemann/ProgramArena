# Game Logic

The different rules and attributes connected to the game

## Unit

A unit has 3 actions to choose between attack, defend and heal. A unit can move.

### Attack

When an unit attacks, the unit chooses a certain direction. The attack works like ball thrown, that will continue flying until the first enemy is hit. An attack does 3 damage when hitting an unit. The direction that can be chosen is like the movement of a queen in chess.

### Defend

A unit using defend, can only take 1 damage from each attack hitting.

### Heal

Heals the unit for 1 hp.

### Movement

Each round a unit can move 1 field, and can choose to move in any direction. if 2 units move to the same field, they will "bounce" off eachother, and lose one health each.

## World
The world size scales depending on the number of players. If a unit is going out of bounds the action kills the unit.
The world is made as a grid, with only one unit on any field at any time. All fields are legal to move to.

## Turn
Each turn there is 3 phases.
Each unit can choose to move 1 time each round.
Each unit can choose between one of the 3 actions, attack, heal or defend, each round.

### Round structure
1. All units perform their move.
2. The units that have chosen either heal or defend, do the action they have chosen.
3. The units that have chosen attack, attacks.
