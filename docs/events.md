# Event Storming
The following is a list of events that occur during game play. 
This documentation is the result of a brain storming activity after having played the board game. The desired result
should accurately reflect all of the factual events that occur during the play of the game.

## Traveled to a neighboring city

    This can happen because:
      * Adjacent Travel Action
      
## Traveled to a non-neighboring city

    This can happen because:
    
      * Direct Travel Action
      * Chartered Travel Action
      * Shuttled Travel Action
      * Dispatched Travel Action
      * Event - Person of Interest (Move any 1 player to any city)
      
## Built an analysis station

    This can happen because:
        
      * Build an Analysis Station Action
      * Event - Government Aid (Add 1 research station to any city, no requirements)
      
## Abandoned an analysis station
      
    This can happen because:
    
      * Build an Analysis Station Action and there are already six Analysis Stations in play
      
## Treated an illness
      
    This can happen because:
    
      * Treat an Illness Action
      * Doctor arrived in a city and illness has been cured        
      
## Shared research
      
    This can happen because:
    
      * Share Research Action

## Cured an illness

    This can happen because:
    
      * Discover Vaccine Action

## Eliminated an illness
      
    This can happen because:
    
      * Illness is cured and there are no instances of that illness in any cities 
      
## Discarded a card
      
    This can happen because:
    
      * Player has too many cards
      
## A city was afflicted with illness
      
    This can happen because:
     
      * Afflict Cities Game Step

## An illness surged

    This can happen because:
    
      * Afflict Citites Game Step and the city is already afflicted with three instances of the illnesss
      
## An epidemic occurred

    This can happen because:
    
      * An epedemic card was drawn
      
## City afflictions were predicted
      
    This can happen because:
    
      * Event - Simulation (draw, look at and rearrange top six cards of the infection deck)
      
## A city became immune to an illness 
      
    This can happen because:
    
      * Event - Preventative Measures (remove any one card in the affliction discard pile from the game)
      
## No cities were afflicted
      
    This can happen because:
      
      * Event - Lucky Break (Skip the next afflict cities step)
      
## Game was lost
      
    This can happen because:
    
      * The surge level reaches the limit
      * Run out of illness instance markers
      * No more player cards
      
## Game was won
      
    This can happen because:
    
      * All four illness types are cured


# What's next?
With the events in mind, it is time to design the domain implementation. 
We know that the entities and or aggregates that we define must accommodate all of the defined events.